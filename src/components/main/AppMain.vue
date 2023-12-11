<script>
import AppSectionCards from './AppSectionCards.vue';
import AppSectionGoals from './AppSectionGoals.vue';

export default {
    name: 'Main',
    components: {
        AppSectionCards,
        AppSectionGoals,
    }
};
</script>

<template>
<main>
    <AppSectionCards></AppSectionCards>
    <AppSectionGoals></AppSectionGoals>
</main>
</template>