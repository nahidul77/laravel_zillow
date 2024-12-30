<template>
  <MainLayout>
    <div>The page with time {{ timer }}</div>
    <div>Show</div>
    <Link href="/">Main Page</Link>
  </MainLayout>
</template>

<script setup>
import { Link } from "@inertiajs/vue3";
import { ref } from "vue";
import MainLayout from "../../Layouts/MainLayout.vue";

const timer = ref(0);
setInterval(() => timer.value++, 1000);
</script>