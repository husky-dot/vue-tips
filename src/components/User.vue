<template>
  <div>
    <p>私有数据:{{ privateData }}</p>
    <p>私有数据(大写):{{ upperCasePrivateData }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      privateData: "secrecy",
    };
  },
  computed: {
    upperCasePrivateData() {
      return this.privateData.toUpperCase();
    },
  },
};
</script>
