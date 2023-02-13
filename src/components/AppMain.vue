<script>
import AppCards from './AppCards.vue';
import comics from '../data/comics';
import AppBottomMain from './AppBottomMain.vue';
export default {
  name: "AppMain",
  components: { AppCards, AppBottomMain },
  data() {
    return {
      comics,
    };
  },
};
</script>

<template>
    <main>
        <div class="container">
            <div class="cards">
                <AppCards class="cards-container" v-for="(card, index) in comics" :key="index" :cardImg="card.thumb" :cardTitle="card.series"/> 
            </div> 
            <div class="btn">
                <a href="#">LOAD MORE</a>
            </div>
            <div class="container">
                <AppBottomMain/>
            </div>
        </div>
    </main>   
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
.container {
  font-family: 'Open Sans', sans-serif;
  background-color: #1c1c1c;
  display: flex;
  flex-direction: column;
  position: relative;
  .cards {
    display: flex;
    flex-wrap: wrap;
    padding-top: 50px;
  }
  .cards-container {
    width: calc(100% / 6);
    height: 170px;
    padding: 10px 10px;
    margin-bottom: 50px;
  }
  .btn {
    margin: 50px auto;
    width: 150px;
    text-align: center;
    background-color: #0282f9;
    padding: 10px 15px;
    cursor: pointer;
    a {
      color: white;
      font-weight: bold;
      text-decoration: none;
      text-transform: uppercase;
    }
  }  
}
</style>