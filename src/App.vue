<script setup>
import { useTableStore } from "./store/table";
const tableStore = useTableStore();

onMounted(async () => {
  await tableStore.fetchTables();
});



</script>

<template>
  <VApp>
    <RouterView />
  </VApp>
</template>
