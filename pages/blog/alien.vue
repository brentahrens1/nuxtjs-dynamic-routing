<template>
    <div>
        <h2>This is the nested route</h2>
        <nuxt-link to="/blog">Back to the blog page</nuxt-link>
    </div>
</template>

<script>
export default {
    validate() {
        return false
    }
}
</script>

<style scoped>

</style>