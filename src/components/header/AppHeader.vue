<script>
import AppLogo from '../general/AppLogo.vue';
import AppTopMenu from './AppTopMenu.vue';
import AppJumbotron from './AppJumbotron.vue';

export default {
    name: 'AppHeader',
    components: {
        AppLogo,
        AppTopMenu,
        AppJumbotron,
    }
};
</script>

<template>
    <header>
        <div id="dc-navbar">
            <AppLogo></AppLogo>
            <AppTopMenu></AppTopMenu>
        </div>
        <AppJumbotron></AppJumbotron>
    </header>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;

    #dc-navbar {
        @include my-container-size;
        @include my-flex;
        justify-content: space-between;
        height: $size-header;
    }
</style>
