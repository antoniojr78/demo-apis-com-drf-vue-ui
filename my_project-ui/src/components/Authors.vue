<template>
  <!-- Obs.: Div required -->
  <div>
      <h1 class="text-center text-info">List of Authors</h1>
      <ul class="list-group-item" v-for="author in authors" v-bind:key="author.id">
        <li class="list-group-item">{{ author.name }}</li>
        <li class="list-group-item">{{ author.address }}</li>
        <li class="list-group-item" v-if="author.site === null || author.site.trim() == ''">Not Informe</li>
        <li class="list-group-item" v-else>{{ author.site }}</li>
        <li class="list-group-item">{{ author.email }}</li>
        <br/>
      </ul>
  </div>
</template>

<script>
import axios from 'axios'
import 'bootstrap/dist/css/bootstrap.min.css'
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