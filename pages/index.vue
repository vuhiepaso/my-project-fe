<template>
  <div>
    <listView :listData="listData">
      <template #item="{ item }">
        <itemStudent :dataItem="item"></itemStudent>
      </template>
    </listView>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      listData: [
        {
          id: "1",
          name: "hiep1",
          content: "minh la hiep",
        },
        {
          id: "2",
          name: "hiep2",
        },
        {
          id: "3",
          name: "hiep3",
        },
      ],
    };
  },
};
</script>
