<template>
  <div>
    data:
    <code><pre>{{ data }}</pre></code>
  </div>
</template>

<script setup>
const data = await queryContent('/posts/hello-world').findOne()

console.log(data)
</script>