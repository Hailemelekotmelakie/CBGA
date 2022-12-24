<template>
    <div class="boardImges">
        <div class="imagesDiv1">
            <img class="images1" src="@/assets/joshua-sortino-xZqr8WtYEJ0-unsplash.jpg" alt="">
        </div>
        <div class="imagesDiv2">
            <img class="images2" src="@/assets/joshua-sortino-xZqr8WtYEJ0-unsplash.jpg" alt="">
        </div>
    </div>
</template>

<style scoped>
.boardImges{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding: 5px 50px;
    position: unset;
    height: 80vh;
}
.imagesDiv1{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    z-index: -10;
    border: 3px solid rgb(255, 158, 3);
}
.imagesDiv2{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    border: 3px solid rgb(255, 158, 3);
    z-index: -10;
}
.images1{
    width: 500px;
    height: auto;
    position: relative;
    z-index: -9;
    top: 15px;
    left: 15px;
}
.images2{
    position: relative;
    z-index: -9;
    width: 300px;
    height: auto;
    bottom: 15px;
    right: 15px;
}
@media screen and (max-width:900px){
    .boardImges{
        flex-direction: column;
    }
}
</style>