<template>
  <div id="app">
    <div v-for="item in inputs" :key="item.id">
      <component :is="item.type" :children="item.children" />
    </div>
  </div>
</template>

<script>
import InputRadio from "./components/InputRadio";
import InputText from "./components/InputText";

export default {
  components: {
    InputText,
    InputRadio
  },
  data() {
    return {
      inputs: [
        {
          id: 1,
          type: "InputRadio",
          children: [{ name: "bozo" }, { name: "xuxa" }]
        },
        {
          id: 2,
          type: "InputText"
        }
      ]
    };
  }
};
</script>

<style>
</style>
