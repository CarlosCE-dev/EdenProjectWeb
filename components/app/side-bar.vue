a<template>
    <v-navigation-drawer color="purple-light" dark left app temporary stateless v-model="drawer">

        <div class="d-flex align-center flex-row-reverse pa-2">
            <v-btn icon @click="drawer = false">
                <v-icon>mdi-close</v-icon>
            </v-btn>
        </div>

        <v-list nav dense>
            <v-list-item :to="item.route" v-for="(item, index) in items" :key="index">
                <v-list-item-icon>
                    <v-icon>{{item.icon}}</v-icon>
                </v-list-item-icon>
                <v-list-item-title>{{item.name}}</v-list-item-title>
            </v-list-item>
        </v-list>

        <template v-slot:append>
           <v-list nav dense>
                <v-list-item link>
                    <v-list-item-icon>
                        <v-icon>mdi-login-variant</v-icon>
                    </v-list-item-icon>
                    <v-list-item-title>Log out</v-list-item-title>
                </v-list-item>
            </v-list>
        </template>
    </v-navigation-drawer>
</template>

<script>
export default {
    props: ['value'],
    data: () => ({
        items: [
            { name: 'Home', route: "/", icon: 'mdi-home' },
            { name: 'Download',  route: "/admin", icon: 'mdi-shield-key' }, 
            { name: 'Social Network',  route: "/admin", icon: 'mdi-shield-key' }, 
            { name: 'Register',  route: "/admin", icon: 'mdi-shield-key' },
            { name: 'Home to play',  route: "/admin", icon: 'mdi-shield-key' },
            { name: 'Rules',  route: "/admin", icon: 'mdi-shield-key' },
            { name: 'Ranking',  route: "/admin", icon: 'mdi-shield-key' },
            { name: 'Language',  route: "/admin", icon: 'mdi-shield-key' },
        ],
    }),
    computed: {
        drawer: {
            get () {
                return this.value;
            },
            set (value) {
                this.$emit('input', value)
            }
        }
    }, 
}
</script>

<style lang="scss" scoped>
h1{ 
    color: $deep;
}

.navigation__profile{
    padding-left: 8px !important;
    padding-right: 8px !important;
}
</style>