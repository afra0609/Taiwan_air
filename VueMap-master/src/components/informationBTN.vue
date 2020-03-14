<template>
  <div class="container">
    <div class="dropdown">
      <button class="dropdown_btn">環保署資訊</button>
      <div class="dropdown_menu">
        <a href="#">個測站資訊</a>
        <a href="#">IDW資訊</a>
      </div>
    </div>                      

    <div class="dropdown">
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
@import url(https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css)

html,body
  height: 100%
  width: 100%
  margin: 0

.container 
  display: flex
  align-items: center
  height: 7vh
  width: 60vh
  margin-top: -2%
  margin-left:.5rem
  justify-content: center
  // background: #fca589


.dropdown
  display: inline-block
  position: relative
  margin: 0 10px 0 10px

  

.dropdown_btn
  font-weight: bold
  background: #FFFFFF
  font-family: Microsoft JhengHei 
  border: 1.5px solid #323333 
  outline: none
  font-size: 18px
  text-transform: uppercase
  padding: 0 42px 0 15px
  border-radius: 10px
  color:#323333
  letter-spacing: 1.5px
  line-height: 36px
  cursor: pointer
  border-bottom: 3px solid #323333
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
      background: #323333
      box-shadow: 2px 0 1px rgba(0, 0, 0, 0.05) inset
      
  &:focus
    &:before
      background: #323333
      box-shadow: 2px 0 1px rgba(0, 0, 0, 0.05) inset
      top: 100%

    &:after
      background: #323333
      box-shadow: 2px 0 1px rgba(0, 0, 0, 0.05) inset
      top: 0%

.dropdown_menu
  pointer-events: none
  background: #CCCCCC
  position: absolute
  width: 100%
  top: 40px
  left: -100px
  opacity: 0
  transition: all 0.5s ease-in-out
  border-radius: 10px


  a
    display: block
    line-height: 40px
    padding: 0 15px
    text-decoration: none
    color: #323333
    letter-spacing: 2px
    transition: all 0.2s linear
    overflow: hidden
    border-bottom: 1px solid #323333
    font-size:18px
   
    &:first-child
      border-radius: 10px 10px 0 0

    &:last-child
      border-bottom: 0
      border-radius: 0 0 10px 10px

    &:hover
      box-shadow: 3px 3px 8px rgba(0, 0, 0, 0.16) inset
      background: #323333
      color:#FFFFFF

.dropdown .dropdown_btn:focus + .dropdown_menu
  left: 0
  opacity: 1
  pointer-events: inherit

  &:hover
    left: 0
    opacity: 1
    pointer-events: inherit

@media (min-width: 576px) 


@media (min-width: 768px)

.dropdown
  display: inline-block
  position: relative
  margin: -8px 5.2px 0 10px
  

.dropdown_btn
  font-weight: bold
  background: #FFFFFF
  font-family: Microsoft JhengHei 
  border: 1.5px solid #323333 
  outline: none
  font-size: 14px
  text-transform: uppercase
  padding: 0 40px 0 15px
  border-radius: 10px
  color: #323333
  letter-spacing: 0.5px
  line-height: 24px
  cursor: pointer
  border-bottom: 2px solid #323333
  overflow: hidden
  position: relative
  margin-top: 36%

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
    line-height: 60px
     

  &:after
    content: "\f106"
    position: absolute
    right: 0
    top: -40%
    display: block
    height: 48px
    width: 40px
    text-align: center
    line-height: 45px
    
.dropdown_menu
  pointer-events: none
  background: #CCCCCC
  position: absolute
  width: 100%
  top: 75px
  left: -100px
  opacity: 0
  transition: all 0.5s ease-in-out
  border-radius: 6px

  a
      display: block
      line-height: 24px
      padding: 0 15px
      text-decoration: none
      color: #323333
      letter-spacing: 1px
      transition: all 0.2s linear
      overflow: hidden
      border-bottom: 1px solid #323333
      font-size: 14px
    
      &:first-child
        border-radius: 10px 10px 0 0

      &:last-child
        border-bottom: 0
        border-radius: 0 0 10px 10px

      &:hover
        box-shadow: 3px 3px 8px rgba(0, 0, 0, 0.16) inset
        background: #323333
        color:#FFFFFF


@media (min-width: 992px) 


@media (min-width: 1200px) 

</style>