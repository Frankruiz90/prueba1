<template>
  <div class="history history__container">
    <h1 class="history__title">History</h1>
    <p class="history__text">
      Lorem Ipsum es simplemente el texto de relleno de las imprentas y archivos
      de texto. Lorem Ipsum ha sido el texto de relleno estándar de las
      industrias desde el año 1500, cuando un impresor (N. del T. persona que se
      dedica a la imprenta) desconocido usó una galería de textos y los mezcló
      de tal manera que logró hacer un libro de textos especimen. No sólo
      sobrevivió 500 años, sino que tambien ingresó como texto de relleno en
      documentos electrónicos, quedando esencialmente igual al original. Fue
      popularizado en los 60s con la creación de las hojas "Letraset", las
      cuales contenian pasajes de Lorem Ipsum, y más recientemente con software
      de autoedición, como por ejemplo Aldus PageMaker, el cual incluye
      versiones de Lorem Ipsum.
    </p>
    <div class="history__image">
      <img src="../assets/img/foto.svg" class="history__image--foto" />
      <h1 class="history__image--text">#Developers</h1>
    </div>
    <h1 class="history__title">Contact</h1>
    <p class="history__text">
      Lorem ipsum dolor sit amet consectetur adipiscing elit, potenti neque
      hendrerit nostra libero convallis donec, nam dapibus tempor vulputate quam
      nibh. Tempor urna feugiat semper iaculis eros mauris integer class, nisi
      eleifend nibh consequat nullam habitasse ridiculus morbi, molestie arcu eu
      odio aenean tellus massa. Dignissim luctus sollicitudin rutrum porttitor
      fames magna augue dictum, id pretium natoque justo tortor dis netus, ut
      vulputate at vitae suspendisse nullam nascetur. Scelerisque lacus
      tincidunt eget euismod placerat rhoncus arcu, nulla potenti cum purus
      condimentum aenean, tellus nisi risus dignissim elementum senectus.
    </p>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.history {
  &__title {
    color: #48484a;
    line-height: 1.1em;
    font-weight: bold;
    font-size: 70px;
  }
  &__text {
    font-size: 16px;
    line-height: 1.1em;
    color: #48484a;
    padding: 0 50px;
  }
  &__image {
    margin-top: 30px;
    position: relative;
    // background-image: url("../assets/img/foto.svg");
    // background-repeat: no-repeat;

    &--foto {
      border-radius: 150px 50%;
    }
    &--text {
      color: white;
      line-height: 1.1em;
      font-weight: bold;
      font-size: 70px;
      position: absolute;
      top: 25%;
      left: 15%;
    }
  }
  @media screen and (min-width: 768px) {
    &__text {
      padding: 0 200px;
    }
    &__image {
      &--text {
        top: 37%;
        left: 35%;
      }
    }
  }
}
</style>