<template>
  <div class="head">
    <h1>我是头部</h1>
    <navs :datas='list'>
      <template slot-scope="slotProps">
        <span v-if="slotProps.item.id=='2'" class="te">{{slotProps.item.name}}</span>
        <span v-else>{{slotProps.item.name}}</span>
      </template>
    </navs>
  </div>
</template>
<script>
import navs from "./nav";
export default {
  components: {
    navs
  },
  data() {
    return {
      list: [1, 2, 3]
    }
  }
};
</script>
<style scoped>
.te {
  color: red;
  font-size: 20px;
}
</style>>