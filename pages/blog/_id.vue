<template>
    <div>
        <h1>This id is {{ $route.params.id }}</h1>
        <h1>{{ post.title }}</h1>
        <p>{{ post.body }}</p>
    </div>
</template>

<script>
export default {
    asyncData({ $axios, route }) {
        return $axios.get(`https://jsonplaceholder.typicode.com/posts/${route.params.id}`)
        .then(res => {
            return {
                post: res.data
            }
        })
    },
    layout: 'blog'
}
</script>


<style scoped>

</style>