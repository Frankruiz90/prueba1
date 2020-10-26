<template>
  <div class="heaer_container">
    <div class="title__container">
      <h1 class="title">Welcome to the family</h1>
      <div class="icon__container--down">
        <a href="#history">
          <img src="../assets/img/iconoAbajo.svg" alt="" />
        </a>
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
  padding-top: 110px;
  width: 100%;
  height: 400px;
  background: -webkit-linear-gradient(
    left,
    rgba(0, 187, 255, 1) 0%,
    rgba(136, 200, 156, 1) 50%,
    rgba(161, 203, 0, 1) 100%
  );
  clip-path: ellipse(71% 68% at 40% 26%);

  position: relative;
  text-align: -webkit-center;

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
    position: relative;
    margin-top: 20px;
    bottom: 0;
    width: 50px;
    animation: upAndDown 5s ease-in-out infinite;
    transition: all 0.5s;
  }
  @keyframes upAndDown {
    0% {
    }
    50% {
      bottom: -50px;
    }
    100% {
      bottom: 0px;
    }
  }
  @media screen and (min-width: 768px) {
    background-size: inherit;
    min-height: 600px;
    .logo-container {
      position: absolute;
    }

    .links_container {
      display: inline;
    }
    .title__container {
      height: 100%;
    }

    @keyframes upAndDown {
      0% {
      }
      50% {
        bottom: -100px;
      }
      100% {
        bottom: 0px;
      }
    }
  }
}
</style>