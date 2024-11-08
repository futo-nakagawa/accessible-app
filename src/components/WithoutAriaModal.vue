<template>
    <div v-if="isOpen">
      <h2>モーダルタイトル</h2>
      <p>モーダルの説明内容です。</p>
      <button @click="closeModal">閉じる</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isOpen: true,
      };
    },
    methods: {
      closeModal() {
        this.isOpen = false;
      },
    },
  };
  </script>
  
  <style>
  div {
    border: 1px solid #000;
    padding: 20px;
    margin: 10px;
  }
  </style>
  