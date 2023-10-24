<script>
import Column from './components/Column.vue'
export default {
  components:{
    Column,
  },
  data: () => {
    return{
      columns: 3,

    }
  },
  computed: {},
  watch: {},
  methods: {}
}
</script>

<template>
<div class="app">
  <Column v-for="col, index in columns" :key="index">

  </Column>
</div>
  
</template>

<style scoped>
.app{
  display: flex;
  gap: 100px;
}
</style>
