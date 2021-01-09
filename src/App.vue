<template>
  <div id="app">
    <img @click="clickDots" id="dots-gray" src="./assets/dots-gray.svg" />
    <div id="div-line"></div>
    <div id="info-container">
      <img id="avatar" src="./assets/tk-avatar.jpg" />
      <div id="admin-name">TenkeySeven</div>
      <info-block :title="eduTitle" :infolist="eduInfoList"></info-block>
      <info-block :title="rscTitle" :infolist="rscInfoList"></info-block>
      <info-block :title="focTitle" :infolist="focInfoList"></info-block>
      <info-block :title="recTitle" :infolist="recInfoList"></info-block>
    </div>
    <!-- <div id="div-line-end"></div> -->
    <!-- <img id="building-img" src="./assets/investment-building.svg" /> -->
    <skate-meow>
    </skate-meow>
    <div id="building-info-container">
      <div id="building-text">🍓 Working</div>
      <img id="dots-color" src="./assets/dots-color.svg" />
    </div>
    <div id="footer">
      <p class="footer-text">
        TenkeySeven@2021
        <a class="footer-text" href="http://www.beian.miit.gov.cn/">京 ICP 备 17065315</a>
      </p>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import InfoBlock from "./components/InfoBlock.vue";
import SkateMeow from "./components/SkateMeow.vue";

export default {
  name: "App",
  components: {
    InfoBlock,
    SkateMeow
  },
  data: function() {
    return {
      eduTitle: "Education",
      eduInfoList: [
        {
          id: 1,
          content: "Beijing Institute of technology (Bachelor, 2016-2020)"
        },
        {
          id: 2,
          content: "Beijing Institute of technology (Master, Since 2020)"
        }
      ],

      rscTitle: "Research Interest",
      rscInfoList: [
        {
          id: 1,
          content: "Backdoor Attacks against Neural Netwoks"
        },
        {
          id: 2,
          content: "Adversarial Examples"
        }
      ],

      focTitle: "Recent Focus",
      focInfoList: [
        {
          id: 1,
          content: "⚡ Working on a novel backdoor attack"
        },
        {
          id: 2,
          content: "⚡ Paper is under construction"
        },                
      ],
      recTitle: "Things on the way",
      recInfoList:[
        {
          id: 1,
          content: "🍥 2020 年度总结 - Blog 版本"
        },
        {
          id: 2,
          content: "🍕 2020 年度总结 - Vlog 版本"
        }
      ]
    };
  },
  methods: {
    clickDots: function() {·
      alert("矩阵分析好楠阿呜呜呜呜 qaq  P-1 A P");
    }
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@300;400;500;700&display=swap');

body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #fafafa;
  margin:0 0;
  padding:0 0;
  overflow-x: hidden;
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
  font-family: 'Raleway', sans-serif;
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
  margin-bottom: 20px;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-items: center;
  align-content: stretch;
}

#building-text {
  font-family: 'Raleway', sans-serif;
  font-style: normal;
  font-weight: 300;
  font-size: 48px;
  line-height: 56px;
  text-align: center;

  color: #263238;
}

#footer {
  margin-top: 30px;
  width: auto;
  height: 409px;
  background-image: url("./assets/footer-wave.svg");
  
  display: flex;
	flex-direction: column;
	flex-wrap: nowrap;
	justify-content: flex-end;
	align-items: center;
	align-content: stretch;
}

.footer-text {
  margin-bottom: 20px;
  margin-top: auto;
  font-family: Microsoft YaHei UI;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 23px;
  text-align: center;

  color: #fafafa;
}
</style>
