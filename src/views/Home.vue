<template>
  <div class="home">
    <new-header />
    <history />
    <my-form />
    <my-footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NewHeader from '@/components/NewHeader.vue'
import History from '@/components/History.vue'
import MyForm from '@/components/MyForm.vue'
import MyFooter from '@/components/MyFooter.vue'

export default {
  name: 'Home',
  components: {
    NewHeader,
    History,
    MyForm,
    MyFooter
  }
}
</script>
