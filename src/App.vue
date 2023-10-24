<script>
import Slider from './components/Slider.vue'
export default {
  components:{
    Slider,
  },
  data: () => {
    return{
      slides:[
        {id: 1, title: 'Заголовок Slide One', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'},
        {id: 2, title: 'Заголовок Slide Two', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'},
        {id: 3, title: 'Заголовок Slide Three', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'},
        {id: 4, title: 'Заголовок Slide Four', text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'}
      ],
      slideId: 1,
    }
  },
  computed: {},
  watch: {},
  methods: {
    showNextSlide(){

    }
  }
}
</script>

<template>
  <div class='app'>
    <button>Previos</button>
    <Slider 
      v-if=""
      :key="slide.id"
      :id="slide.id"
      :title="slide.title"
      :text="slide.text" />
    <button @click="showNextSlide">Next</button>
  </div>
</template>

<style scoped></style>
