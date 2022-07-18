<template>
  <div class="header">
    <div class="header-outer">
      <img src="../assets/logo.png" class="main-logo" />
      <img src="../assets/menu.png" class="menu-logo" @click="loadMenu()" />
    </div>
    <div v-if="isLoaded" class="menu-container">
      <div v-for="menu in menuItems" :key="menu" class="menu-items">
        {{ menu }}
      </div>
    </div>
    <button class="login-btn">LOGIN/REGISTER</button>
    <button class="news-btn">News Letter Signup</button>
    <div class="media-btns">
      <div v-for="img in mediaLogos" :key="img">
        <img :src="img" class="media-buttons" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menuItems: [
        "ABOUT US",
        "GALLERY",
        "M2 SERVICES",
        "NEWS",
        "FAQ",
        "BLOG",
        "CONTACT US",
      ],
      isLoaded: false,
      mediaLogos: [
        "../assets/header-twitter.png",
        "src/assets/header-instagram.png",
        "src/assets/googleheader.png",
        "src/assets/header-facebook.png",
      ],
    };
  },
  methods: {
    loadMenu() {
      this.isLoaded = this.isLoaded ? false : true;
    },
  },
};
</script>

<style scoped>
.media-btns {
  display: flex;
  flex-direction: row;
  margin-top: 5px;
  justify-content: space-evenly;
}
.media-buttons {
  background: #032149;
  margin-right: 20px;
  width: 37px;
  height: 40px;
}
.header {
  display: flex;
  flex-direction: column;
}
.header-outer {
  padding-top: 20px 0px 20px 0px;
  padding: 40px;
  display: flex;
  justify-content: space-between;
}
.menu-logo {
  width: 50px;
  height: 50px;
  margin-top: 20px;
}
.menu-items {
  color: #363a47;
  padding: 15px 20px;
  font-family: lato;
  font-weight: bold;
}
.login-btn {
  font-weight: bold;
  color: #032149;
  padding: 10px 90px;
  align-self: center;
  border: 2px #021631 solid;
  border-radius: 5px;
  background-color: white;
}
.menu-items {
  display: block;
}
.news-btn {
  font-weight: bold;
  background-color: #032149;
  color: white;
  align-self: center;
  padding: 20px 70px;
  padding-left: 85px;
  padding-right: 85px;
  margin-top: 20px;
}

@media screen and (min-width: 1100px) {
  .main-logo {
    width: 150px;
    height: 97px;
  }
  .menu-logo {
    display: none;
  }
  .menu-items {
    display: block;
    width: max-content;
  }
  .header {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
  }
  .menu-container {
    display: flex;
    flex-direction: row;
  }
  .news-btn {
    padding: 20px 30px;
    width: fit-content;
    margin: 15px;
    height: 40px;
    margin-top: 15px;
    border: 0px;
    padding-top: 10px;
  }
  .login-btn {
    padding: 10px 45px;
    width: fit-content;
    margin: 15px;
  }
}
</style>
