<template>
  <el-form-item :label="label">
    <el-input :type="type" v-model="ruleForm.pass" show-password></el-input>
  </el-form-item>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: "label",
    },
    type: {
      type: String,
      default: "text",
    },
  },
};
</script>

<style></style>
