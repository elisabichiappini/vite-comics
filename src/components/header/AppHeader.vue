<script>
import AppLogo from '../general/AppLogo.vue';
import AppTopMenu from './AppTopMenu.vue';
export default {
    name: 'AppHeader',
    components: {
        AppLogo,
        AppTopMenu,
    }
}
</script>

<template>
    <header>
        <AppLogo></AppLogo>
        <AppTopMenu></AppTopMenu>
    </header>
</template>

<style lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/general.scss' as *;
@use '../../styles/partials/mixin' as *;

    header {
        @include my-container-size;
        @include my-flex;
        justify-content: space-between;
        height: $size-header;
    }
</style>
