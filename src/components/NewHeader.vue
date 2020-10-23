<template>
  <div class="heaer_container">
    <div class="logo-container">
      <img src="../assets/img/logo.svg" alt="" />
    </div>
    <div class="links_container">
      <a class="link__text" href="">History</a>
      <a class="link__text" href="">Form</a>
    </div>
    <div class="title__container">
      <h1 class="title">Welcome to the family</h1>
      <div class="icon__container--down">
        <img src="../assets/img/iconoAbajo.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.heaer_container {
  padding: 1rem;
  width: 100%;
  height: 400px;
  background: -webkit-linear-gradient(
    left,
    rgba(0, 187, 255, 1) 0%,
    rgba(136, 200, 156, 1) 50%,
    rgba(161, 203, 0, 1) 100%
  );
  // background-repeat: no-repeat, repeat;
  // background-image: url("../assets/img/pequeno.svg");

  position: relative;
  text-align: -webkit-center;

  // background-size: 100%;

  .logo-container {
    width: 76px;
    position: relative;
    margin: 0.5rem;
  }
  .links_container {
    display: none;
    position: absolute;
    top: 1rem;
    right: 1rem;
    margin: 0.5rem;
    text-align: right;
    a {
      text-decoration: none;
      &:active {
        color: #00bcff;
      }
    }
    .link__text {
      margin: 1rem;
      color: white;
      font-size: 40px;
      line-height: 1.1em;
      font-weight: bold;
    }
  }
  .title__container {
    position: relative;
    display: flex;
    width: 80%;
    height: 80%;
    place-content: center;
    background: center;
    flex-direction: column;
    align-items: center;
    .title {
      color: white;
      line-height: 1.1em;
      font-weight: bold;
      font-size: 70px;
    }
  }
  .icon__container--down {
    // padding-top: 110px;
    position: absolute;
    bottom: 0;
    width: 50px;
  }
  @media screen and (min-width: 768px) {
    // background-image: url("../assets/img/ss.svg");
    background-size: inherit;
    min-height: 600px;
    // background-size: cover;
    .logo-container {
      position: absolute;
    }

    .links_container {
      display: inline;
    }
    .title__container {
      height: 100%;
    }
    .icon__container--down {
      // padding-top: 210px;
    }
  }
}
</style>