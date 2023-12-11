<script>
import AppFooterMenu from './AppFooterMenu.vue';

export default {
    name: 'FooterTop',
    components: {
        AppFooterMenu,
    }
};
</script>

<template>
<div id="footer-top">
    <div class="container">
        <AppFooterMenu></AppFooterMenu>
        <img class="logo-bg" src="../../../public/img/dc-logo-bg.png" alt="dc-logo-bg">
    </div>
</div>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
@use '../../styles/general.scss' as *;

#footer-top {
    background-image: url('../../../public/img/footer-bg.jpg');
    background-size: cover;
    .container{
        @include my-container-size;
        @include my-flex;
        justify-content: space-between;
        overflow: hidden;
        .logo-bg {
            width: 600px;
            max-height: 400px;
            object-fit: cover;
        }
    }
}
</style>