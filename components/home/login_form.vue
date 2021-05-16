<template>
    <v-form ref="form" v-model="valid" lazy-validation>
        <v-text-field
            prepend-inner-icon="mdi-account" 
            dense
            label="Username" 
            required
            outlined
            background-color="white"
            >
        </v-text-field>
        <v-text-field
            prepend-inner-icon="mdi-lock" 
            dense
            label="Password"
            outlined
            background-color="white"
            required
        ></v-text-field>
        <div class="d-flex">
            <v-text-field
            dense
            class="captcha__button"
            label="Captcha"
            outlined
            background-color="white"
            required
            ></v-text-field>
            <img src="~/assets/images/captcha.jpg" class="ml-4 form__captcha" alt="eden-eternal-logo">
        </div>
        <v-btn :disabled="!valid"
            color="success"
            @click="validate"
            block>
            <v-icon left>mdi-login-variant</v-icon>
            Login
        </v-btn>
        <div class="form__spacer"></div>
        <v-btn :disabled="!valid"
            color="primary"
            block>
            <v-icon left>mdi-account-plus</v-icon>
            Register
        </v-btn>
  </v-form>
</template>

<script>
export default {
    data: () => ({
        valid: false
    }),
    methods: {
        validate() {
            
        }
    },
}
</script>

<style lang="scss" scoped>
.form__spacer {
    display: block;
    height: 40px;
}
.form__captcha {
    border-radius: 4px;
    border: 1px solid #9E9E9E;
    width: auto;
    height: 40px;
}
</style>