<template>
    <div class="app">
        <Header></Header>
        <Hero></Hero>
    </div>
</template>

<style lang="scss" src="./app.scss"></style>

<script>
import Header from '../header/header.vue';
import Hero from '../hero/hero.vue';

export default {
    name: 'App',
    components: { Header, Hero },
    data() {
        return {}
    }
}
</script>