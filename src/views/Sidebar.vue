<template>
  <div class='sidebar-wrapper'>
    <HeaderLogo/>
  </div>
</template>


<script>
import HeaderLogo from "@/components/HeaderLogo.vue"

export default {
  components: {
    HeaderLogo
  }
}
</script>
<style scoped>
.sidebar-wrapper {
  width: 321px;
  height: 100vh;
  border-radius:0px 24px 24px 0px ;
  background-color: #fff;
}
</style>