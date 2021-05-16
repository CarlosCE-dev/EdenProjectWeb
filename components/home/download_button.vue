<template>
    <v-hover v-slot="{ hover }">
        <v-card :elevation="hover ? 10 : 2"
            class="d-flex align-center justify-center flex-column light-blue white--text download_button pa-4 font-weight-bold">
            <div class="d-flex align-center justify-center download_button__title amber--text">
                <v-icon color="amber" class="mr-2" large>mdi-download</v-icon>
                Download
            </div>
            <span>Download the full client and join us!</span>
        </v-card>
    </v-hover>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.download_button {
    border-radius: 2px;
    transition: box-shadow .2s ease;
    cursor: pointer;
}

.download_button__title {
    font-size: 30px;
}
</style>