<template>
    <div class="d-flex justify-center appbar__buttons align-center menu-list--height">
        <v-btn small text plain color="red" class="mx-md-4">Home</v-btn>
        <v-btn small text plain color="red" class="mx-md-4">Download</v-btn>
        <v-btn small text plain color="red" class="mx-md-4">Social Network</v-btn>
        <v-btn small text plain color="red" class="mx-md-4">Register</v-btn>
        <div class="appbar__image mx-md-4">
            <img src="~/assets/images/logo.png" class="appbar__logo" alt="eden-eternal-logo">
        </div>
        <v-btn small text plain color="red" class="mx-md-4">Home to play</v-btn>
        <v-btn small text plain color="red" class="mx-md-4">Rules</v-btn>
        <v-btn small text plain color="red" class="mx-md-4">Ranking</v-btn>
        <v-btn small text plain color="red" class="mx-md-4">Language</v-btn>
    </div>
</template>

<style lang="scss" scoped>
.appbar__buttons {
    width: 100%;
    height: 100%;
    position: absolute;
    text-overflow: ellipsis;
}
.appbar__image {
    top: -10px;
    position: relative;
    width: 150px;
}
.appbar__logo {
    position: absolute;
    width: 150px;
}
.__view {
    display: flex;
    align-items: center;
}

.menu-list--desktop {
    display: block;
}
.menu-list--tablet {
    display: none !important;
}

@media screen and (max-width: "1364px") {
    .appbar__image {
        display: none;
    }
    .menu-list--desktop {
        display: none !important;
    }
}
</style>