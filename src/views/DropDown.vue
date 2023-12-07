<template>
    <div class="container">
      <div class="card">
        <div class="face face1">
          <div class="content">
            <h3>Mission</h3>
          </div>
        </div>
        <div class="face face2">
          <div class="content">
            <p>Lorem
              at.</p>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="face face1">
          <div class="content">
            <h3>Plan</h3>
          </div>
        </div>
        <div class="face face2">
          <div class="content">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident
              at.</p>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="face face1">
          <div class="content">
            <h3>Vision</h3>
          </div>
        </div>
        <div class="face face2">
          <div class="content">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident
              at.</p>
          </div>
        </div>
      </div>
    </div>
</template>

<style scoped> 

.container{
    width: auto;
    position: relative;
    display: flex;
    justify-content: space-between;
    flex-direction: row;
    padding: 10px 25px;
    gap: 10px;
}

.container .card{
    position: relative;
    cursor: pointer;
    display: flex;
    flex-direction: column;
    flex: 1;
}

.container .card .face{
    width: auto;
    height: 130px;
    transition: 0.5s;
}

.container .card .face.face1{
    position: relative;
    background: rgb(67, 186, 121);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1;
    transform: translateY(30px);
}

.container .card:hover .face.face1{
    background: #5ed9a1;
    transform: translateY(0);
}

.container .card .face.face1 .content{
    opacity: 0.8;
    transition: 0.5s;
}

.container .card:hover .face.face1 .content{
    opacity: 1;
}


.container .card .face.face1 .content h3{
    margin: 10px 0 0;
    padding: 0;
    color: rgb(10, 81, 57);
    text-align: center;
    font-size: 1.5em;
}

.container .card .face.face2{
    position: relative;
    background: rgb(239, 255, 245);
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 20px;
    box-sizing: border-box;
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.8);
    transform: translateY(-100px);
}

.container .card:hover .face.face2{
    transform: translateY(0);
}

.container .card .face.face2 .content p{
    margin: 0;
    padding: 0;
}

.container .card .face.face2 .content a{
    margin: 15px 0 0;
    display:  inline-block;
    text-decoration: none;
    font-weight: 900;
    color: #333;
    padding: 5px;
    border: 1px solid #333;
}

.container .card .face.face2 .content a:hover{
    background: #333;
    color: #fff;
}
@media screen and (max-width:800px){
    .container{
        flex-direction: column;
    }
}
</style>