<script>
export default {
    name: 'SocialLink',
}
</script>

<template>
    <div class="bottom-right">
        <h3>Follow Us</h3>
        <div class="social-links">
            <a href="" target="">
                <img class="img-logo" src="../../../public/img/footer-facebook.png" alt="">
            </a>
            <a href="" target="">
                <img class="img-logo" src="../../../public/img/footer-twitter.png" alt="">
            </a>
            <a href="" target="">
                <img class="img-logo" src="../../../public/img/footer-youtube.png" alt="">
            </a>
            <a href="" target="">
                <img class="img-logo" src="../../../public/img/footer-pinterest.png" alt="">
            </a>
            <a href="" target="">
                <img class="img-logo" src="../../../public/img/footer-periscope.png" alt="">
            </a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixin' as *;
.bottom-right {
    @include my-flex;
    gap: 20px;
    color: $bg-primary;
    .social-links {
        display: flex;
        gap: 15px;
        .img-logo {
            width: 35px;
            display: block;
            padding: 5px;
        }
    }
}

</style>