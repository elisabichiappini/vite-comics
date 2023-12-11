<script>
export default {
    props: ['image', 'title']
};
</script>

<template>
    <div class="card">
        <img 
        :src="image" 
        :alt="title">
        <h4>{{ title }}</h4>
    </div>
</template>

<style lang="scss" scoped>

.card {
    img {
        width: 100%;
        display: block;
        height: 200px;
        object-fit: cover;
        margin-bottom: 10px;
    }
    h4{
        text-align: start;
    }
}
</style>