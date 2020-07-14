<template>
    <div>
        <div class="blog">
            <div class="blog-inner">
                <nuxt />
            </div>
            <div class="blog-sidebar">

            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    .blog {
        display: flex;
    }

    .blog-inner {
        flex: 8;
    }
    
    .blog-sidebar {
        flex: 4;
        height: 100vh; 
        background: pink;
    }
</style>