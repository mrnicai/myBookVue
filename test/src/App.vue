<template>
  <div id="app">
    <headers></headers>
    <router-view/>
    <footers></footers>
  </div>
</template>
<script>
import headers from './components/header/headers.vue'
import footers from './components/footer/footers.vue'
export default {
  data(){
    return{}
  },
  components:{
    headers,footers
  }
  
}
</script>
