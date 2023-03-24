<script>
    export default {
        name: 'Header',
    }
</script>

<template>
    <div class="body">
        <span>Open the door for a spacious living -</span>
        <div class="links">
            <button>Book a hotel service<img src="../assets/arrow.svg" alt="" /></button>
            <button>Book a hotel service<img src="../assets/arrow.svg" alt="" /></button>
            <button>Book a hotel service<img src="../assets/arrow.svg" alt="" /></button>
        </div>
    </div>
</template>

<style scoped>
.body {
    background: #121212;
    padding: 0 151px;
    height: 287px;
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.body span {
    width: 585px;
    font-weight: 700;
    font-size: 50px;
    line-height: 133.02%;
    text-transform: uppercase;
}
.links {
    display: flex;
    flex-direction: column;
    gap: 16px;
}
.links button {
    width: 235px;
    height: 30px;
    background: transparent;
    color: white;
    border: none;
    border-bottom: 2px solid white;
    display: flex;
    justify-content: space-between;
    align-content: center;
}
</style>