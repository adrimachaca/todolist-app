<script>
import Header from '@/components/Header.vue';
import Sidebar from '@/components/Sidebar.vue';

export default {
  components: {
    Header,
    Sidebar
  }
};
</script>

<template>
  <div class="container">
    <Header />
    <Sidebar />
  </div>  
</template>

<style scoped>
  .container {
    background-color: lightgreen;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
</style>