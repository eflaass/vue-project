<template>
    <div class="header">
        <a
            v-for="link in links"
            :key="link.name"
            :href="link.url"
            class="header__item">
            {{ link.name }}
        </a>
    </div>
</template>

<style lang="scss" src="./header.scss"></style>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: [
                {
                    name: 'Works',
                    url: '#',
                },
                {
                    name: 'Blog',
                    url: '#',
                },
                {
                    name: 'Contact',
                    url: '#',
                },
            ]
        }
    }
}
</script>