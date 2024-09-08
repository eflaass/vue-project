<template>
    <div class="hero">
        <div class="hero__content">
            <h1 class="hero__title">{{ title }}</h1>
            <p class="hero__subtitle">{{ subtitle }}</p>
            <DownloadButton
                :text="btn.text"
                :url="btn.url"
            ></DownloadButton>
        </div>
        <div class="hero__image-wrapper">
            <img :src="image" class="hero__image" alt="" />
        </div>
    </div>
</template>

<style lang="scss" src="./hero.scss"></style>

<script>
import DownloadButton from '../download-button/download-button.vue';

export default {
    name: 'Hero',
    components: { DownloadButton },
    data() {
        return {
            btn: {
                text: 'Download Resume',
                url: '#'
            },
            title: 'Hi, I am Johnny, Creative Technologist',
            subtitle: 'Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.',
            image: 'public/img/person-image.png'
        }
    }
}
</script>