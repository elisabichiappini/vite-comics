<script>
import AppPrimaryButton from '../general/AppPrimaryButton.vue';
import AppLinksSocial from './AppLinksSocial.vue';

export default {
    name: 'AppFooterBottom',
    components: {
        AppPrimaryButton,
        AppLinksSocial,
    }
};
</script>

<template> 
        <div id="footer-bottom">
            <div class="container">
                <AppPrimaryButton></AppPrimaryButton>
                <AppLinksSocial></AppLinksSocial>
            </div>
        </div>
</template>

<style scoped lang="scss">
@use '../../styles/general.scss' as *;
@use '../../styles/partials/mixin.scss' as *;
@use '../../styles/partials/variables' as *;

    #footer-bottom {
        background-color: $bg-bottom-footer ;
        .container {
            padding: 20px 0;
            @include my-flex;
            @include my-container-size;
            justify-content: space-between;
        }
    }
</style>
