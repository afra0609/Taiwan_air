<template>
  <div class="container">
    <div class="dropdown">
      <button class="dropdown_btn">環保署資訊</button>
      <div class="dropdown_menu">
        <a href="#">個測站資訊</a>
        <a href="#">IDW資訊</a>
      </div>
      <button class="dropdown_btn">Lass感測站</button>
      <div class="dropdown_menu">
        <a href="#">各感測器</a>
        <a href="#">空間內插</a>
      </div>
    </div>
  </div>
</template>





<style lang="sass">
@import url(https://fonts.googleapis.com/css?family=Righteous)

html,body
  height: 100%
  width: 100%
  margin: 0

.container 
  display: flex
  align-items: center
  height: 7vh
  width:60vh
  margin-top:-.3%
  margin-left:13%
  justify-content: center
  background:#f4fc03

.dropdown
  display: inline-block
  position: relative
  background:#fc036f
  

.dropdown_btn
  background: #18bc9c
  // display: inline-block
  font-family: Microsoft JhengHei 
  border: 0
  outline: none
  font-size: 18px
  text-transform: uppercase
  padding: 0 42px 0 15px
  margin:0 10px 0 10px
  border-radius: 10px
  color: #ffff
  letter-spacing: 1.5px
  line-height: 36px
  cursor: pointer
  border-bottom: 3px solid #128f76
  overflow: hidden
  position: relative

  &:before, &:after
    display: inline-block
    font: normal normal normal 14px/1 FontAwesome
    font-size: inherit
    text-rendering: auto
    -webkit-font-smoothing: antialiased
    -moz-osx-font-smoothing: grayscale
    transition: all 0.2s linear

  &:before
    content: "\f107"
    position: absolute
    right: 0
    top: 0
    display: block
    height: 45px
    width: 40px
    text-align: center
    line-height: 45px

  &:after
    content: "\f106"
    position: absolute
    right: 0
    top: -100%
    display: block
    height: 45px
    width: 40px
    text-align: center
    line-height: 45px

  &:hover
    &:before, &:after
      background: #15a589
      box-shadow: 2px 0 1px rgba(0, 0, 0, 0.05) inset
      
  &:focus
    &:before
      background: #15a589
      box-shadow: 2px 0 1px rgba(0, 0, 0, 0.05) inset
      top: 100%

    &:after
      background: #15a589
      box-shadow: 2px 0 1px rgba(0, 0, 0, 0.05) inset
      top: 0%

.dropdown_menu
  pointer-events: none
  background: #128f76
  position: absolute
  width: 45%
  top: 40px
  left: -100px
  opacity: 0
  transition: all 0.5s ease-in-out
  border-radius: 10px

  a
    display: block
    line-height: 45px
    padding:0 15px
    text-decoration: none
    color: #fff
    letter-spacing: 2px
    transition: all 0.2s linear
    overflow: hidden
    border-bottom: 1px solid #0f7864
  
    &:first-child
      border-radius: 10px 10px 0 0

    &:last-child
      border-bottom: 0
      border-radius: 0 0 10px 10px

    &:hover
      box-shadow: 3px 3px 8px rgba(0, 0, 0, 0.16) inset
      background: #18bc9c

.dropdown .dropdown_btn:focus + .dropdown_menu
  left: 0
  opacity: 1
  pointer-events: inherit

  &:hover
    left: 0
    opacity: 1
    pointer-events: inherit

</style>