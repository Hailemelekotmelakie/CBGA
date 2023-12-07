<template>
  <div class="FooterBelow">
    <div class="FooterBelowLeft">
      <div class="phoneNumber">
        <a href="tel:+251912-442502"
          ><fa icon="fa-solid fa-phone" />&nbsp;&nbsp; +251 912-442502
        </a>
      </div>
      <div class="emailAdress">
        <a href="mailto:cbgaethiopia@gmail.com">
          <fa icon="fa-solid fa-envelope" /> &nbsp;&nbsp; cbgaethiopia@gmail.com
        </a>
      </div>
      <div class="copywrite">
        © Copyright 2022 Center for Budgetary Governance Advocacy. All Rights Reserved.
      </div>
    </div>
    <div class="FooterBelowRight">
      <fa class="FooterBelowRightfa" :icon="['fab', 'telegram']" />
      <fa class="FooterBelowRightfa" :icon="['fab', 'facebook']" />
      <fa class="FooterBelowRightfa" :icon="['fab', 'youtube']" />
      <fa class="FooterBelowRightfa" :icon="['fab', 'instagram']" />
      <fa class="FooterBelowRightfa" icon="fa-brands fa-twitter" />
      <fa class="FooterBelowRightfa" icon="fa-solid fa-envelope" />
    </div>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style scoped>
.FooterBelow {
  color: aliceblue;
  background-color: rgb(0 64 43);
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  padding: 30px 50px;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}
.FooterBelowLeft {
  display: flex;
  flex-direction: column;
  gap: 10px;
  font-size: 15px;
}
.FooterBelowRight {
  color: rgba(255, 255, 255, 0.632);
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  gap: 25px;
}
.FooterBelowRightfa {
  font-size: 25px;
  cursor: pointer;
  transition: all 0.5s ease-in-out;
}
.FooterBelowRightfa:hover {
  color: rgb(255, 255, 255);
}
.copywrite {
  padding: 20px 0;
}
.phoneNumber,
.emailAdress {
  color: aliceblue;
  font-style: italic;
}
.phoneNumber a,
.emailAdress a {
  color: rgb(159, 159, 253);
  text-decoration: none;
  font-family: sans-serif;
}
@media screen and (max-width: 800px) {
  .FooterBelow {
    flex-direction: column;
    padding: 20px 5px;
    align-items: center;
    justify-content: center;
  }
  .FooterBelowLeft,
  .FooterBelowRight {
    justify-content: center;
    align-items: center;
  }
  .FooterBelowRightfa {
    font-size: 20px;
  }
  .copywrite {
    padding: 10px;
    text-align: center;
    font-size: 12px;
    font-weight: 500;
    line-height: 1.4rem;
  }
}
</style>
