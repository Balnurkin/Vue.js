<script>
export default {
  data: () => {
    return {};
  },
  computed: {},
  watch: {},
  methods: {},
};
</script>

<template>
  <div class="app">
    <div class="display">
      <div class="display--action"></div>
      <div class="display--result"></div>
    </div>
    <div class="content">
      <div class="content--inner">
        <button class="number zero">C</button>
        <button class="number del">/</button>
      </div>
      <div class="content--inner">
        <button class="number style">7</button>
        <button class="number style">8</button>
        <button class="number style">9</button>
        <button class="number umnoz style">*</button>
      </div>
      <div class="content--inner">
        <button class="number style">4</button>
        <button class="number style">5</button>
        <button class="number style">6</button>
        <button class="number minus style">-</button>
      </div>
      <div class="content--inner">
        <button class="number style">1</button>
        <button class="number style">2</button>
        <button class="number style">3</button>
        <button class="number minus style">+</button>
      </div>
      <div class="content--inner">
        <button class="number tochka style">.</button>
        <button class="number style">0</button>
        <button class="number left style">{{"<="}}</button>
        <button class="number ravno style">=</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.app{
    width: 350px;
    height: 740px;
    background-color: rgb(28, 26, 26);
    border: 2px solid black;
    margin: 0 auto;
    padding-top: 145px;
    color: white;
}
.display--action{
    width: 335px;
    height: 47px;
    font-size: 30px;
    display: flex;
    align-items: flex-end;
    justify-content: end;
}
.display--result{
    margin-top: 10px;
    width: 335px;
    height: 96px;
    font-size: 50px;
    display: flex;
    align-items: flex-end;
    justify-content: end;
}
.content{
    margin-top: 20px;
    display: flex;
    flex-direction: column;
    gap: 10px;
}
.content--one{
    display: flex;
    justify-content: space-between;
}
.zero{
    width: 160px;
    height: 72px;
    background: #4E505F;
    border: none;
    border-radius: 24px;
    font-size: 32px;
    color: white;
}
.del{
    width: 160px;
    height: 72px;
    background: #4B5EFC;
    border: none;
    border-radius: 24px;
    font-size: 32px;
    color: white;
}
.content--inner{
    display: flex;
    justify-content: space-between;
}
.style{
    width: 72px;
    height: 72px;
    border-radius: 24px;
    border: none;
    color: white;
    font-size: 32px;
}
.number{
    background: #2E2F38;
}
.umnoz, .minus, .tochka, .left, .ravno{
    background: #4B5EFC;
}
</style>
