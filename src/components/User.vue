// User.vue
<template>
  <div class="user">
    <slot />
  </div>
</template>

<style scoped>
.user .userInfo {
  color: red;
}

/* 插槽选择器 */
/* :slotted(.userInfo){
  color: red;
} */

/* 全局选择器 */
/* :global(.red) {
  color: red;
} */
</style>


