<template>
  <div class = "colorboard">
    <div class= "type_name">PM2.5</div>
    <div class= "colorpic">
      <img src="@/assets/colorrr.jpg">
    </div>

  </div>
</template>



<style lang="sass">

html,body
  height: 100%
  width: 100%
  margin: 0

@media (min-width: 768px)

.colorboard
  width: 36%
  height: 9%
  // background: #eb4034
  margin-top: -5%
  display: flex
  border: .5px solid #2A3561
  margin-left: 2.5%
  border-radius: 6px
  z-index: 999



img
  width: 100%
  height: 100%


.type_name
  width: 12%
  height: 70%
  // background: #f5b8c9
  margin-top: 3.2%
  margin-left: 2%



.colorpic
  width: 83%
  height: 85%
  // background: #f5b8c9
  margin-top: .5%
  margin-left: .8%







</style>
