<template>
  <div id="app">
    <header>
      <nav>
        <ul>
          <li class="nav-item">
              <img class="logo" src="./assets/build-a-bot-logo.png" />

            <!-- <router-link :to="{name: 'Home'}" class="nav-link" exact>
              <img class="logo" src="./assets/build-a-bot-logo.png" />
              Build-a-Bot
            </router-link> -->
              Build-a-Bot

          </li>
          <li class="nav-item">
            Build
            <!-- <router-link :to="{name: 'Build'}" class="nav-link" exact>Build</router-link> -->
          </li>
          <li class="nav-item cart">
            <!-- <router-link :to="{name: 'Cart'}" class="nav-link" exact>Cart</router-link>
            <div class="cart-items">{{cart.length}}</div> -->
          </li>
        </ul>
      </nav>
    </header>
    <main>
    <RobotBuilder />


    </main>
  </div>
</template>

<script>
// import HomePage from "./home/HomePage.vue";
import RobotBuilder from "./build/RobotBuilder.vue";


export default {
  name: "app",
  components: {
    // HomePage,
    RobotBuilder
  }
};
</script>

<style>
body {
  background: linear-gradient(to bottom, #555, #999);
  background-attachment: fixed;
}
</style>


<style scoped>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
}
main {
  padding: 30px;
  background-color: white;
  width: 964px;
  min-height: 300px;
}
header {
  background-color: #999;
  width: 1184px;
  margin: 0 auto;
}
ul {
  padding: 3px;
  display: flex;
}
.nav-item {
  display: inline-block;
  padding: 5px 10px;
  font-size: 22px;
  border-right: 1px solid #bbb;
}
.nav-item.cart {
  position: relative;
  margin-left: auto;
  border-right: none;
}
.logo {
  vertical-align: middle;
  height: 30px;
}

.nav-link {
  text-decoration: none;
  color: inherit;
}
.router-link-active {
  color: white;
}

.container {
  display: flex;
  margin: 10px auto 0 auto;
  justify-content: center;
}

.aside {
  padding: 30px;
  background-color: #aaa;
  width: 100px;
  min-height: 300px;
}
.cart-items {
  position: absolute;
  top: -5px;
  right: -9px;
  font-size: 18px;
  width: 20px;
  text-align: center;
  display: inline-block;
  border-radius: 100px;
  background-color: mediumseagreen;
}
</style>
