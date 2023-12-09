<script>
import AppLogo from './AppLogo.vue';
import AppTopMenuVue from './AppTopMenu.vue';
export default {
    name: 'AppHeader',
    components: {
        AppLogo,
        AppTopMenuVue,
    }
}
</script>

<template>
    <header>
        <AppLogo></AppLogo>
        <AppTopMenuVue></AppTopMenuVue>
    </header>
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

    header {
        max-width: 1300px;
        margin: 0 auto;
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 120px;
    }
</style>
