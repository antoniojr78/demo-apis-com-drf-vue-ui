<template>
  <!-- Obs.: Div required -->
  <div>
      {{ authors }}
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'Authors',
  data(){
      return {
          authors: null
      }
  },
  mounted() {
      axios.get("http://localhost:8000/api/authors/")
      .then(resp=>this.authors = resp.data)
  }
}
</script>