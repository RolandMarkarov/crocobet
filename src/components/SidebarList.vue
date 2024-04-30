<template>
    <SidebarListItem  v-for="item in listArray" :key="item.id" :item='item' @click='toggleActive(item.id)'/>
</template>

<script>
import { ref, computed } from 'vue';
import SidebarListItem from "./SidebarListItem.vue";
export default {
  components: { SidebarListItem },
  setup () {

    const listArray = ref([
      {id: 1, title: 'კონტენტი', url: '/src/assets/icons/content.png', isActive:false},
      {id: 2, title: 'პარამეტრები', url: '/src/assets/icons/params.png', isActive:false},
      {id: 3, title: 'ადმინები', url: '/src/assets/icons/profile-2user.png', isActive:false},
      {id: 4, title: 'ლიდერბორდი', url: '/src/assets/icons/cup.png', isActive:false},
      {id: 5, title: 'კალენდარი', url: '/src/assets/icons/calendar.png', isActive:false},
      {id: 6, title: 'პარტნიორები', url: '/src/assets/icons/people.png', isActive:false},
      {id: 7, title: 'ფოტო გალერეა', url: '/src/assets/icons/gallery.png', isActive:false},
      {id: 8, title: 'ვიდეო გალერეა', url: '/src/assets/icons/video-square.png', isActive:false},
      {id: 9, title: 'სლაიდერი', url: '/src/assets/icons/slider.png', isActive:false},
      {id: 10, title: 'სიახლეები', url: '/src/assets/icons/flash.png', isActive:false},
      {id: 11, title: 'მენიუ', url: '/src/assets/icons/dots.png', isActive:false},
    ])
    function toggleActive(id){
      listArray.value.forEach(el => {if (el.id === id){
        el.isActive= true
      } else {
        el.isActive = false
      }})
    }
    return {
      listArray,
      toggleActive
    }
  }
}
</script>

<style lang="scss" scoped>

</style>