<script>
import MyButtonGr from './UI/MyButtonGr.vue';
import MyButtonR from './UI/MyButtonR.vue';

export default {
  name: "BalanceForm",
  components: {
    MyButtonGr,
    MyButtonR,
  },
  props: {},
  data: () => {
    return {

    };
  },
  computed: {},
};
</script>

<template>
  <div>
    <div class="balance">
      <p>BALANCE:</p>
      
    </div>
    <div class="buttons">
      <MyButtonGr>add profit</MyButtonGr>
      <MyButtonR>add expense</MyButtonR>
    </div>
  </div>
  
</template>

<style scoped>
.balance {
  width: 250px;
  height: 150px;
}
.buttons {
  width: 200px;
  height: 150px;
}
</style>
