<script>
export default {
    data() {
        return {
            dumbotron: 'dumbo.jpeg'
        }
    },
    methods: {
        image(path) {
            return new URL(path, import.meta.url).href
        }
    }
}
</script>

<template lang="">
    <div>
        <img :src="image(`../../img/${dumbotron}`)" alt="">
    </div>
</template>

<style lang="">
    
</style>