<template>
    <div>
      <button @click="selectTab(1)">タブ1</button>
      <button @click="selectTab(2)">タブ2</button>
      <div v-if="selectedTab === 1">タブ1の内容</div>
      <div v-if="selectedTab === 2">タブ2の内容</div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        selectedTab: 1,
      };
    },
    methods: {
      selectTab(tab) {
        this.selectedTab = tab;
      },
    },
  };
  </script>
  
  <style>
  button {
    margin: 5px;
    padding: 5px 10px;
  }
  </style>
  