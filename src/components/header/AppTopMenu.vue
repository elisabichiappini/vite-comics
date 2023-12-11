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

    <ul class="list-links">
        <li class="link" v-for="li in menu">
            <a :href="li.href" :target="li.target">{{ li.nome }}</a>
        </li>
    </ul>
</template>

<style scoped lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
@use '../../styles/partials/typography' as *;
.list-links {
    display:flex;
    gap: 35px;
    @include my-uppercase;
    .link {
        list-style-type: none;
        line-height: $size-header;
        border-bottom: 2px solid transparent;
        
        &:hover {
                color: $bg-primary;
                border-bottom: 2px solid $bg-primary;
        }

        a {
            all: unset;
            font-weight: 600;
            text-decoration: none;
        }
    }
}
</style>