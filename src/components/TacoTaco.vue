<template>
  <div class="taco-container">
    <p v-for="(data, index) in tacos" :key="index">I have a {{ data.taco }} taco.</p>
    <p v-if="tacos.length >= 4">I am wise</p>
    <p else>I need more tacos.</p>
  </div>
</template>


<script>
export default {
  name: "TacoTaco",
  data() {
    return {
      tacos: [
        { taco: "carnitas" },
        { taco: "super sweet al pastor" },
        { taco: "weird" }
      ]
    };
  }
};
</script>


<style>
.taco-container {
  background-color: hsl(185, 50%, 75%);
  padding: 3rem;
}
</style>