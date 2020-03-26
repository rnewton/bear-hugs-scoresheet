<template>
    <div>
        <iframe 
            class="airtable-embed airtable-dynamic-height" 
            src="https://airtable.com/embed/shrMGg9Jo9odCmhi4?backgroundColor=green" 
            frameborder="0" 
            onmousewheel="" 
            width="100%" 
            height="1143" 
            style="background: transparent; border: 1px solid #ccc;"
        ></iframe>
    </div>
</template>

<script>
export default {
  name: 'FeedbackForm',
  mounted() {
      let tag = document.createElement('script')
      tag.setAttribute('src', 'https://static.airtable.com/js/embed/embed_snippet_v1.js')
      document.head.appendChild(tag)
  }
}
</script>