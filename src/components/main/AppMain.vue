<script>
export default {
    name: 'AppMain',
    data () {
        return {
            listQualities: [
                {
                    nome: 'Digital comics',
                    src: '../../../public/img/buy-comics-digital-comics.png',
                    alt: 'digital-comics-image'
                },
                {
                    nome: 'Dc merchandise',
                    src: '../../../public/img/buy-comics-merchandise.png',
                    alt: 'comics-merchandise'
                },
                {
                    nome: 'Subscription',
                    src: '../../../public/img/buy-comics-subscriptions.png',
                    alt: 'comics-subscriptions'
                },
                {
                    nome: 'Comics shop locator',
                    src: '../../../public/img/buy-comics-shop-locator.png',
                    alt: 'shop-locator'
                },
                {
                    nome: 'Dc power visa',
                    src: '../../../public/img/buy-dc-power-visa.svg',
                    alt: 'power-visa'
                },
            ]
        }
    }
};
</script>

<template>
    <main id="main-top">
        <div class="container">
            <div class="content-string">
                <span>Content goes here...</span>
            </div>
        </div>
    </main>
    <div id="main-bottom">
        <div class="container">
            <ul class="list-skills">
                <li class="skill-content" v-for="li in listQualities">
                    <img :src="li.src" :alt="li.alt">
                    <h3>{{ li.nome }}</h3>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss">
@use '../../styles/partials/variables' as *;
@use '../../styles/general.scss' as *;
@use '../../styles/partials/mixin.scss' as *;

#main-top {            
    background-color: $bg-main;

    .container {
        @include my-container-size;

        .content-string {
            color: $color-white;
            padding: 50px 0;
        }
    }
}

#main-bottom {            
    background-color: $bg-primary;
    color: $color-white;

    .container {
        @include my-container-size;
        padding: 50px 0;

        .list-skills {
            @include my-flex;
            justify-content: center;
            gap: 30px;

            .skill-content {
                @include my-flex;
                @include my-uppercase;
                justify-content: center;
                gap: 15px;

                img {
                    width: 50px;
                }
            }
        }
    }
}
</style>
