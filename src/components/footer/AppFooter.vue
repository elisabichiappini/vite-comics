<script>
import AppFooterTop from './AppFooterTop.vue';
import AppFooterBottom from './AppFooterBottom.vue';

export default {
    name: 'Footer',
    components: {
        AppFooterTop,
        AppFooterBottom,
    }
};
</script>

<template>
    <footer>
        <AppFooterTop></AppFooterTop>
        <AppFooterBottom></AppFooterBottom>
    </footer>
</template>
