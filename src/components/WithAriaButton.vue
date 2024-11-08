<template>
    <button class="styled-button" role="button" aria-label="Submit" @click="handleClick">
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
        alert('WAI-ARIA導入ボタンがクリックされました');
      },
    },
  };
  </script>
  
  <style>
  .styled-button {
    background-color: #007bff;
    color: white;
    border: none;
    border-radius: 4px;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.3s;
  }
  .styled-button:hover {
    background-color: #0056b3;
  }
  </style>
  