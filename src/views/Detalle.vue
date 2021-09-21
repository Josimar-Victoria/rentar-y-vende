<template>
  <div class="detalle">
    <div class="img-header">
      <div class="icons">
        <div class="icons-container">
          <div class="icon">
            <i class="bx bxs-chevron-left"></i>
          </div>
          <div class="text">Available</div>
          <div class="icon color-pink">
            <i class="bx bx-heart"></i>
          </div>
        </div>
      </div>
      <img
        src="https://images.unsplash.com/photo-1585670149967-b4f4da88cc9f?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=500&q=80"
        alt="detalle"
      />
    </div>
    <div class="detalle-text">
      Lorem ipsum dolor sit amet, consectetur adip minim veniam, sed do eiusmod
      tempor incidunt ut labore et dolore magna aliqua. Ut enim ad minim veniam
      nib nibh euismod Lorem ipsum dolor sit amet, consectetur adip minim
      veniam, sed do eiusmod tempor incidunt ut labore et dolore magna aliqua.
      Ut enim ad minim veniam nib nibh euismod Lorem ipsum dolor sit amet,
      consectetur adip minim veniam, sed do eiusmod tempor incidunt ut labore et
      dolore magna aliqua. Ut enim ad minim veniam nib nibh euismod Lorem ipsum
      dolor sit amet, consectetur adip minim veniam, sed do eiusmod tempor
      incidunt ut labore et dolore magna aliqua. Ut enim ad minim veniam nib
      nibh euismod
    </div>
  </div>
</template>

<style scoped>
.img-header {
  width: 100%;
  height: 50vh;
  position: relative;
  top: 0;
}
.icons {
  position: fixed;
  width: 100%;
}
.icons-container{
  display: flex;
  justify-content: space-between;
  padding:20px;
  align-items: center;
}
.icon{
  background-color: white;
  padding: 10px;
  border-radius: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
}
.text{
  background-color:rgba(108, 200, 117);
  padding: 10px;
  border-radius: 20px;
  color: white
}
.color-pink{
  color: rgba(233, 73, 22)
}
img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
.detalle-text {
  z-index: 1000;
  margin-top: -10;
  position: absolute;
  border-radius: 20px;
  background-color: #fff;
  padding: 20px;
}
</style>
