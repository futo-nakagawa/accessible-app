<template>
  <div id="app">
    <header class="header">
      <h1>WAI-ARIA 比較サイト</h1>
    </header>
    <ComparisonView />
  </div>
</template>

<script>
import ComparisonView from './views/ComparisonView.vue';

export default {
  components: {
    ComparisonView,
  },
};
</script>

<style>
#app {
  font-family: 'Roboto', sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f8f9fa;
}
.header {
  background-color: #343a40;
  color: #ffffff;
  padding: 15px;
  text-align: center;
}
</style>
