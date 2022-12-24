<template>
    <!--image slider start-->
    <div class="sliderContainer">
        <h4>Developers</h4>
        <div class="slider">
        <div class="slides">
            <!--radio buttons start-->
            <input type="radio" name="radio-btn" id="radio1">
            <input type="radio" name="radio-btn" id="radio2">
            <input type="radio" name="radio-btn" id="radio3">
            <input type="radio" name="radio-btn" id="radio4">
            <!--radio buttons end-->
            <!--slide images start-->
            <div class="slide first">
            <img class="slideImages" src="@/assets/Hailemelekot.png" alt="">
            </div>
            <div class="slide">
            <img class="slideImages" src="@/assets/jonatan-pie-3l3RwQdHRHg-unsplash.jpg" alt="">
            </div> 
            <!--slide images end-->
            <!--automatic navigation start-->
            <div class="navigation-auto">
              <div class="auto-btn1"></div>
              <div class="auto-btn2"></div>
            </div>
            <!--automatic navigation end-->
        </div>
        <!--manual navigation start-->
        <div class="navigation-manual">
            <label for="radio1" class="manual-btn"></label>
            <label for="radio2" class="manual-btn"></label>
        </div>
        <!--manual navigation end-->
        </div>
    </div>
    <!--image slider end-->
</template>

<script>
export default {
   data() {
    return {
        counter: 1,
    }
    },
    created() {
      this.startInterval();
    },
    methods: {
        startInterval: function() {
          setInterval(() => {
                document.getElementById('radio' + this.counter).checked = true;
                this.counter++;
                if (this.counter > 2) {
                    this.counter = 1;
                }
            }, 3000)
        },
    },
}
</script>

<style scoped>
.sliderContainer{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 40px;
} 
.sliderContainer h4{
  font-size: 23px;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
  font-weight: bold;
  text-decoration: 2px rgb(14, 22, 144) underline double;
  /* border-bottom:2px solid #40D3DC; */
}
.slider{
  width: 800px;
  height: 500px;
  border-radius: 10px;
  overflow: hidden;
}

.slides{
  width: 500%;
  height: 500px;
  display: flex;
}

.slides input{
  display: none;
}

.slide{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 20%;
  transition: 1s;
  height: 300px;
  overflow: hidden;
 }

.slide img{
  width: auto;
  max-width: 500px;
  height: 300px;
 }

/*css for manual slide navigation*/

.navigation-manual{
  position: absolute;
  width: 800px;
  margin-top: -40px;
  display: flex;
  justify-content: center;
  top: 1300px;
}

.manual-btn{
  border: 2px solid #a6a5a5;
  padding: 5px;
  border-radius: 10px;
  cursor: pointer;
  transition: 1s;
}

.manual-btn:not(:last-child){
  margin-right: 40px;
}

.manual-btn:hover{
  background: #ffffff;
}

#radio1:checked ~ .first{
  margin-left: 0;
}

#radio2:checked ~ .first{
  margin-left: -20%;
}

/*css for automatic navigation*/

.navigation-auto{
  position: absolute;
  display: flex;
  width: 800px;
  justify-content: center;
  margin-top: 460px;
  top: 800px;
}

.navigation-auto div{
  border: 2px solid #828282;
  padding: 5px;
  border-radius: 10px;
  transition: 1s;
}

.navigation-auto div:not(:last-child){
  margin-right: 40px;
}

#radio1:checked ~ .navigation-auto .auto-btn1{
  background: #ffffff;
}

#radio2:checked ~ .navigation-auto .auto-btn2{
  background: #ffffff;
}

@media screen and (max-width:890px){
  .sliderContainer{
    margin-top: -100px;
    margin-bottom: 0px;
    padding: 0;
    padding: 5px;
    transform: scale(0.5);
  }
  .navigation-auto{
  top: -100px;
  }
  .navigation-manual{
  top: 400px;
  }
}
@media screen and (max-width:281px){
   .sliderContainer{
    margin-top: -100px;
    margin-bottom: 0px;
    padding: 0;
    padding: 5px;
    transform: scale(0.3);
  }
  .navigation-auto{
  top: -100px;
  }
  .navigation-manual{
  top: 400px;
  }
}

</style>