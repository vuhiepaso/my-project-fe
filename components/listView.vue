<template>
  <div>
    <div v-for="(item, index) in listData" :key="index">
      <slot name="item" :item="item" :index="index">
        <div class="item-default">1{{ index }}</div>
      </slot>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    listData: Array,
  },
};
</script>

<style scoped>
.item-default {
  padding: 15px;
  margin-bottom: 2px;
  background: #cccccc;
  color: gray;
  font-size: 20;
  font-weight: 900;
}
</style>
