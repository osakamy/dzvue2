<script setup>

</script>

<template>
<section class="footer">
    <div class="container footer__container">
        <div class="footer__title">
            <img src="../assets/logo.svg" alt="">
            <button class="footer__title--btn">Get on Webflow</button>
        </div>
        <div class="footer__social">
            <div class="footer__social--templates">
                <p>Showcase</p>
                <p>Landing one</p>
                <p>Sign up</p>
                <p>Other templates</p>
            </div>
            <div class="footer__social--img">
                <img src="../assets/instagram.svg" alt="">
                <img src="../assets/twiter.svg" alt="">
                <img src="../assets/facebook.svg" alt="">
            </div>
        </div>
        <div class="footer__contact">
            <div class="footer__contact--list">
                <p>Powered by</p>
                <p>webflow</p>
                <p>Designed by</p>
                <p class="footer__contact--list__name">Veljko</p>
            </div>
            <p>Contact</p>
        </div>
    </div>
</section>
</template>

<style scoped lang="scss">
.footer {
    background: black;
    padding-top: 64px;

    &__title {
        display: flex;
        justify-content: space-between;
        padding-bottom: 64px;

        &--btn {
            color: black;
            background: white;
            padding: 12px 32px;
            border-radius: 6px;
            border-color: white;
            font-weight: 700;
        }
    }

    &__social {
        display: flex;
        justify-content: space-between;
        color: white;
        align-items: center;
        padding-bottom: 28px;

        &--templates {
            display: flex;
            gap: 16px;
        }

        &--img {
            display: flex;
            gap: 8px;
        }
    }

    &__contact {
        display: flex;
        justify-content: space-between;
        color: white;
        border-top: 1px solid rgb(48, 48, 48);
        padding-top: 29px;

        &--list {
            display: flex;
            gap: 12px;

            &__name {
                color: #FF7143;
            }
        }
    }
}
</style>
