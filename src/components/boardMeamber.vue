<template>
    <div class="boardImges">
        <div class="imagesDiv1">
            <div class="memberName">MR. Aboneh Teshome</div>
            <div class="memberHoner">Head Director</div>
            <img class="images1" src="@/assets/pngtree-male-avatar-vector-icon-png-image_691595.jpg" alt="">
        </div>
        <div class="imagesDiv2">
        <div class="memberName">MR. Abrham</div>
            <div class="memberHoner">Head Director</div>
            <img class="images2" src="@/assets/businessman-icon-image-male-avatar-profile-vector-glasses-beard-hairstyle-179728610.jpg" alt="">
        </div>
    </div>
</template>

<style scoped>
.boardImges{
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    padding: 5px 50px;
    height: auto;
    padding-bottom: 250px;
}
.imagesDiv1{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    z-index: -10;
    margin: 30px;
    gap: 5px;
}
.imagesDiv2{
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
    align-items: center;
    bottom: -205px;
    gap: 5px;
    z-index: -1;
}
.images1{
    width: 300px;
    height: 300px;
    overflow: hidden;
    position: relative;
    z-index: -9;
    border-radius: 50%;
    border: 3px solid rgb(255, 158, 3);
}
.images2{
    z-index: -9;
    width: 300px;
    height: 300px;
    overflow: hidden;
    z-index: -9;
    border-radius: 50%;
    border: 3px solid rgb(255, 158, 3);
}
.memberName{
    border-bottom: 1px solid rgb(17, 169, 114);
    font-size: 20px;
    font-weight: bold;
    font-family:  Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}
.memberHoner{
    font-size: 15px;
    font-weight: bold;
    font-family: monospace;
    padding: 10px;
    background: rgb(0,212,255); 
background: linear-gradient(90deg, rgba(0,212,255,1) 8%, rgb(15, 123, 139) 50%, rgba(0,212,255,1) 100%);
}
@media screen and (max-width:900px){
    .boardImges{
        flex-direction: column;
        padding: 5px;
    }
    .images2, .images1{
        z-index: -9;
        width: 220px;
        height: 220px;
    }
    .imagesDiv2{
        position: unset;
        align-items: center;
        bottom: 0px;
    }
}
</style>