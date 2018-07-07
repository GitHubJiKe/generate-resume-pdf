<template>
  <div class="level-title">
    <h1 v-if="level == 1">{{content}}</h1>
    <h2 v-if="level == 2">{{content}}</h2>
    <h3 v-if="level == 3">{{content}}</h3>
    <h4 v-if="level == 4">{{content}}</h4>
    <h5 v-if="level == 5">{{content}}</h5>
    <h6 v-if="level == 6">{{content}}</h6>
  </div>
</template>

<script>
export default {
  name: 'LevelTitle',
  props: {
    level: {
      type: String,
      default: '1'
    },
    content: {
      type: String,
      default: 'title content'
    }
  }
}
</script>
<style scoped>
  .level-title{
    width: 100%;
  }
  .level-title >h1,h2,h3,h4,h5,h6{
    text-align: left;
    padding-left: 10px;
    padding-bottom: 5px;
    font-weight: bolder;
  }
</style>
