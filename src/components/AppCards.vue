<script>
export default {
  name: 'AppCards',
  props: {
    cardImg: String,
    cardTitle: String
    }
  }
</script> 

<template>
    <div class="card">
      <a href="#"><img :src="cardImg" /></a>
      <h5>{{ cardTitle }}</h5>
    </div>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
  .card {
    font-family: 'Open Sans', sans-serif;
    padding: 15px;
    width: 150px;
    height: 150px;
    margin-bottom: 30px;
    cursor: pointer;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: top;
    }
    h5 {
      color: white;
      text-transform: uppercase;
      min-height: 20px;
      padding-top: 5px;
      margin-top: 15px;
    }
  } 
</style>