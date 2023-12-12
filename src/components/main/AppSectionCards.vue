<script>
import CardsList from '../CardsList.vue';
export default {
    name: 'SectionCards',
    components: {
        CardsList,
    }
};
</script>

<template>
    <section id="dc-main-top">
        <div class="container">
            <h2 class="label-section">CURRENT SERIES</h2>
            <CardsList></CardsList>
        </div>
    </section>
    
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin.scss' as *;

#dc-main-top {            
    background-color: $bg-main;
    .container {
        @include my-container-size;
        position: relative;
        .label-section {
        background-color: $bg-primary;
        color: $color-white;
        padding: 10px 20px;
        display: inline-block;
        position: absolute;
        top: -25px;
    }
    }
}
</style>
