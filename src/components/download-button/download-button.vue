<template>
    <a :href="url" class="download-button">{{ text }}</a>
</template>

<style lang="scss" src="./download-button.scss"></style>

<script>
export default {
    name: 'DownloadButton',
    props: {
        text: {
            type: String,
            default: 'Download'
        },
        url: {
            type: String,
            default: '#'
        }
    },
}
</script>