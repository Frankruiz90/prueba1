<template>
  <div class="home">
    <new-header />
    <history />
  </div>
</template>

<script>
// @ is an alias to /src
import NewHeader from '@/components/NewHeader.vue'
import History from '@/components/History.vue'

export default {
  name: 'Home',
  components: {
    NewHeader,
    History
  }
}
</script>
