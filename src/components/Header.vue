<template>

<div class="header_main">
    <a href="#"><img src="../assets/img/logo.svg" alt="Логотип" class="logo_img"></a>
    <nav class="header_nav">
        <ul class="header_list">
            <li class="list_component" v-for="(name, index) in names_of_pages" :key="index"><a href="#">{{ names_of_pages[index] }}</a></li>
        </ul>
    </nav>
    <button class="consult_btn">Консультация</button>
    
</div>

</template>

<script>
    export default{
        name: 'MHeader',
        props: {
            names_of_pages: {
                type: Array
            }
        }
    }
</script>

<style lang="scss" scoped>
@import "../styles/Header.scss";
</style>