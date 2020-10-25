<template>
  <div class="information information__container">
    <h1 class="information__title">Form</h1>
    <div class="information__form__container">
      <form action="" class="form" method="post">
        <label class="form__text" for="">Nombre *</label>
        <input
          class="form__input"
          type="text"
          name=""
          id=""
          required
          v-model="name"
        />
        <label class="form__text" for="">Apellido</label>
        <input class="form__input" type="text" name="" id="" />
        <label class="form__text" for="">Correo *</label>
        <input
          class="form__input"
          type="email"
          name=""
          id=""
          required
          v-model="mail"
        />
        <label class="form__text" for="">Fecha de Nacimiento *</label>
        <input
          class="form__input"
          type="date"
          name=""
          id=""
          required
          v-model="date"
        />
        <input
          type="checkbox"
          class="form__checkbox--style"
          name=""
          id="accept"
          v-model="check"
        />
        <label class="form__text form__text--checkbox" for="accept">
          Acepto terminos y condiciones *
        </label>
        <label class="form__parraf">
          Contrary to popular belief, Lorem Ipsum is not simply random text. It
          has roots in a piece of classical Latin literature from 45 BC, making
          it over 2000 years old. Richard McClintock, a Latin
        </label>
        <button class="form__btn" :disabled="!name || !mail || !date || !check">
          Enviar
        </button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      mail: "",
      date: "",
      check: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.information {
  &__container {
    margin-top: 40px;
    padding: 20px 96px;
    background: -webkit-linear-gradient(
      left,
      rgba(0, 187, 255, 1) 0%,
      rgba(136, 200, 156, 1) 50%,
      rgba(161, 203, 0, 1) 100%
    );
    height: auto;
  }
  &__title {
    color: white;
    line-height: 1.1em;
    font-weight: bold;
    font-size: 70px;
  }
  &__form__container {
    border: solid 1px white;
    border-radius: 25px;
    // height: 300px;
    padding: 93px;
    padding-top: 50px;
    .form {
      display: flex;
      flex-direction: column;
      &__text {
        text-align: left;
        color: white;
        font-size: 40px;
        font-weight: bold;
        line-height: 1.1em;
        margin-top: 10px;
      }
      &__text--checkbox {
        text-align: center;
        position: relative;
        padding-left: 28px;
        max-width: 700px;
        margin: 10px auto;
        &::before {
          content: "";
          border: solid 1px white;
          width: 20px;
          height: 20px;
          position: absolute;
          left: 0;
          top: 50%;
        }
      }
      &__checkbox--style {
        display: none;
        &:checked + label::before {
          color: green;
          content: "\f00c";
          font-family: FontAwesome;
        }
      }
      &__input {
        padding-left: 10px;
        margin: 5px 0;
        height: 50px;
        border-radius: 12px;
        background: none;
        color: white;
        font-size: 25px;
        border: 1px solid white;
        &::before {
          opacity: 0.5;
        }
        &:focus {
          border: 2px solid #ff1d25;
        }
        &:focus {
          outline: none;
        }
      }
      &__parraf {
        padding-left: 10px;
        margin: 5px auto;
        max-width: 600px;
        color: white;
        line-height: 1.1em;
        font-weight: bold;
        font-size: 16px;
      }
      &__btn {
        margin-top: 10px;
        height: 50px;
        width: 150px;
        border-radius: 12px;
        align-self: flex-end;
        font-size: 25px;
        line-height: 1.1em;
        font-weight: bold;
        color: #48484a;
      }
    }
  }
}
</style>