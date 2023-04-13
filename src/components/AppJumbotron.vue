<script>
export default {
    name: "AppJumbotron",
    data() {
        return {
            img: {
                id: "img01.jpg",
                description: "Un paesaggio di montagna",
            },
        }
    },
    methods: {
        getImgPath(name) {
            console.log(new URL(`../assets/img/${name.id}`, import.meta.url).href);
            return new URL(`../assets/img/${name.id}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <img class="jumbotron" :src="`src/assets/img/${img.id}`" :alt="`${img.description}`">
    <img class="jumbotron" :src="getImgPath(img)" :alt="`${img.description}`">
</template>


<style>
img.jumbotron {
    margin-top: 1rem;
    object-fit: cover;
    width: 100%;
    height: 300px;
}
</style>