<template>
  <div id="wrapper">
    <!-- <div id="nav">
      <router-link to="/">

      </router-link>
    </div> -->
    <router-view/>
  </div>
</template>

<style lang="scss">
body {
  padding: 0;
  margin: 0;
  background-color: #ececec;
}
#nav {
  margin: 0;
  padding: 0;
  background-color: blue;
  height: 100vh;
}
button {
  background-color: #FF9241;
  border: none;
  border-radius: 4px;
  color: white;
}
</style>
