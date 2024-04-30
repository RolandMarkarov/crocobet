<template>
    <h1>
      <img src="@/assets/icons/cblogo.png" alt="Crocobet-Logo" class='logo-image'>
      <a href="https:crocobet.com" target='_blank'>
        <img src="@/assets/icons/arrow.png" alt="">
        crocobet.com
      </a>
    </h1>
</template>
<script>
export default {
  setup () {
    

    return {}
  }
}
</script>

<style lang="scss" scoped>
h1{
  padding: 60px;
  width: 100%;
  text-align: center;
}
.logo-image{
  width: 86px;
  height: auto;
  margin: auto;
  display: block; }
a{
  height: 32px;
  width: 145px;
  margin: 20px auto;
  padding:0 18px;
  align-items: center;
  display: block;
  font-size: 12px;
  border-radius: 100px;
  background: #0E9F6E;
  color: #F3F6F7;
  line-height: 32px;

}

</style>