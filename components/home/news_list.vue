<template>
    <div>
        <p class="mb-0">
            <span class="blue--text title__news pr-1">News</span>EdenEternal.To
        </p>
        <v-divider class="pb-4"></v-divider> 
        <div v-for="item in news" :key="item">
            <HomeNews/>
        </div>
    </div>
</template>

<script>
export default {
    data: () => ({
        news: ['1','2']
    })
}
</script>

<style lang="scss" scoped>
.title__news {
    font-size: 2rem;
}
</style>