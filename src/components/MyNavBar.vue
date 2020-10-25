<template>
  <div class="navbar navbar__container">
    <div class="navbar__container--logo">
      <a href="#new-header">
        <img src="../assets/img/logo.svg" alt="" />
      </a>
      
    </div>
    <div class="links__container">
      <a class="links__container--text" href="#history">History</a>
      <a class="links__container--text" href="#my-form">Form</a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {

    }
  },
};
</script>

<style lang="scss" scoped>
.navbar {
  &__container {
    position: fixed;
    z-index: 100;
    padding: 1rem;
    width: 100%;
    background: -webkit-linear-gradient(
      left,
      rgba(0, 187, 255, 1) 0%,
      rgba(136, 200, 156, 1) 50%,
      rgba(161, 203, 0, 1) 100%
    );
    background-color: yellowgreen;
    text-align: -webkit-center;

    &--logo {
      width: 76px;
      position: relative;
      margin: 0.5rem;
      transition: all 0.5s;
      &:hover {
        width: 86px;
      }
    }
    .links__container {
      display: none;
      position: absolute;
      top: 1rem;
      right: 1rem;
      margin: 0.5rem;
      text-align: right;
      padding-right: 2rem;
      a {
        text-decoration: none;
        &:active {
          color: #00bcff;
        }
      }
      &--text {
        margin: 1rem;
        color: white;
        font-size: 40px;
        line-height: 1.1em;
        font-weight: bold;
        transition: all 0.5s;
        &:hover {
          font-size: 50px;
        }
      }
    }
  }
  @media screen and (min-width: 768px) {
    &__container {
          text-align: -webkit-left;
      .links__container {
        display: inline;
      }
    }
  }
}
</style>