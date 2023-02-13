<script>
import nav from '../data/nav';
export default {
  name: "AppHeader",
  data() {
    return {
      nav
    };
  },
};
</script>

<template>
    <header>
      <div class="container">
            <img src="../assets/img/dc-logo.png" alt="logo" />
      </div>
      <div>
            <nav>
                <ul>
                <li v-for="(link, index) in nav" :key="index">
                    <a :href="link.href">{{ link.text }}</a>
                </li>
                </ul>
            </nav>
      </div>
    </header>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-family: 'Open Sans', sans-serif;
  height: 80px;
  background-color:white;
  padding: 15px;
  img {
    width: 80px;
    margin-left: 100px;
    cursor: pointer;
    padding: 10px;
  }
  ul {
    display: flex;
    justify-self: flex-end;
    align-items: center;
    margin-right: 100px;
    width: 600px;
    list-style: none;
  }
  li {
    margin-left: 20px;
    font-size: 10px;
    font-weight: bold;
  }
  a {
    text-decoration: none;
    color: #1c1c1c;
    padding-bottom: 30px;
  }
  a:hover {
    color: #0282f9;
    border-bottom: 4px solid #0282f9;
  }
}
</style>