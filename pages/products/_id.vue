<template>
  <h1>Products: {{ $route.params.id }} </h1>
</template>
<script>
  export default {
    validate(data){
      // console.log(data)
      // return true

      // return data.params.id == 1

      return /^\d+$/.test(data.params.id)
  }
}
</script>


