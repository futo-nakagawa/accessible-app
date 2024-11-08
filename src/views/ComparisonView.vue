<template>
    <div class="comparison-view">
      <div class="side">
        <h2>WAI-ARIA導入</h2>
        <WithAriaButton label="送信" />
        <WithAriaNav />
        <WithAriaTabs />
        <WithAriaModal />
      </div>
      <div class="side">
        <h2>WAI-ARIA未導入</h2>
        <WithoutAriaButton label="送信" />
        <WithoutAriaNav />
        <WithoutAriaTabs />
        <WithoutAriaModal />
      </div>
    </div>
  </template>
  
  <script>
  import WithAriaButton from '../components/WithAriaButton.vue';
  import WithoutAriaButton from '../components/WithoutAriaButton.vue';
  import WithAriaNav from '../components/WithAriaNav.vue';
  import WithoutAriaNav from '../components/WithoutAriaNav.vue';
  import WithAriaTabs from '../components/WithAriaTabs.vue';
  import WithoutAriaTabs from '../components/WithoutAriaTabs.vue';
  import WithAriaModal from '../components/WithAriaModal.vue';
  import WithoutAriaModal from '../components/WithoutAriaModal.vue';
  
  export default {
    components: {
      WithAriaButton,
      WithoutAriaButton,
      WithAriaNav,
      WithoutAriaNav,
      WithAriaTabs,
      WithoutAriaTabs,
      WithAriaModal,
      WithoutAriaModal,
    },
  };
  </script>
  
  <style>
  .comparison-view {
    display: flex;
    justify-content: space-around;
  }
  
  .side {
    width: 45%;
    padding: 20px;
    border: 1px solid #ccc;
  }
  </style>
  