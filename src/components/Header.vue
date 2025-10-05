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
                    <p>Landing</p>
                    <p>All pages</p>
                    <p>Template</p>
                </nav>
                <button class="header__btn">Purchase template</button>
            </div>
            
        </div>
    </section>
</template>

<style scoped>
    .header {
        background-color: black;
        padding: 16px 0px 16px 0px;
        align-items: center;
        margin: 0 auto;
    }

    .hero__container {
        max-width: 90rem;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 272px;
    }

    .header__logo {
        display: flex;
        gap: 65px;
    }

    .header__email {
        background-color: gray;
        color: white;
        border: 2px solid gray;
        padding: 4px 8px;
    }

    .header__info {
        display: flex;
        gap: 65px;
    }

    .header__naviagtion {
        display: flex;
        color: white;
        gap: 20px;
        align-items: center;
    }

    .header__btn {
        color: black;
        background: #FF7143;
        border-color: #FF7143;
        border-radius: 6px;
        padding: 12px 32px;
        font-weight: bold;
    }
</style>
