<template>
  <div class="detalle">
    <div class="img-header">
      <div class="icons">
        <div class="icons-container">
          <div @click="changeState" class="icon">
            <router-link to="/">
              <i class="bx bxs-chevron-left"></i>
            </router-link>
          </div>
          <div class="text">Available</div>
          <div class="icon color-pink">
            <i class="bx bx-heart"></i>
          </div>
        </div>
      </div>
      <img
        src="https://cloudfront-us-east-1.images.arcpublishing.com/semana/RFMYKD3VLNBHPPM4R2EV3DRNNM.jpg"
        alt="detalle"
      />
    </div>
    <div class="view-text">
      <div class="view-text-content">
        <div class="header-view">
          <div class="left">
            <div class="location">
              <i class="bx bx-current-location"></i>
              Colombia
            </div>
            <h2 class="title-text">
              Sṕecial House Mix
            </h2>
          </div>
          <div class="right">
            <div class="top-bar-img">
              <img
                src="https://conceptodefinicion.de/wp-content/uploads/2015/03/hombre.jpg"
                alt="img"
              />
            </div>
          </div>
        </div>
        <div class="tags-view">
          Hight speed wifi | Deskspace | Safe location
        </div>
        <div class="icons-view">
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
        <div class="options-view">
          <button class="selected">
            <i class="bx-sm bx bxs-info-circle"></i>
            Information
          </button>
          <button>
            <i class="bx-sm bx bx-comment-dots"></i>
            Contactar
          </button>
          <button>
            <i class="bx-sm bx bxs-offer"></i>
            Offert
          </button>
          <button>
            <i class="bx-sm bx bx-share-alt"></i>
            Share
          </button>
        </div>
        <div class="description-view">
          <h1>Description</h1>
          <small
            >lorem ipsum dolor sit amet, lorem ipsum dolor sit amet lorem ipsum
            dolor sit amet lorem ipsum d lorem ipsum dolor sit amet lorem ipsum
            lorem ipsum dolor sit amet lorem ipsum d lorem ipsum dolor sit amet
            lorem ipsum d lorem ipsum dolor sit amet lorem ipsum d >lorem ipsum
            dolor sit amet, lorem ipsum dolor sit amet lorem ipsum dolor sit
            amet lorem ipsum d lorem ipsum dolor sit amet lorem ipsum lorem
            ipsum dolor sit amet lorem ipsum d lorem ipsum dolor sit amet lorem
            ipsum d lorem ipsum dolor sit amet lorem ipsum d >lorem ipsum dolor
            sit amet, lorem ipsum dolor sit amet lorem ipsum dolor sit amet
            lorem ipsum d lorem ipsum dolor sit amet lorem ipsum lorem ipsum
            dolor sit amet lorem ipsum d lorem ipsum dolor sit amet lorem ipsum
            d lorem ipsum dolor sit amet lorem ipsum d >lorem ipsum dolor sit
            amet, lorem ipsum dolor sit amet lorem ipsum dolor sit amet lorem
            ipsum d lorem ipsum dolor sit amet lorem ipsum lorem ipsum dolor sit
            amet lorem ipsum d lorem ipsum dolor sit amet lorem ipsum d lorem
            ipsum dolor sit amet lorem ipsum d
          </small>
        </div>
      </div>
    </div>
    <div class="bottom-price">
      <div class="content">
        <p class="precio">$1500</p>
        <ButtomApp color="primary">Reserved Now!</ButtomApp>
      </div>
    </div>
  </div>
</template>
<script>
import ButtomApp from "@/components/ButtomApp.vue";

export default {
  components: {
    ButtomApp,
  },
  created() {
    this.$store.state.isView = true;
  },
  methods: {
    changeState() {
      this.$store.state.isView = false;
    },
  },
};
</script>

<style scoped>
.bottom-price {
  background-color: #fff;
}

.content {
  display: flex;
  width: 100%;
  justify-content: space-between;
}
.precio {
  font-size: 28px;
}
.img-header {
  width: 100%;
  height: 50vh;
  position: relative;
  top: 0;
  object-fit: cover;
}
.icons {
  position: fixed;
  width: 100%;
}
.icons-container {
  display: flex;
  justify-content: space-between;
  padding: 20px;
  align-items: center;
}
.icon {
  background-color: #fff;
  padding: 8px;
  border-radius: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
}
.text {
  background-color: rgba(108, 200, 117);
  padding: 10px;
  border-radius: 20px;
  color: white;
}
.color-pink {
  color: rgba(233, 73, 22);
}
img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
.view-text {
  z-index: 1000;

  border-radius: 25px;
  background-color: #fff;
  padding: 20px;
  width: 90%;
}
.title-text {
  font-weight: bold;
}
.header-view {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-right: 40px;
}
.top-bar-img {
  width: 44px;
  height: 44px;
  overflow: hidden;
  border-radius: 25px;
}
.top-bar-img img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
.icons-view {
  width: 60%;
  margin-top: 10px;
  align-items: center;
  display: flex;
  justify-content: space-between;
}
i {
  color: rgb(108, 200, 117);
  margin: 3px;
  font-weight: bold;
}
.options-view {
  display: flex;

  justify-content: space-between;
}
.options-view button {
  border: none;
  background: transparent;
  font-weight: bold;
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  align-items: center;
  margin-top: 20px;
}
.options-view button i {
  color: rgb(44, 62, 80);
  align-items: center;
  margin: 0 auto;
}
.selected {
  color: rgb(108, 200, 117);
}

.description-view {
  overflow: hidden;
}
.description-view p {
  color: rgba(164, 179, 192);
  font-size: 30rem;
  font-weight: bold;
}
.description-view small {
  font-size: 18px;
  font-weight: bold;
}
</style>
