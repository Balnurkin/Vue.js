<script>
import Slider from './components/Slider.vue'
export default {
  components:{
    Slider,
  },
  data: () => {
    return{
      slides:[
        {title: 'Заголовок Slide One', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'},
        {title: 'Заголовок Slide Two', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'},
        {title: 'Заголовок Slide Three', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'},
        {title: 'Заголовок Slide Four', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'}
      ]
    }
  },
  computed: {},
  watch: {},
  methods: {}
}
</script>

<template>
  <div class='app'>
    <button>Previos</button>
    <Slider />
    <button>Next</button>
  </div>
</template>

<style scoped></style>
