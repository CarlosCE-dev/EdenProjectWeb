<template>
    <v-container fluid>
        <v-row no-gutters>
            <v-col cols="12" md="4" lg="3" class="d-flex flex-column">
                <HomeDownloadButton class="mb-4"/>
                <HomeLoginCard/>
            </v-col>
            <v-col cols="6" md="4" lg="6">

            </v-col>
            <v-col cols="3" md="4" lg="3">

            </v-col>
        </v-row>
    </v-container>
</template>

<script>

export default {
    head() {
        return {
            title: "Home",
        }
    },
}
</script>

<style lang="scss" scoped>

</style>
