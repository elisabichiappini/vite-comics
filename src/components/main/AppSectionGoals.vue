<script>
export default {
    name: 'SectionGoals',
    data () {
        return {
            Goals: [
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
}
</script>

<template>
    <div id="dc-main-bottom">
        <div class="container">
            <ul class="list-goals">
                <li class="goal-content" v-for="li in Goals">
                    <img :src="li.src" :alt="li.alt">
                    <h3>{{ li.nome }}</h3>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
@use '../../styles/partials/typography' as *;

#dc-main-bottom {            
    background-color: $bg-primary;
    color: $color-white;

    .container {
        @include my-container-size;
        padding: 50px 0;

        .list-goals {
            @include my-flex;
            justify-content: center;
            gap: 30px;

            .goal-content {
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