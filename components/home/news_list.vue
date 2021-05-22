<template>
    <div>
        <p class="mb-0">
            <span class="blue--text title__news pr-1">News</span>EdenEternal.To
        </p>
        <v-divider class="pb-4"></v-divider> 
        <div v-for="item in news">
            <HomeNews :news="item"/>
        </div>
    </div>
</template>

<script>
export default {
    data: () => ({
        news: [
            {
                title: "Next big patch soon",
                description: "Soon!"
            }
        ]
    })
}
</script>

<style lang="scss" scoped>
.title__news {
    font-size: 2rem;
}
</style>