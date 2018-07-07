<template>
  <div class="label-with-value">
    <div class="label">{{label}}</div>
    <div v-if="!isLink" class="value">{{value}}</div>
    <a class="value" v-else :href="value">{{value}}</a>
  </div>
</template>
<script>
export default {
  name: 'LabelWithValue',
  props: {
    label: {
      type: String,
      default: 'label'
    },
    value: {
      type: String,
      default: 'value'
    },
    isLink: {
      type: Boolean,
      default: false
    }
  }
}
</script>
<style scoped>
  .label-with-value{
    width: 100%;
    padding: 5px 0px;
  }
  .label-with-value .label{
    width: 15%;
    text-align: right;
    display: inline-block;
  }
  .label-with-value .label::after{
    content: ":";
    margin-left: 3px;
  }
  .label-with-value .value{
    width: 80%;
    text-align: left;
    font-weight: bold;
    display: inline-block;
    padding-left: 10px;
  }
</style>
