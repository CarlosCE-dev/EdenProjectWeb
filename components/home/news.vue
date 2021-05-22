<template>
    <v-card class="my-4">
        <v-system-bar dark color="green"  height="35" class="rounded-b-0">
            <v-spacer></v-spacer>
            <span class="white--text">{{ new Date().toDateString() }}</span>
        </v-system-bar>
        <v-card-title>
            {{ news.title }}
        </v-card-title>
        <v-card-text>
            {{ news.description }}
        </v-card-text>
    </v-card>
</template>

<script>
export default {
    props: ['news']
}
</script>

<style lang="scss" scoped>
.card__bard{
    border-bottom-left-radius: 0px !important;
    border-bottom-right-radius: 0px !important;
}
</style>