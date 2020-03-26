<template>
  <div class="home container">
    <ScoreSheet />
    <FeedbackForm />
  </div>
</template>

<script>
// @ is an alias to /src
import ScoreSheet from '@/components/ScoreSheet.vue'
import FeedbackForm from '@/components/FeedbackForm.vue'

export default {
  name: 'home',
  components: {
    ScoreSheet,
    FeedbackForm,
  }
}
</script>
