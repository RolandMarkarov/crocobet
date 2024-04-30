<template>
  <div class='main-wrapper'>
    <Sidebar/>
  </div>
</template>

<script>
import Sidebar from './Sidebar.vue'
export default {
  components: { Sidebar },
  setup () {
    

    return {}
  }
}
</script>

<style lang="scss" scoped>
.main-wrapper{
  background-color: #ccc
}
</style>