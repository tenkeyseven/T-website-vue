<template>
  <div class="Info-List-Container">
    <div class="Title">{{title}}</div>
    <div class="Info-List" v-for="item in infolist" v-bind:key="item.id">{{item.content}}</div>
    <div class="Dots-info">...</div>
  </div>
</template>

<script>
export default {
  name: "InfoBlock",
  props: ["title", "infolist"],
  data: function() {
    return {};
  }
};
</script>

<style scoped>
.Title {
  margin-top: 40px;
  margin-bottom: 10px;
  width: auto;
  height: 28px;

  font-family: Raleway;
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 28px;
  text-align: center;

  color: #4f5b62;
}

.Title::before {
  content: "#";
  margin-top: 40px;
  margin-right: 10px;
  margin-bottom: 10px;
  width: 139px;
  height: 28px;

  font-family: Raleway;
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 28px;
  text-align: center;

  color: #66bb6a;
}

.Info-List-Container {
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  justify-content: center;
  align-items: center;
  align-content: center;
}

.Info-List {
  margin-top: 10px;
  width: auto;
  height: 21px;

  font-family: Raleway;
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 21px;
  text-align: center;

  color: #4f5b62;
}

.Info-List::before {
  margin-right: 10px;
  margin-top: 10px;
  content: ">";
  width: 452px;
  height: 21px;

  font-family: Raleway;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 21px;
  text-align: center;

  color: #f9a825;
}

.Dots-info {
  font-family: Raleway;
  font-style: normal;
  font-weight: bold;
  font-size: 38px;
  line-height: 56px;
  text-align: center;

  color: #66bb6a;
}
.Dots-info::before {
  margin-right: 10px;
  content: ">";
  width: 452px;
  height: 21px;

  font-family: Raleway;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 21px;
  text-align: center;

  color: #f9a825;
}
</style>