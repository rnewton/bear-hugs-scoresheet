<template>
  <div class="home container">
    <ScoreSheet />
  </div>
</template>

<script>
// @ is an alias to /src
import ScoreSheet from '@/components/ScoreSheet.vue'

export default {
  name: 'home',
  components: {
    ScoreSheet
  }
}
</script>
