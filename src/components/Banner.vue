<script>
    export default {
        name: 'Banner',
        data() {
            return {
                menu: []
            }
        },
        mounted() {
            this.menu = [
                {
                    id: 1,
                    image: 'welcome_drinks.svg',
                    text: 'Welcome Drinks'
                },
                {
                    id: 2,
                    image: 'car_rental.svg',
                    text: 'Car Rental'
                },
                {
                    id: 3,
                    image: 'resort_spa.svg',
                    text: 'Resort & Spa'
                },
                {
                    id: 4,
                    image: 'wifi.svg',
                    text: 'Free WIFI'
                }
            ]
        },
        methods: {
            getImgUrl(path) {
                return require('../assets/' + path)
            }
        }
    }
</script>

<template>
    <div class="banner"></div>
    <div class="menu">
        <div v-for="item in menu" :key="item.id" class="menuObj">
            <div class="image">
                <img :src="`/src/assets/${item.image}`" alt="">
            </div>
            <span>{{ item.text }}</span>
        </div>
    </div>
    <h2 class="heading">Why You Should <span>Stay Here</span></h2><br/>
    <p class="subtitle">Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat.</p>
</template>

<style scoped>
    .banner {
       width: 100%;
       height: 565px;
       background: url("/src/assets/bg-main.png");
    }
    .menu {
        width: 840px;
        height: 74px;
        /* background: red; */
        margin: 71px auto 139px;
        display: flex;
        gap: 40px
    }
    .menuObj {
        display: flex;
        align-items: center;
        gap: 40px;
    }
    .menuObj span {
        color: #565656;
    }
    .image {
        width: 74px;
        height: 74px;
        background: #FF75000A;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 50%;
    }
    .heading {
        font-weight: 700;
        font-size: 45px;
        line-height: 133.02%;
        color: #292929;
        text-align: center;
    }
    .heading span {
        color: #FF7500;
    }
    .subtitle {
        font-size: 16px;
        max-width: 475px;
        font-weight: 500;
        line-height: 175.52%;
        color: #292929;
        opacity: 0.4;
        text-align: center;
        margin: 0 auto;
    }
</style>