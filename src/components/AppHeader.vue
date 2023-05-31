<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "AppHeader",
}

</script>


<template>
  <nav>
    <a href="#">
      <img src="../assets/img/favicon.ico" alt="#">
    </a>
    <ul>
      <li>
        <a href="#">CHARACTERS</a>
      </li>
      <li>
        <a href="#">COMICS</a>
      </li>
      <li>
        <a href="#">MOVIES</a>
      </li>
      <li>
        <a href="#">TV</a>
      </li>
      <li>
        <a href="#">GAMES</a>
      </li>
      <li>
        <a href="#">COLLECTIBLES</a>
      </li>
      <li>
        <a href="#">VIDEO</a>
      </li>
      <li>
        <a href="#">FANS</a>
      </li>
      <li>
        <a href="#">NEWS</a>
      </li>
      <li>
        <a href="#">SHOP</a>
      </li>
    </ul>
  </nav>
</template>


<style lang="scss" scoped>
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 80px;

  img {
    width: 50px;
    height: 50px;
  }

  ul {
    display: flex;
    font-size: 12px;
    font-weight: bold;
    list-style-type: none;

    li {
      padding: 0 10px;

      a {
        color: rgb(120, 118, 118);
        text-decoration: none;
      }
    }
  }
}
</style>
