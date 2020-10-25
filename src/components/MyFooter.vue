<template>
  <div class="footer footer__container">
    <p class="footer__container--text">all right reserved</p>
    <img
      src="../assets/img/logo_footer.svg"
      alt=""
      class="footer__container--logo"
    />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer {
  &__container {
    background: #1e1e1e;
    display: flex;
    height: 300px;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    &--text {
      color: white;
      font-size: 44px;
      line-height: 1.1em;
      font-weight: bold;
      margin-bottom: 5px;
    }
    &--logo {
      width: 80px;
      height: 69px;
    }
  }
}
</style>