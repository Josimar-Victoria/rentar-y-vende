<template>
  <div class="home">
    <div class="title">
      <p>Hola Harry</p>
      <p class="text-bold">Bienvenido a Renta y Venta....</p>
    </div>
    <div class="input">
      <input type="text" placeholder="Buscar...." />
      <i class="slider bx bx-slider bx-rotate-90"></i>
    </div>
    <div class="tags">
      <div class="icons-tags selected">
        <i class="bx-sm bx bx-home-smile"></i>
      </div>
      <div class="icons-tags">
        <i class="bx-sm bx bx-building-house"></i>
      </div>
      <div class="icons-tags">
        <i class="bx-sm bx bxs-offer"></i>
      </div>
      <div class="icons-tags">
        <i class="bx-sm bx bx-grid-alt"></i>
      </div>
    </div>
    <CardApp
      style="margin-top: 20px"
      title="apartamento"
      imgUser="https://images.unsplash.com/photo-1501196354995-cbb51c65aaea?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80"
      imgCard="https://images.unsplash.com/photo-1593696140826-c58b021acf8b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1yZWxhdGVkfDE5fHx8ZW58MHx8fHw%3D&auto=format&fit=crop&w=500&q=60"
      price="400"
      username="Harry Campaz"
      Start="20"
      :key="index"
      v-for="(item, index) in 10"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import CardApp from "@/components/CardApp.vue";

export default {
  name: "Home",
  components: {
    CardApp,
  },
};
</script>

<style scoped>
.home {
  padding: 10px;
}
.title {
  margin-top: 70px;
  margin-bottom: 0px;
}
p {
  color: rgb(0, 0, 0, 0.7);
  font-size: 18px;
}
.text-bold {
  font-weight: bold;
}
.input {
  width: 100%;
  display: flex;
  position: relative;
  align-items: center;
}
input {
  padding: 10px;
  border: none;
  outline: none;
  margin-bottom: 20px;
  width: 100%;
  border-radius: 10px;
  background-color: white;
  box-shadow: 0px 5px 10px -2px rgba(74, 54, 251, 0.2);
}
.slider {
  position: absolute;
  right: 0;
  align-items: center;
  color: rgba(69, 208, 215);
  font-size: 1.3rem;
}

.tags {
  display: flex;
  justify-content: space-between;
}
.icons-tags{
  background-color: rgb(0,0,0,0.1);
  padding: 24px;
  border-radius: 10px;
  font-size: 20px;
  magin-top: 10px;
}
.selected{
  color: white;
background-color: rgba(69, 208, 215);
}
</style>
