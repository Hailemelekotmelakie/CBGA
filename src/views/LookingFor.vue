<template>
    <div class="container">
      <div class="info">
        <h1>Looking For Consultancy</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus odit nihil ullam nesciunt quidem iste, Repellendus odit nihil</p>
        <button>Get Started</button>
      </div>
      <div class="image">
        <img src="@/assets/backgroundLookingfor.png">
      </div>
    </div>
</template>
<style scoped>


.container {
    padding: 15px 50px;
    display: flex;
    flex-direction: row;
}

 .info {
    display: flex;
    flex: 1;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 20px;
}

.info h1 {
    font-size: 40px;
    margin: 0 0 20px;
    line-height: 1.4;
    color: #5d5d5d;
}

.info p {
    margin: 0;
    line-height: 1.6;
    font-size: 15px;
    color: #000000;
}

.info button {
    border: 0;
    border-radius: 20px;
    padding: 12px 30px;
    margin-top: 30px;
    cursor: pointer;
    color: rgb(0, 0, 0);
    background-color: #38ca8d;
    font-size: 16px;
    transition: all 0.3s ease-in-out;
}

 .info button:hover {
    background-color: #1e9f65;
}

.image {
    display: flex;
    flex: 1;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.image img {
    max-width: 100%;
}


</style>