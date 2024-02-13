<template>
  <h4>Your Balance</h4>
  <h1 id="balance">${{ Math.round(total * 100) / 100 }}</h1>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  total: {
    type: Number,
    required: true,
  },
});
</script>
