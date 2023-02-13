<script>
export default {
  name: 'AppBottomMain',
}
</script>

<template>
    <div class="bottom-main">
        <div>
            <img src="../assets/img/buy-comics-digital-comics.png" alt="Logo">
            <span>DIGITAL COMICS</span>
        </div>
        <div>
            <img src="../assets/img/buy-comics-merchandise.png" alt="Logo">
            <span>DC MERCHANDISE</span>
        </div>
        <div>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="Logo">
            <span>SUBSCRIPTION</span>
        </div>
        <div>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="Logo">
            <span>COMIC SHOP LOCATOR</span>
        </div>
        <div>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="Logo">
            <span>DC POWER VISA</span>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    
    .bottom-main {
        display: flex; 
        align-items: center;
        justify-content: space-evenly;
        background-color: #0282f9; 
        padding: 30px;     
    }
    span {
        padding: 10px;
        color: white;
    }
    img {
        object-fit: cover;
        width: 35px;
        margin-right: 5px;
        align-items: center;
    }
</style>