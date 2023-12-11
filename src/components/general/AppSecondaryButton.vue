<script>
export default {
    name: 'SecondaryButton',
}
</script>

<template>
    <button class="fill-button">
        Load more
    </button>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
.fill-button {
    all: unset;
    background-color: $bg-primary;
    padding: 10px 50px;
    color: $color-white;
    @include my-uppercase;
}
</style>