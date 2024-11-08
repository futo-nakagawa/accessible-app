<template>
    <div v-if="isOpen" role="dialog" aria-labelledby="modalTitle" aria-describedby="modalDesc">
      <h2 id="modalTitle">モーダルタイトル</h2>
      <p id="modalDesc">モーダルの説明内容です。</p>
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
  