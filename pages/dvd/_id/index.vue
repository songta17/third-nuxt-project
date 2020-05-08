<template>
  <h1>DVD avec params, methode numéro 2: {{ $route.params.id }}</h1>
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
