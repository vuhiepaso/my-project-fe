<template>
  <div>
    <h3>{{ dataItem.name }}</h3>
    <p>{{ dataItem.content }}</p>
  </div>
</template>

<script>
export default {
  props: {
    dataItem: {},
  },
};
</script>
