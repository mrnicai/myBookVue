<template>
  <div class="nav">
    <!-- <h1>导航条</h1> -->
    <p v-for="(item,index) in list" :key="index">
      <slot :item="item" >{{item.name}}</slot>
    </p>
    <p>{{datas}}</p>
  </div>
</template>
<script>
export default {
  props:['datas'],
  data() {
    return {
      list: [
        { id: "1", name: "aa" },
        { id: "2", name: "vb" },
        { id: "3", name: "cc" }
      ]
    };
  }
};
</script>
