<template>
  <header>
    <nav>
      <div id="navigation-container">
        <img class="logo" src="../assets/logoipsum.svg" alt="" />
        <ul class="nav-bar">
          <li>home</li>
          <li>buy</li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {};
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
  padding: 12px 0;
  transition: 0.5s ease all;
  margin: 0 auto;
  width: 470px;
  height: 75px;
  z-index: 1;
  justify-content: right;
}
ul li {
  list-style-type: none;
  padding: 10px 10px;
  text-transform: uppercase;
  padding-top: 30px;
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
  padding-top: 0%;
}
</style>