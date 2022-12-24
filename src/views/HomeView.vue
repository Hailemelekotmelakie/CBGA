<template>
  <div class="home">
    <div class="homeUp">
      <div class="homeLabelContainer">
        <div class="homeLabelContainerUp">
          We Are Center for Budgetary Governance Advocacy
        </div>
        <button class="homeButtonContainerUp">Get Started</button>
      </div>
      <div class="homeLabelContainer">
        <iframe src="https://embed.lottiefiles.com/animation/96413"></iframe>
      </div>
    </div>
    <div class="homeDown">
      <div class="WhoWeAre">Who We Are</div>
      <div class="WhoWeAreDesc">
        Center for Budgetary Governance Advocacy (CBGA) is a Non-governmental Organization
        established in Ethiopia in order to advocate for robust budgetary governance
        throughout government organizations and goal orientation towards Sustainable
        Development Goals (SDGs)
      </div>
    </div>  
    <DropDown></DropDown>
    <LookingFor></LookingFor>
  </div>
</template>

<script>
import DropDown from '@/views/DropDown.vue'
import LookingFor from '@/views/LookingFor.vue'
export default {
  name: "HomeView",
  components: {
    DropDown:DropDown,
    LookingFor:LookingFor
  },
  data() {
    return {};
  },
};
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  padding: 0px 50px;
}
.homeUp {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}
.homeLabelContainerUp {
  display: flex;
  font-size: 30px;
  text-align: center;
  font-weight: bold;
}
.homeLabelContainer {
  display: flex;
  text-align: center;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.homeButtonContainerUp {
  display: flex;
  font-size: 18px;
  text-align: center;
  font-weight: bold;
  border: none;
  border-radius: 7px;
  background-color: rgb(46, 100, 100);
  color: aliceblue;
  padding: 10px 20px;
  margin: 10px;
  cursor: pointer;
  margin: 10px;
  transition: 0.4s;
}
.homeButtonContainerUp:hover {
  background-color: rgb(66, 164, 128);
}
.homeLabelContainer {
  display: flex;
  flex: 1;
  margin: 0px;
  padding: 0px;
}

iframe {
  width: 100%;
  height: auto;
  min-height: 280px;
  max-height: 400px;
  border: none;
  padding: 0;
  margin: 0;
}
.homeDown {
  margin-top: 30px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 20px;
}
.WhoWeAre {
  font-size: 30px;
  font-weight: 600;
}
.WhoWeAreDesc {
  max-width: 650px;
  font-size: 14px;
  font-weight: 500;
  line-height: 1.5rem;
  padding: 10px;
}
@media screen and (max-width: 800px) {
  .home {
    padding: 5px;
  }
  .homeUp {
    flex-direction: column;
  }
  .homeLabelContainerUp {
    font-size: 15px;
    margin-top: 20px;
  }
  .WhoWeAre {
    font-size: 15px;
  }
}
</style>
