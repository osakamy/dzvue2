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
                <p class="footer__social--templates-showcase">Showcase</p>
                <p class="footer__social--templates-landing_one">Landing one</p>
                <p class="footer__social--templates-sing_up">Sign up</p>
                <p class="footer__social--templates-other_templates">Other templates</p>
            </div>
            <div class="footer__social--img">
                <img class="footer__social--img_inst" src="../assets/instagram.svg" alt="">
                <img class="footer__social--img_twiter" src="../assets/twiter.svg" alt="">
                <img class="footer__social--img_facebook" src="../assets/facebook.svg" alt="">
            </div>
        </div>
        <div class="footer__contact">
            <div class="footer__contact--list">
                <p>Powered by</p>
                <p>webflow</p>
                <p>Designed by</p>
                <p class="footer__contact--list__name">Veljko</p>
            </div>
            <p class="footer__contact--name">Contact</p>
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

            &:hover {
                cursor: pointer;
            }
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

            &-showcase:hover {
                color: #645b5b;
                transition: 0.3s;
                cursor: pointer;
            }

            &-landing_one:hover {
                color: #645b5b;
                transition: 0.3s;
                cursor: pointer;
            }

            &-sing_up:hover {
                color: #645b5b;
                transition: 0.3s;
                cursor: pointer;
            }

            &-other_templates:hover {
                color: #645b5b;
                transition: 0.3s;
                cursor: pointer;
            }
        }

        &--img {
            display: flex;
            gap: 8px;

            &_inst:hover {
                cursor: pointer;
            }

            &_twiter:hover {
                cursor: pointer;
            }

            &_facebook:hover {
                cursor: pointer;
            }
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

        &--name:hover {
            color: #645b5b;
            transition: 0.3s;
            cursor: pointer;
        }
    }
}
</style>
