<template>
  <div id="app">
    <img @click="clickDots" id="dots-gray" src="./assets/dots-gray.svg" />
    <div id="div-line"></div>
    <div id="info-container">
      <img id="avatar" src="./assets/tk-avatar.jpg" />
      <div id="admin-name">TenkeySeven</div>
    </div>
    <div id="div-line-end"></div>
    <img id="building-img" src=".\assets\investment-building.svg" />
    <div id="building-info-container">
      <div id="building-text">Building</div>
      <img id="dots-color" src="./assets/dots-color.svg" />
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "App",
  components: {
    // HelloWorld
  },
  methods: {
    clickDots: function() {
      alert("Hey you find me!");
    }
  }
};
</script>

<style>
body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #fafafa;
}

#app {
  margin-top: 10px;
}

#info-container {
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  justify-content: flex-start;
  align-items: center;
  align-content: stretch;
  text-align: center;
  margin-top: 20px;
}

#dots-gray {
  margin-left: auto;
  margin-right: 20px;
  display: block;
}

#dots-color {
  margin-left: 10px;
}

#div-line {
  margin-top: 10px;
  height: 0;
  width: 100%;
  border: 2px solid #bcaaa4;
  box-shadow: 0px 4px 4px rgba(188, 170, 164, 0.25);
}

#div-line-end {
  margin-top: 40px;
  height: 0;
  width: 100%;
  border: 2px solid #bcaaa4;
  box-shadow: 0px 4px 4px rgba(188, 170, 164, 0.25);
}

#avatar {
  width: 227px;
  height: 227px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 50%;
}

#admin-name {
  margin-top: 10px;
  font-family: Raleway;
  font-style: normal;
  font-weight: 300;
  font-size: 48px;
  line-height: 56px;
  text-align: center;

  color: #263238;
}

#building-img {
  margin-left: auto;
  margin-right: auto;
  display: block;
  width: 290px;
  height: 306px;
}

#building-info-container {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-items: center;
  align-content: stretch;
}

#building-text {
  font-family: Raleway;
  font-style: normal;
  font-weight: 600;
  font-size: 48px;
  line-height: 56px;
  text-align: center;

  color: #263238;
}
</style>
