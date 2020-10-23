<template>
  <div class="home">
    <new-header />
  </div>
</template>

<script>
// @ is an alias to /src
import NewHeader from '@/components/NewHeader.vue'

export default {
  name: 'Home',
  components: {
    NewHeader
  }
}
</script>
