<script>
    export default {
        name: 'PrimaryButton',
    };
</script>

<template>
    <button class="primary-button">
        Sign-up now!
    </button>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/general.scss' as *;
    .primary-button{
        padding: 10px 10px;
        border: 2px solid $bg-primary;
        color: $color-white;
        text-transform: uppercase;
        background-color: transparent;
        cursor: pointer;
    }
</style>