<template>
  <div class="wrapper">
    <sidebar/>
  </div>
</template>

<script>
import Sidebar from './Sidebar.vue'

export default {
  components: {Sidebar},
  setup() {


    return {}
  }
}
</script>

<style lang="scss" scoped>
.wrapper {
  background: #DFE5E7;

}

</style>