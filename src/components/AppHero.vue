<script>
export default {
  name: "AppHero",
};
</script>

<template>
    <section class="hero">
          <div class="current-series">
              <h3>CURRENT SERIES</h3>
          </div>
    </section>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');

.hero {
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: cover;
    height: 345px;
    .current-series {
        font-family: 'Open Sans', sans-serif;
        color:white;
        position: absolute;
        top: 400px;
        left: 250px;
        z-index: 100;
    }
    h3 {
        background-color: #0282f9;
        display: inline-block;
        text-align: center;
        padding: 10px 25px;
    }
}
</style>
