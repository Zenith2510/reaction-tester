<template>
  <p>Result is {{ score }} ms</p>
  <div v-if="score < 250">
    <p>You are legend</p>
  </div>
  <div v-else-if="score > 250">
    <p>Weak</p>
  </div>
</template>

<script>
export default {
  props: ["score"],
};
</script>

<style>
p {
  color: blue;
}
</style>
