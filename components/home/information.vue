<template>
    <v-card color="grey lighten-3" class="information">
        <img src="~/assets/images/character01.png" class="information__image" alt="character-eden">
        <v-card-title class="blue--text">Information</v-card-title>
        <v-card-text>
            <v-list-item dense class="information__list">
                <v-list-item-content>
                    <v-list-item-title class="d-flex align-center">
                        <v-icon>mdi-chevron-right</v-icon>
                        Max Level 70
                    </v-list-item-title>
                    <v-list-item-title class="d-flex align-center">
                        <v-icon>mdi-chevron-right</v-icon>
                        Exp x5
                    </v-list-item-title>
                    <v-list-item-title class="d-flex align-center">
                        <v-icon>mdi-chevron-right</v-icon>
                        Drop x5
                    </v-list-item-title>
                    <v-list-item-title class="d-flex align-center">
                        <v-icon>mdi-chevron-right</v-icon>
                        Free play
                    </v-list-item-title>
                    <v-list-item-title class="d-flex align-center">
                        <v-icon>mdi-chevron-right</v-icon>
                        And more...
                    </v-list-item-title>
                </v-list-item-content>
            </v-list-item>
        </v-card-text>
    </v-card>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.information {
    position: relative;
    overflow: hidden;
}
.information__list {
    padding: 0px !important;
}
.information__image {
    right: 5%;
    position: absolute;
    height: 95%;
}
</style>