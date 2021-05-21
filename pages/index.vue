<template>
    <v-container fluid>
        <v-row no-gutters>
            <v-col cols="12" md="4" lg="3">
                <HomeDownloadButton class="mb-4"/>
                <HomeLoginCard/>
            </v-col>
            <v-col cols="12" md="4" lg="7">
                <div class="mx-md-8">
                    <HomeTips class="mt-4 mt-md-0"/>
                    <HomeNewsList class="py-4"/>
                </div>
            </v-col>
            <v-col cols="12" md="4" lg="2">
                <HomeInformation/>
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
