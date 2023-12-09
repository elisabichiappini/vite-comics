<script>
export default {
    name: 'NavMenu',
};
</script>

<template>
    <ul class="navbar">
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
        <li>
            <a href="" target="">menu</a>
        </li>
    </ul>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;
.navbar {
    display:flex;
    gap: 35px;

    li {
        list-style-type: none;
        text-transform: uppercase;
        line-height: $size-header;
        a {
        color: $bg-bottom-footer;
        text-decoration: none;
            &:hover {
            color: $bg-primary;
            }
        }
    }
}
</style>