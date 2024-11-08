<template>
    <button @click="handleClick">
      {{ label }}
    </button>
  </template>
  
  <script>
  export default {
    props: {
      label: {
        type: String,
        default: '送信',
      },
    },
    methods: {
      handleClick() {
        alert('WAI-ARIA未導入ボタンがクリックされました');
      },
    },
  };
  </script>
  
  <style>
  button {
    padding: 10px 20px;
    margin: 10px;
    font-size: 16px;
  }
  </style>

