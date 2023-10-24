<script>
import axios from "axios";
export default {
  data: () => {
    return {
      info: null,
    };
  },
  computed: {},
  watch: {
  },
  methods: {
    
  },
  mounted() {
    axios.get("https://api.coindesk.com/v1/bpi/currentprice.json")
      .then((response) => {
        this.info = response.data.bpi
        console.log(this.info);
      });
  },
};
</script>

<template>
  <div id="app">
    <div class='app--inner' v-for="item, index in info" :key="index">
      <h1>Bitcoin Price Index</h1>
      <p>Code: <span>{{item?.code}}</span></p>
      <p>Description: <span>{{item?.description}}</span></p>
      <p>Rate: <span>{{item?.rate}}</span></p>
    </div>
  </div>
</template>

<style scoped>
#app{
  width: 1000px;
  margin: 0 auto;
  display: flex;
  gap: 50px;
}
.app--inner{
  width: 300px;
  border:1px solid black;
  text-align: center;
}
</style>
