<template>
  <div>
    <h1 v-for="item in data">{{item}}</h1>
    <span @click="aa">dianwo</span>
  </div>
</template>
<script>
export default {
  data() {
    return {
      data: [1, 2, 3]
    };
  },
  methods: {
    aa() {
      this.$emit("a", this.data);
    }
  }
};
</script>