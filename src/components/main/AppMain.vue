<script>
export default {
    name: 'AppMain',
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
                <li class="skill-content">
                    <img src="../../../public/img/buy-comics-digital-comics.png" alt="digitalComics">
                    <h3>Digital Comics</h3>
                </li>
                <li class="skill-content">
                    <img src="../../../public/img/buy-comics-merchandise.png" alt="digitalComics">
                    <h3>Digital Comics</h3>
                </li>
                <li class="skill-content">
                    <img src="../../../public/img/buy-comics-shop-locator.png" alt="digitalComics">
                    <h3>Digital Comics</h3>
                </li>
                <li class="skill-content">
                    <img src="../../../public/img/buy-comics-subscriptions.png" alt="digitalComics">
                    <h3>Digital Comics</h3>
                </li>
                <li class="skill-content">
                    <img src="../../../public/img/buy-comics-merchandise.png" alt="digitalComics">
                    <h3>Digital Comics</h3>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped lang="scss">
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
            .skill-content{
                @include my-flex;
                justify-content: center;
                gap: 15px;
                text-transform: uppercase;

                img {
                    width: 50px;
                }
            }
        }
    
    }
}
</style>
