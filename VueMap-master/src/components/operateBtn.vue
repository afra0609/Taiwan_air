<template>
  <div class = 'operateBtn'>
    <div class = 'btn_container' @click="turn_back">
      <div class = 'btn_imag'>
        <img src ='https://image.flaticon.com/icons/svg/137/137531.svg' alt=''>
      </div>
      <div class = 'btn_txt'><b>回前頁</b>
      </div>
    </div>
    <div class = 'btn_container'>
      <div class = 'btn_imag'>
        <img src ='https://image.flaticon.com/icons/svg/760/760669.svg' alt=''>
      </div>
      <div class = 'btn_txt'><b>使用說明</b>
      </div>
    </div>
  </div>
</template>

<script>
import closemap from "../App"

export default {
  methods: {
    turn_back() {

      this.$parent.closemap();
      console.log("click");
      console.log(name);
    }
  }
}
</script>

<style lang="sass">

html,body
  height: 100%
  width: 100%
  margin: 0

@media (min-width: 768px)

.operateBtn
  height: 15%
  width: 9.5%
  // background: #fcf403
  margin-top: 1%
  margin-left: 22%
  padding: 4px .5px .5px 4px
  



.btn_container
  height: 42%
  width: 98%
  // background: #1303fc
  margin-top: 2.8%
  border: .6px solid #2A3561
  border-radius: 10px
  display: flex
  position: relative
  z-index: 9999
  transition: .3s

  &:hover
      width: 110%
      cursor: pointer
    




.btn_txt
  height: 99%
  width: 65%
  // background: #51f542
  font-size: 1rem
  text-align: center
  line-height: 200%

.btn_imag
  height: 92%
  width: 35%
  // background: #ebd8f2

 

img
  width: 100%
  height: 100%



 
  

</style>
