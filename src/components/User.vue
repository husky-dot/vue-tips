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

/* :slotted(.userInfo){
  color: red;
} */

/* :global(.red) {
  color: red;
} */
</style>
