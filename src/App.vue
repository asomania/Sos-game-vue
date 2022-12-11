<template>
  <div class="app">
    <div class="flex button">
      <button>S</button>
      <button>O</button>
    </div>
    <div class="flex">
      <div v-for="n in 10" :key="n" class="hello" @click="getKey(n)"></div>
    </div>
    <div class="flex">
      <div v-for="n in 10" :key="n" class="hello" @click="getKey(n)"></div>
    </div>
    <div class="flex">
      <div v-for="n in 10" :key="n" class="hello" @click="getKey(n)"></div>
    </div>
    <div class="flex">
      <div v-for="n in 10" :key="n" class="hello" @click="getKey(n)"></div>
    </div>
    <div class="flex">
      <div v-for="n in 10" :key="n" class="hello" @click="getKey(n)"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  methods: {
    getKey: (n) => {
      //key
      console.log(n);
    },
  },
};
</script>
55

<style>
.app {
  flex-wrap: wrap;
  margin-top: 4rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.flex {
  display: flex;
}

.hello {
  width: 100px;
  height: 100px;
  border: 1px solid #000;
}
.button {
  margin-bottom: 1rem;
  gap: 1rem;
  font-size: 2rem;
}
</style>
