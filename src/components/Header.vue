<script setup>
import { ref } from 'vue';

const isActive = ref(false);
function activeBurger(){
    isActive.value = !isActive.value;
}
</script>

<template>
    <section class="header">
        <div class="container hero__container">
            <div class="header__logo">
                 <a class="header__left-logo" href="#">
                    <svg class="header__left-logo-img" width="112" height="36" viewBox="0 0 112 36" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path class="header__left-logo-img-text" d="M48.391 21.177C48.391 16.911 45.88 13.698 41.992 13.698C40.264 13.698 38.806 14.427 37.753 15.831V9H34V28.386H37.456V26.307C38.563 27.819 40.129 28.656 41.992 28.656C45.88 28.656 48.391 25.389 48.391 21.177ZM44.53 21.177C44.53 23.877 42.991 25.308 41.155 25.308C39.292 25.308 37.78 23.85 37.78 21.123C37.78 18.396 39.346 17.019 41.155 17.019C42.991 17.019 44.53 18.423 44.53 21.177ZM53.2259 28.386V9H49.4459V28.386H53.2259ZM63.8274 28.386H66.8784V19.314C66.8784 15.777 64.6644 13.698 60.8844 13.698C57.4014 13.698 54.9984 15.858 54.7824 19.179H58.1574C58.2924 17.559 59.2644 16.614 60.8844 16.614C62.4504 16.614 63.3684 17.559 63.3684 19.179V20.043C62.4774 19.935 61.7754 19.881 60.9654 19.881C56.7534 19.881 54.4854 21.393 54.4854 24.201C54.4854 26.901 56.4834 28.656 59.4804 28.656C61.4514 28.656 62.8824 27.954 63.8274 26.604V28.386ZM58.0224 24.093C58.0224 22.797 59.0754 22.122 61.2084 22.122C61.8564 22.122 62.4774 22.176 63.3684 22.311V23.337C63.3684 25.011 62.2074 26.064 60.2904 26.064C58.8864 26.064 58.0224 25.308 58.0224 24.093ZM72.5155 20.529C72.5155 18.207 73.7845 17.019 75.2695 17.019C76.9705 17.019 77.8075 18.207 77.8075 20.34V28.386H81.5335V19.071C81.5335 15.588 79.5355 13.698 76.6465 13.698C74.7565 13.698 73.2715 14.589 72.2185 16.02V13.968H68.7625V28.386H72.5155V20.529ZM87.1704 28.386V21.69L92.6784 28.386H97.4574L90.7884 20.88L96.7554 13.968H92.4354L87.1704 20.07V9H83.4174V28.386H87.1704ZM103.31 28.656C107.495 28.656 110.627 25.362 110.627 21.177C110.627 16.965 107.495 13.698 103.31 13.698C99.1255 13.698 95.9935 16.965 95.9935 21.177C95.9935 25.362 99.1255 28.656 103.31 28.656ZM103.31 25.335C101.447 25.335 99.8545 23.85 99.8545 21.177C99.8545 18.504 101.447 17.046 103.31 17.046C105.173 17.046 106.766 18.504 106.766 21.177C106.766 23.85 105.173 25.335 103.31 25.335Z" fill="white"/>
                        <path d="M22 6H17V23H22V6Z" fill="#FF7043"/>
                        <path d="M17 28V23H0V28H17Z" fill="#FF7043"/>
                        <path d="M22 11V6L5 6V11H22Z" fill="#FF7043"/>
                        <path d="M0 28H5L5 11H0L0 28Z" fill="#FF7043"/>
                    </svg>
                </a>
                <p class="header__email">mail@blanko.com</p>

                <div @click="activeBurger" :class="{active: isActive}" class="burger">
                    <div class="line-up line"></div>
                    <div class="line-middle line"></div>
                    <div class="line-down line"></div>
                </div>
            </div>
            <div class="header__info">
                <nav class="header__naviagtion">
                    <a href="#landing__section" class="header__naviagtion--landing">Landing</a>
                    <p class="header__naviagtion--all-pages">All pages</p>
                    <a href="#hero__section" class="header__naviagtion--template">Template</a>
                </nav>
                <button class="header__btn">Purchase template</button>
            </div>
            
            <div :class="{active: isActive}" class="burger-menu">
                <nav class="burger-menu__nav">
                    <ul class="burger-menu__nav-items">
                        <li class="burger-menu__nav-items-item"><a class="header__naviagtion--landing link" href="#landing__section">Landing</a></li>
                        <li class="burger-menu__nav-items-item"><a class="header__naviagtion--all-pages link" href="#">All pages</a></li>
                        <li class="burger-menu__nav-items-item"><a class="header__naviagtion--template link" href="#hero__section">Template</a></li>
                        <li class="burger-menu__nav-items-mail"><a class="link" href="mailto:mail@blanko.com">mail@blanko.com</a></li>
                    </ul>
                </nav>
                <button class="burger-menu__button btn">Purchase template</button>
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
        position: relative;
    }

    .burger{
        display: none;

        @media (max-width: 979px) {
            width: 2.5rem;
            height: 2rem;
            padding: 0.25rem;
            display: flex;
            flex-direction: column;
            gap: 0.45rem;
            cursor: pointer;
        }

        &.active{
            .line-up{
                transform: translateY(calc((1.18rem / 2) - (2px / 2))) rotate(45deg);
            }

            .line-middle{
                transform: scaleX(0);
            }

            .line-down{
                transform: translateY(calc((1.18rem / -2) - (2px / -2))) rotate(-45deg);
            }
        }
    }

    .burger-menu{
        display: none;
        
        &.active{
            @media (max-width: 979px) {
                display: flex;
                flex-direction: column;
                gap: 1.5rem;
                max-width: 30rem;
                width: 100%;
                align-items: center;
                position: absolute;
                top: 100%;
                left: 0;
                right: 0;
                background: black;
                padding: 2rem 1rem;
                z-index: 1000;
            }
        }

        &__nav{
            width: 100%;

            &-items{
                @media (max-width: 979px) {
                    display: flex;
                    justify-content: space-between;
                }

                @media (max-width: 767px) {
                    display: grid;
                    grid-template-columns: auto auto;
                    justify-content: center;
                    gap: 0.5rem 2rem;
                }

                &-item {
                    list-style: none;
                    
                    a {
                        color: white;
                        text-decoration: none;
                        
                        &:hover {
                            color: #645b5b;
                            transition: 0.3s;
                        }
                    }
                }

                &-mail{
                    background: rgba($color: #fff, $alpha: 0.12);
                    padding: 0.25rem 0.5rem;
                    border-radius: 0.25rem;
                    list-style: none;
                    
                    a {
                        color: white;
                        text-decoration: none;
                        
                        &:hover {
                            color: #645b5b;
                            transition: 0.3s;
                        }
                    }
                }
            }
        }

        &__button{
            background: #FF7143;
            font-size: 1rem;
            font-weight: 700;
            line-height: 150%;
            padding: 0.75rem 2rem;
            border-radius: 0.375rem;
            white-space: nowrap;
            width: 100%;
            max-width: 20rem;
            color: black;
            border: none;
            cursor: pointer;
        }
    }

    .line{
        border-bottom: 2px solid #fff;
        transition: transform 0.3s ease 0s;
    }

    @media (max-width: 979px) {
        .header__info {
            display: none;
        }

        .header__logo {
            width: 100%;
            justify-content: space-between;
        }
    }

    @media (min-width: 980px) {
        .burger-menu {
            display: none !important;
        }
    }
</style>