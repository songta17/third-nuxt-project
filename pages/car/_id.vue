<template>
  <h1>Car with params: id: {{ $route.params.id }}</h1>
</template>
<script>
  export default {
    validate(data) {
      // console.log(data)
      // return true

      //return data.params.id === 1 // est strictement identique alors affiché
      //return data.params.id == 1 // est égal alors affiché

      // on peut mettre un regex
      return /^\d+$/.test(data.params.id)

    }
  }
</script>
