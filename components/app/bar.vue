<template>
    <v-app-bar fixed dense flat>
        <AppMenuList class="menu-list--desktop"/>
        <vue-scroll :ops="scrollOptions" class="menu-list--tablet"> <AppMenuList/> </vue-scroll>
    </v-app-bar>
</template>

<script>
    export default {
        data: () => ({
            scrollOptions: {
                bar: {
                    keepShow: true,
                    opacity: 0.7,
                    step: 180,
                    mousedownStep: 30,
                    minSize: 0.7,
                    background: '#c1c1c1',
                    size: "7px",
                },
            }
        })
    }
</script>

<style lang="scss" scoped>
 .menu-list--tablet {
     display: none !important;
 }
 @media screen and (max-width: "1364px") {
    .menu-list--tablet {
        display: block !important;
    }
}
</style>