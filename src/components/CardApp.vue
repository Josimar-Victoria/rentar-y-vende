<template>
  <div class="card">
    <div class="card-content">
      <div class="tag-card">Los Angeles CA</div>
      <div class="footer-card-container">
        <div class="action">
          <button>
            <i class="bx bx-heart"></i>
          </button>
        </div>
        <div class="footer-card">
          <div class="footer-card-left">
            <div class="title">
              <h3>{{ title }}</h3>
            </div>
            <div class="user">
              <div class="content-user">
                <div class="img-content">
                  <img :src="imgUser" alt="avatar-user" />
                </div>
                <div class="username">
                  {{ username }}
                </div>
              </div>
              <div class="starts">
                <span><i class="bx bxs-star"></i></span>
                <span><i class="bx bxs-star"></i></span>
                <span><i class="bx bxs-star"></i></span>
                <small>{{ Start }} Start</small>
              </div>
            </div>
          </div>
          <div class="footer-card-right">
            <div class="price">
              <h2>${{ price }} Cop</h2>
            </div>
            <div class="rooms">
              <div class="room-item">
                <i class="bx bx-bed"></i>
                2
              </div>
              <div class="room-item">
                <i class="bx bx-cloud-light-rain"></i>
                2
              </div>
              <div class="room-item">
                <i class="bx bx-cloud-light-rain"></i>
                2
              </div>
            </div>
          </div>
        </div>
      </div>
      <img :src="imgCard" alt="img" />
    </div>
  </div>
</template>

<script>
export default {
  name: "CardApp",
  props: {
    title: {
      type: String,
      default: "Not Found",
    },
    imgUser: {
      type: String,
      default:
        "https://us.123rf.com/450wm/mialima/mialima1603/mialima160300025/55096766-hombre-icono-de-usuario-aislado-en-un-fondo-blanco-avatar-cuenta-para-la-web-foto-de-perfil-de-usuar.jpg?ver=6",
    },
    imgCard: {
      type: String,
      default:
        "https://st3.depositphotos.com/23594922/31822/v/600/depositphotos_318221368-stock-illustration-missing-picture-page-for-website.jpg",
    },
    price: {
      type: Number,
      default: 0,
    },
    username: {
      type: String,
      default: "Not found",
    },
    Start: {
      type: Number,
      default: 0,
    },
  },
};
</script>

<style scoped>
.card-content {
  box-shadow: 0px 5px 10px -2px rgba(74, 54, 251, 0.2);
  border-radius: 20px;
  width: 100%;
  overflow: hidden;
  height: 360px;
  position: relative;
}
.tag-card {
  font-size: 18px;
  margin: 20px;
  top: 0;
  position: absolute;
  border-radius: 16px;
  background-color: rgb(244, 242, 243);
  padding: 8px;
  z-index: 3000;
}
.action {
  position: absolute;
  bottom: 38%;
  right: 20%;
  z-index: 3000;
}
button {
  box-shadow: 0px 5px 10px -2px rgba(74, 54, 251, 0.2);
  border: none;
  outline: none;
  border-radius: 50px;
  background-color: white;
  padding: ;
}

.footer-card {
  border-radius: 20px;
  height: 140px;
  position: absolute;
  bottom: 0%;
  width: 100%;
  display: flex;
  background-color: #fff;
  display: flex;
  align-items: center;
}

.footer-card-left {
  display: flex;
  flex-direction: column;
  width: 60%;
}
.title {
  margin: 5px;
  text-align: start;
}
.footer-card-left .img-content img {
  width: 40px;
  height: 40px;
  border-radius: 50px;
  object-fit: cover;
}
.title {
  text-align: center;
  margin-top: 0;
}
.user {
  display: flex;
  flex-direction: column;
  margin-left: 10px;
}
.content-user {
  display: flex;
  align-items: center;
}
.username {
  margin-left: 10px;
}
.starts {
  text-align: start;
  display: flex;
  align-items: center;
  color: rgba(0, 0, 0, 0.9);
}
.starts small {
  margin-left: 5px;
}

i {
  color: rgb(108, 200, 117);
  margin: 3px;
}
.footer-card-right {
  width: 40%;
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 100%;
  margin: 12px;
}
.rooms {
  display: flex;
  justify-content: space-between;
}
.room-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
img {
  width: 100%;
  height: 100%;
}
.img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
