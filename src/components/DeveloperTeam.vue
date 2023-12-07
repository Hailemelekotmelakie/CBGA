<template>
  <div>
    <h3 class="Developers">Developers</h3>
    <div class="sliderContainer">
      <div class="person">
        <div class="container">
          <div class="container-inner">
            <img class="circle" src="@/assets/pngtree-male-avatar-vector-icon-png-image_691595.jpg" />
          </div>
        </div>
        <div class="divider"></div>
        <div class="name">Hailemelekot</div>
        <div class="title">Developer</div>
        <div class="tel">Tel: <a href="tel:+251947053537">+251 947 053 537</a></div>
      </div>
      <div class="person">
        <div class="container">
          <div class="container-inner">
            <img class="circle"
              src="@/assets/businessman-icon-image-male-avatar-profile-vector-glasses-beard-hairstyle-179728610.jpg" />
          </div>
        </div>
        <div class="divider"></div>
        <div class="name">Dagim</div>
        <div class="title">UX/UI Designer</div>
        <div class="tel">Tel: <a href="tel:+251947053537">+251 947 053 537</a></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
    }
  },

}
</script>

<style scoped>
.Developers {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0px 50px;
  gap: 20px;
  font-size: 26px;
  width: 30%;
  margin: auto;
  padding: auto;
  margin-top: 40px;
  border-bottom: 2px solid #07110c;
}

.sliderContainer {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  padding: 0px 50px;
  margin-top: 20px;
  gap: 20px;
}

.person {
  align-items: center;
  display: flex;
  flex-direction: column;
  width: 250px;
  transition: 1s;
  cursor: pointer;
  padding: 10px;
  border-radius: 4px;
  box-shadow: inset 0px 0px 50px rgba(255, 255, 255, 0.809);
  border: 1px solid rgba(177, 177, 177, 0.809);
}

.person:hover {
  background-color: #84848439;
}

.container {
  border-radius: 50%;
  height: 312px;
  -webkit-tap-highlight-color: transparent;
  transform: scale(0.48);
  transition: transform 250ms cubic-bezier(0.4, 0, 0.2, 1);
  width: 400px;
}

.container:hover {
  transform: scale(0.54);
}

.container-inner {
  clip-path: path("M 390,400 C 390,504.9341 304.9341,590 200,590 95.065898,590 10,504.9341 10,400 V 10 H 200 390 Z"
    );
  position: relative;
  transform-origin: 50%;
  top: -240px;
}

.circle {
  background-color: #ffffff;
  border-radius: 50%;
  cursor: pointer;
  height: 363px;
  left: 10px;
  pointer-events: none;
  position: absolute;
  top: 210px;
  width: 363px;
  box-shadow: 1px 1px 100px black;
  margin: 10px;
}

.img {
  pointer-events: none;
  position: relative;
  transform: translateY(20px) scale(1.15);
  transform-origin: 50% bottom;
  transition: transform 300ms cubic-bezier(0.4, 0, 0.2, 1);
}

.container:hover .img {
  transform: translateY(0) scale(1.2);
}

.img1 {
  left: 22px;
  top: 164px;
  width: 340px;
}

.img2 {
  left: -46px;
  top: 174px;
  width: 444px;
}

.img3 {
  left: -16px;
  top: 144px;
  width: 466px;
}

.divider {
  background-color: #5be6a1;
  height: 1px;
  width: 160px;
}

.name {
  color: #404245;
  font-size: 30px;
  font-weight: 600;
  margin-top: 16px;
  text-align: center;
}

.title {
  color: #6e6e6e;
  font-family: arial;
  font-size: 14px;
  font-style: italic;
  margin-top: 4px;
}

.tel {
  color: #6e6e6e;
  font-family: arial;
  font-size: 12px;
  font-style: italic;
  margin-top: 4px;
}

a {
  color: #07110c;
}

@media screen and (max-width:800px) {
  .sliderContainer {
    padding: 10px;
    flex-direction: column;
  }

  .person {
    width: 80%;
  }
}
</style>