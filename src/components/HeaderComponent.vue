<template>
<header>
  <div class="container">
    <div class="flex">
      <!-- header image -->
      <div class="header-img">
        <img src="../assets/img/dc-logo.png" alt="logo DC">
      </div>
      <!-- header menu -->
      <div class="header-menu">
        <nav>
          <ul class="flex">
            <li>
              <a href="#">CHARACTERS</a>
            </li>
            <li class="active">
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
              <a href="#">VIDEOS</a>
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
      </div>
    </div>
  </div>
</header>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      
    }
  }
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/Variables.scss";

// *STYLING
.container .flex {
  justify-content: space-between;
}
header {
  background-color: #fff;
  box-shadow: 0 0 5px black;
  position: relative;
  z-index: 100;
}
.header-img {
  padding: 0.8rem 0;
  width: 6%;
}
.header-menu {
  font-size: $main-font-size;
  font-weight: $main-font-weight;

  nav {
    height: 100%;

    ul {
      height: 100%;

      li {
        margin-left: 1rem;
        display: flex;
        align-items: center;

        &.active {
          color: $main-color;
          box-shadow: 0 -5px $main-color inset;
        }
      }
    }
  }
}
</style>
