<script setup lang="ts">
const client = useSupabaseClient();

client.from("*").on("*", (payload) => {
  console.log("Change received!", payload);
});
</script>

<template>
  <div></div>
</template>
