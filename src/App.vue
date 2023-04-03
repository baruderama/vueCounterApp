<template>
  <main>
    <div>
      <h4>
        The current is ...
      </h4>
      <h1>{{ count }}</h1>
      <button @click="count--">-</button>
      <button @click="count++">+</button>
      <button @click="subtractToCount()">-</button>
      <button @click="addToCount()">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aquamarine;
  height: 100vh;
  width: 100vw;
  display: flex;

  align-items: center;
  justify-content: center;

}

div {
  text-align: center;
}
</style>


<!-- Compositions API -->
<script setup>
  import {ref} from "vue";

  const count =ref (0);
</script>


<!-- options API -->
<!-- <script>
export default ({
  data() {
    return {
      count: 0
    }
  },
  methods: {
    addToCount() {
      this.count = this.count + 1

    },
    subtractToCount() {
      this.count = this.count - 1

    }

  }
}
)
</script> -->