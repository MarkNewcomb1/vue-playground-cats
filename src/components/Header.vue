<template>
<h1 v-on:click="logCats">THIS IS THE HEADER, BRUH</h1>
</template>

<script>
export default {
    name: "Header",
    props: ['cats', 'logCats']
}
</script>

<style scoped>

</style>