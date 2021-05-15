<template>
  <v-app class="content">

    <AppSideBar v-model="drawer"/>
    
    <AppBar @toggleDrawer="drawerController"/>

    <v-main class="mx-md-4 mx-2 pb-4 content">
        <nuxt/>
    </v-main>

  </v-app>
</template>

<script>

export default {
    data: () => ({
        mobil: false,
        drawer: false,
    }),
    beforeMount () {
        // this.mobil = orientationType();
        // this.$store.commit('window/isMobil', this.mobil); 

        // if (this.mobil) {
        //     this.drawer = false;
        // }
    },
    methods: {
        drawerController() {
            this.drawer = !this.drawer;
        }
    },
}

</script>

<style lang="scss" scoped></style>