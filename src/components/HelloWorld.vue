<template>
  <div class="hello" @click="getKey($event)">{{ n }}</div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {};
  },
  props: {
    msg: String,
  },
  methods: {
    getKey: (event) => {
      //key
      console.log(event.target);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  width: 100px;
  height: 100px;
  border: 1px solid #000;
}
</style>
