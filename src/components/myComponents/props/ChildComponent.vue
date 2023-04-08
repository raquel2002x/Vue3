<script>

export default {
    props: {
        movieTitle: String,
    },
    data() {
        return {
        brandChild: 'DC Comics',
        }
    },
    methods:{
        sendBrand(){
        this.$emit('brand', this.brandChild)
        }
    }
}
</script>

<template>
    <h2>Hija {{ movieTitle }}</h2>
    <button @click="sendBrand">sendBrand</button>
</template>

<style></style>