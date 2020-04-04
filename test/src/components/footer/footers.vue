<template>
  <div class="footer">
    <!-- <h1>我是尾部</h1> -->
    <footers_nav @a='sss'></footers_nav>
  </div>
</template>
<script>
import footers_nav from "./footers-nav";
export default {
  components: {
    footers_nav
  },
  methods:{
      sss:(a)=>{
        //   this.
        console.log(a)
      }
  }
};
</script>>