<template>
  <div class="container">
    <div v-for="(item, key) in children" :key="key">
      <input type="radio" name="oi" value="oi" />
      <label for="oi">{{ item.name }}</label>
    </div>
  </div>
</template>

<script>
export default {
  props: ["children"],
  created() {
    console.log(this.children);
  }
};
</script>

<style>
.container{
  display: flex;
}
</style>