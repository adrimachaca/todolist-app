<script>
export default {
   props: {
      title: String,
      icon: String
   }
};
</script>

<template>
   <div class="item-box">
      <i :class="`pi ${icon}`" style="color: #45474B; font-size: 1.1rem"></i>
      <p>{{ title }}</p>
   </div>
</template>

<style scoped>

.item-box {
   background-color: #fefefe;
   display: flex;
   flex-direction: row;
   align-items: center;
   padding: 15px 30px;
   margin-bottom: 2px;
}

.item-box p {
   margin-left: 10px;
}

</style>