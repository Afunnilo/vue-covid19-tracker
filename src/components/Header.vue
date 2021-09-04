<template>
  <header class="text-center bg-purple-700 text-white p-4 mb-10">
    <div class="text-3xl md:text-5xl font-bold mb-3"><i class = "fa fa-virus"></i>Covid-19 Tracker</div>
    <p> API from <a class="text-300 plum" href="https://covid19api.com" target="_blank">covid19api.com</a></p>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>

a{
  color:plum
}
i{
  padding-right: 10px;
}
</style>
