<template>
    <HeaderComp />
    <router-view />
</template>

<script>
import HeaderComp from '@/components/HeaderComp'

export default {
    components: {
        HeaderComp,
    }
}
</script>

<style>
@import 'C:/vue/web_shishki/src/templates/login.css';
@import 'C:/vue/web_shishki/src/templates/main_page.css';
@import 'C:/vue/web_shishki/src/templates/reg.css';
</style>