<template>
    <div class="spacer d-flex flex-row-reverse align-center">
        <div class="spacer__image pr-2">
            <img src="~/assets/images/logo.png" class="spacer__image" alt="eden-eternal-logo">
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.spacer {
    position: relative;
    height: 150px;
}
.spacer__image {
    height: 120px;
    object-fit: cover;
    display: none;
}
@media screen and (max-width: "1364px") {
    .spacer__image {
        display: block !important;
    }
}
</style>