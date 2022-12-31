<script>
export default {
  name: "toolCard",
  props:{
    toolName:String,
    dist: String,
    description: String,
    isSelected: Boolean
  }
}


</script>
<template>
  <div class="toolcard">
    <div class="toolcard-content">
      <p>{{toolName}}</p>
      <p>{{description}}</p>
      <p>{{dist}}</p>
    </div>
  </div>
</template>

<style scoped>

</style>