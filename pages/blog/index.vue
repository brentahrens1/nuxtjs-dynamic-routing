<template>
    <div>
        <h2>This is the blog</h2>
        <nuxt-link to="/blog/alien">Visit the child page</nuxt-link>
        <hr>
        <ul>
            <li v-for="post in posts" :key="post.id">
                <nuxt-link :to="`/blog/${post.id}`">{{ post.title }}</nuxt-link>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    asyncData({ $axios }) {
        return $axios.get('https://jsonplaceholder.typicode.com/posts')
        .then(res => {
            return {
                posts: res.data
            }
        })
    },
    data() {

    }
}
</script>

<style scoped>

</style>