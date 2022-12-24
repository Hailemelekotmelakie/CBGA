<template>
    <div class="boardImges">
        <div class="imagesDiv1">
            <img class="images1" src="@/assets/Hailemelekot.png" alt="">
        </div>
        <div class="imagesDiv2">
            <img class="images2" src="@/assets/jonatan-pie-3l3RwQdHRHg-unsplash.jpg" alt="">
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
    position: relative;
    height: 80vh;
}
.imagesDiv1{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    position: relative;
}
.imagesDiv2{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    position: relative;
    border: 3px solid rgb(255, 158, 3);
}
.images1{
    position: relative;
    width: 500px;
    height: auto;
}
.images2{
    position: relative;
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