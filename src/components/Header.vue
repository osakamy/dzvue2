<script setup>

</script>

<template>
    <section class="header">
        <div class="container hero__container">
            <div class="header__logo">
                <img src="../assets/logo.svg" alt="">
                <p class="header__email">mail@blanko.com</p>
            </div>
            <div class="header__info">
                <nav class="header__naviagtion">
                    <a href="#landing__section" class="header__naviagtion--landing">Landing</a>
                    <p class="header__naviagtion--all-pages">All pages</p>
                    <a href="#hero__section" class="header__naviagtion--template">Template</a>
                </nav>
                <button class="header__btn">Purchase template</button>
            </div>
            
        </div>
    </section>
</template>

<style scoped lang="scss">
    .header {
        background-color: black;
        padding: 16px 0px 16px 0px;
        align-items: center;
        margin: 0 auto;

        &__logo {
        display: flex;
        gap: 65px;
    }

        &__email {
            background-color: rgb(39, 39, 39);
            color: white;
            border: 2px solid rgb(39, 39, 39);
            padding: 4px 8px;

            &:hover {
                color: #645b5b;
                transition: 0.3s;
                cursor: pointer;
            }
        }

        &__info {
            display: flex;
            gap: 65px;
        }

        &__naviagtion {
            display: flex;
            color: white;
            gap: 20px;
            align-items: center;
            
            a {
                color: white;
                text-decoration: none;
                
                &:hover {
                    color: #645b5b;
                    transition: 0.3s;
                    cursor: pointer;
                }
            }

            &--all-pages:hover {
                color: #645b5b;
                transition: 0.3s;
                cursor: pointer;
            }

            &--template:hover {
                color: #645b5b;
                transition: 0.3s;
                cursor: pointer;
            }
        }

        &__btn {
            color: black;
            background: #FF7143;
            border-color: #FF7143;
            border-radius: 6px;
            padding: 12px 32px;
            font-weight: bold;
        }
    }

    .hero__container {
        max-width: 90rem;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 272px;
    }
</style>
