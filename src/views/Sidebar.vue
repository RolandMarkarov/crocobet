<template>
  <div class='sidebar-wrapper'>
    <HeaderLogo/>
    <SidebarList/>
    </div>
</template>




<script>
import SidebarList from "@/components/SidebarList.vue";
import HeaderLogo from "@/components/HeaderLogo.vue"
  export default {
    components:{HeaderLogo, SidebarList },
  }
</script>
<style lang="scss">
.sidebar-wrapper{
  width: 321px;
  height: 100vh;
  border-radius: 20px, 0;
  background: #F3F6F7;

}
</style>