<script>
    export default {
        name: 'ListMenuFooter',
    };
</script>

<template>
    <ul class="menu-footer-nav"> 
        <strong>DC COMICS</strong>
        <li>
            <a href="" target="" class="footer-nav">Character</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Comics</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Movies</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">TV</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Character</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Comics</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Movies</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">TV</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Character</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Comics</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Movies</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">TV</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Character</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Comics</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Movies</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">TV</a>
        </li> <li>
            <a href="" target="" class="footer-nav">Character</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Comics</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">Movies</a>
        </li>
        <li>
            <a href="" target="" class="footer-nav">TV</a>
        </li>
    </ul>
</template>

<style scoped lang="scss">
@use '../../styles/general.scss' as *;
@use '../../styles/partials/variables' as *;

    .menu-footer-nav {
        display: flex;
        flex-direction: column;
        color: $color-white;
        height: 500px;
        padding: 80px 0;
        gap: 10px 40px;
        flex-wrap: wrap;
        flex-grow: 1;
        align-content: start;
        li {
            font-size: 10px;
            .footer-nav {
                color: $color-white;
            }
        }
    }
</style>