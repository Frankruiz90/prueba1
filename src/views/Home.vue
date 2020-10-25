<template>
  <div class="home">
    <my-nav-bar />
    <new-header id="new-header" />
    <history id="history" />
    <my-form id="my-form" />
    <my-footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NewHeader from "@/components/NewHeader.vue";
import History from "@/components/History.vue";
import MyForm from "@/components/MyForm.vue";
import MyFooter from "@/components/MyFooter.vue";
import MyNavBar from "@/components/MyNavBar.vue";

export default {
  name: "Home",
  components: {
    NewHeader,
    History,
    MyForm,
    MyFooter,
    MyNavBar,
  },
};
</script>
