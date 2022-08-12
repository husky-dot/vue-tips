<script setup>

// `toRef` 可以用来为源响应式对象的某个 `property` 新创建一个 `ref`，
// 然后 `ref `可以被传递，它会保持对其源 `property` 的响应式连接。

import { reactive, toRef } from "vue";

const state = reactive({
  foo: 1,
  bar: 2,
});

const fooRef = toRef(state, "foo");

fooRef.value++;
console.log(state.foo); // 2

state.foo++;
console.log(fooRef.value); // 3
</script>
