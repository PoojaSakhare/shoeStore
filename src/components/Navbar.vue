<template>
  <header>
    <nav>
      <div id="navigation-container">
        <router-link to="/"
          ><img class="logo" src="../assets/logoipsum.svg" alt=""
        /></router-link>

        <ul class="nav-bar">
          <li>
            <router-link to="/Home">Home</router-link>
          </li>
          <li><router-link to="/Buy">Buy</router-link></li>
        </ul>
      </div>
    </nav>
    <!-- <router-view></router-view> -->
  </header>
</template>

<script>
export default {
  name: "Navbar",
  methods: {
    logMessage() {
      console.log("triggered");
      console.log(this.$route.name);
    },
  },
};
</script>

<style>
header {
  background-color: none;
  width: 100%;
  z-index: 99;
  position: fixed;
}
.nav-bar {
  display: flex;
  flex-direction: row;
  transition: 0.5s ease all;
  margin: 0 20px;
  width: 470px;
  height: 75px;
  z-index: 1;
  justify-content: right;
}
li {
  list-style-type: none;
  padding: 10px 10px;
  text-transform: uppercase;
  padding-right: 40px;
  text-align: center;
}
#navigation-container {
  position: relative;
  background-color: none;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.logo {
  padding-left: 40px;
}
li:hover {
  border-bottom: 5px solid black;
}
a {
  text-decoration: none;
  color: black;
}
</style>