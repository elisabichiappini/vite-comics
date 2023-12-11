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
            <CardsList></CardsList>
        </div>
    </section>
    
</template>

<style lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin.scss' as *;

#dc-main-top {            
    background-color: $bg-main;

    .container {
        @include my-container-size;
        padding: 55px 0 25px;
    }
}
</style>
