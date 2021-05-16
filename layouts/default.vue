<template>
  <v-app>

    <AppSideBar v-model="drawer"/>
    
    <AppBar @toggleDrawer="drawerController"/>

    <div class="background_image">
        <v-main class="app__content">
            <AppSpacer/>
            <v-card class="mx-md-4 mx-2 pb-4">
                <nuxt/>
            </v-card>
        </v-main>
    </div>

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

<style lang="scss" scoped>
.app__content {
    overflow-y:auto;
    height: 100%;
}
.background_image {  
    height: 100%;
    width: 100%;
    background: url('~assets/images/background.jpg');
    background-repeat:no-repeat;
    background-position: center center;
    background-size: cover;
    background-clip: border-box;
}
</style>