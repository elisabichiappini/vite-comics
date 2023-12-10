<script>
export default {
    name: 'NavMenu',
    data() {
        return {
        menu: [
        {   
            nome: 'Characters',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'Comics',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'Movies',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'Tv',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'Games',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'Collectibles',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'Videos',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'Fans',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'News',
            href: '#',
            target: '_blank'
        },
        {
            nome: 'Shop',
            href: '#',
            target: '_blank'
        }
    ]}},
};
    
</script>

<template>
    <ul class="navbar">
        <li class="link" v-for="li in menu">
            <a :href="li.href" :target="li.target">{{ li.nome }}</a>
        </li>
    </ul>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/general.scss' as *;
@use '../../styles/partials/mixin' as *;
.navbar {
    display:flex;
    gap: 35px;
    @include my-uppercase;
    .link {
        list-style-type: none;
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