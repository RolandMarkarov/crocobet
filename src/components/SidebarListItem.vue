<template>
    <p class='list-item' :class= '{active: item.isActive}' >
      <img :src="item.url" alt="" class='list-item--img'>
      <span class='list-item--text'>{{ item.title }}</span>
    </p>
</template>

<script>

import { ref, computed } from 'vue';
export default {
  props:{
    item: {type: Object}
  },
  setup () {
    const isActive = ref(false)
    const classObject = computed(()=>{

    })

    return {
      isActive,
      classObject,
      }
  }
}
</script>

<style lang="scss" scoped>

.list-item{
  padding: 15px;
  display: flex;
  justify-content: start;
  border-bottom: 1px solid #5c6f7523;
&:hover{
  background: #5c6f7523;
  cursor: pointer;
}

  &--img{
    margin-right: 20px;
  }
  
}

.active{
  position: relative;
  background: #fff;

  &::after{
  display: block;
  content: '';
  height: 100%;
  width: 2px;
  background: green;
  position: absolute;
  right: 0;
  top: 0;
  }
}
</style>