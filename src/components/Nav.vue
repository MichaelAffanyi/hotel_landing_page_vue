<script>
    export default {
        data() {
            return {

            }
        },
        name: 'Nav',
    }
</script>

<template>
    <div class="body">
        <div class="logo">The<br/> Breakdance</div>
        <ul>
            <li>Home</li>
            <li>Services</li>
            <li>About us</li>
            <li>Room</li>
            <li>Contact</li>
        </ul>
        <button>Book now</button>
    </div>
</template>

<style scoped>
    .body {
        background: #121212;
        height: 123px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 151px;
        color: white;
    }
    .logo {
        font-weight: 700;
        font-style: 18px;
    }
    ul {
        display: flex;
        gap: 44px;
        text-decoration: none;
        list-style: none;
        margin-left: 73px;
        font-weight: 500;
        font-style: 16px;
    }
    li {
        cursor: pointer;
    }
    button {
        padding: 14px 47px;
        background: transparent;
        border: 2px solid white;
        color: white;
        font-weight: bold;
    }
</style>