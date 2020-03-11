<template>
  <component :is="component" />
</template>

<script>
import Input from "./Input";

export default {
  data() {
    return {
      component: Input
    };
  }
};
</script>

<style>
</style>