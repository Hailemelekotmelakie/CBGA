<template>
  <div class="mainContainerx">
    <div @click="isDisplayed = !isDisplayed" class="menusContainerUp">
      <div class="menusContainer">
        <div class="lines"></div>
        <div class="lines"></div>
        <div class="lines"></div>
      </div>
    </div>
    <nav :class="{ displayable: isDisplayed }">
      <router-link @click="isDisplayed = !isDisplayed" to="/"> Home </router-link>
      <router-link @click="isDisplayed = !isDisplayed" to="/contact">
        Contact
      </router-link>
      <router-link @click="isDisplayed = !isDisplayed" to="/about"> About </router-link>
      <router-link @click="isDisplayed = !isDisplayed" to="/stuff">
        Board members
      </router-link>
      <router-link @click="isDisplayed = !isDisplayed" to="/donate"
        ><button class="Donate">Donate</button></router-link
      >
    </nav>
  </div>
  <router-view />
</template>

<script>
export default {
  el: "#appHeader",
  data() {
    return {
      isDisplayed: false,
    };
  },
  methods: {},
};
</script>

<style scoped>
.mainContainerx {
  z-index: 999;
  background-color: rgb(240, 247, 253);
  box-shadow: 0px 0.1px 0px 0px rgb(5, 0, 0);
  position: sticky;
  top: 0px;
}
nav {
  padding: 0px 50px;
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
}

nav a {
  font-size: 18px;
  font-weight: bold;
  color: #2c3e50;
  margin: 10px;
  text-decoration: none;
}

nav a:hover {
  color: #42b983;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.Donate {
  font-size: 18px;
  font-weight: bold;
  background-color: #47df9b;
  padding: 7px 15px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  border: 1px solid #38d996;
}
.Donate:hover {
  background-color: transparent;
  border: 1px solid #38d996;
  background-color: #a9fdd7;
}

@media screen and (max-width: 800px) {
  nav {
    z-index: 999;
    right: 200%;
    flex-direction: column;
    position: absolute;
    width: 100%;
    justify-content: center;
    transition: 0.7s;
    background-color: rgb(210, 234, 255);
    height: auto;
    padding: 40px 0px;
  }

  .menusContainerUp {
    display: flex;
    justify-content: flex-end;
  }
  .menusContainer {
    display: flex;
    flex-direction: column;
    justify-content: right;
    align-items: flex-end;
    gap: 5px;
    padding: 10px 30px;
    cursor: pointer;
    width: min-content;
  }
  .lines {
    display: flex;
    justify-content: flex-end;
    background-color: #276e57;
    /* width: 25px; */
    height: 3.5px;
    border-radius: 3px;
  }
  .lines:nth-child(even) {
    width: 30px;
  }
  .lines:nth-child(odd) {
    width: 25px;
  }
  .displayable {
    right: 0%;
  }
}
</style>
