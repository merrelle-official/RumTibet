<template>

<div class="body">
  <img src="./assets/img/hear_background_img.png" alt="Задний фон горы" class="hear_background_img">
  <div class="main">
    <Header class="header" :names_of_pages="names_of_pages"></Header>
  </div>
</div>

</template>

<script>
import Header from "./components/Header.vue"


export default {
  name: 'App',
  components: {
    Header,
  },
  data() {
    return {
      names_of_pages: ['Главная', 'Про гида', 'Программа тура', 'Стоимость', 'Блог', 'Контакты'],
    }
  }
}
</script>

<style lang="scss">
@import './styles/App.scss';
</style>
