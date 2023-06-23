<script setup>
    import LogoIcon from './icons/IconLogo.vue'
    import LogInIcon from './icons/IconLogIn.vue'
</script>

<template>
    <div class="container">
        <div class="icon-logo">
            <LogoIcon />
        </div>
        <h1 class="logo">
            Лого
        </h1>
        <button class="btn-login">
            <LogInIcon />
        </button>
    </div>
</template>

<style scoped>
    .container {
        margin: 0 auto;
        max-width: 1600px;
        display: flex;
        place-items: center;
    }

    .icon-logo{
        margin: 1rem 1.2rem 1rem 0;
    }

    .logo {
        margin: 0;
        padding: 0;
        display: flex;
        place-items: center;
        flex: 1;
    }

    .btn-login {
        cursor: pointer;
        border: none;
        background-color: white;
    }
</style>