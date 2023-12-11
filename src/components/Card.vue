<script>
export default {
    props: ['image', 'title']
};
</script>

<template>
    <div class="card">
        <img :src="image" 
        :alt="title">
        <h4>{{ title }}</h4>
    </div>
</template>

<style></style>