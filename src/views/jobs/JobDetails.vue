<template>
  <h1>Job Details</h1>
  <p>The id for this Job Details page is: {{ id }}</p>
</template>


<script>
  export default {
    data() {
      return {
        id: this.$route.params.id
      }
    }
  }
</script>


<style>

</style>