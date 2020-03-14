<template>
  <div class = "Banner">
    <div class="picface">
      <img src='https://image.flaticon.com/icons/svg/356/356779.svg' alt='...'>
    </div>
    <div class="title_name">
      台灣<br>空汙地圖</br>
    </div>
    <div class="time_btn">
      <div id='now_btn'><b>現況</b></div>
      <div id='predict_btn'><b>預報</b></div>
    </div>
  </div>

</template>


<style lang="sass">

html,body
  height: 100%
  width: 100%
  margin: 0

.Banner 
  width: 30%
  height: 8%
  margin-left:12%
  display: flex
  flex-direction:row
  // background: #f5da42


.picface
  width: 10%
  height: 80%
  margin-left: .5rem
  background-image:url('https://image.flaticon.com/icons/svg/356/356779.svg')
  // background: #eb3d34


img
  width: 100%
  height: 100%

.title_name
  width: 20%
  height: 80%
  margin-left: .2rem
  color: #2A3561
  // background:#ebb9b9
  font-size: 140%
  font-weight: bold
  text-align: left

.time_btn
  width: 50%
  height: 50%
  margin: 2%
  margin-top: 5%
  // background:#038cfc
  display: flex
  font-size: 125%
  color: #000000
  text-align: center

#now_btn
  width: 35%
  height: 100%
  // background: #c40000
  border: 2px solid #323333
  border-radius: 10px
  margin-left: 3%
  transition: .3s
  z-index:999
  &:hover
    background: #323333
    color:#ffff
    cursor: pointer
   
    
#predict_btn
  width: 35%
  height: 100%
  // background:#fce303
  border: 2px solid #323333
  border-radius: 10px
  margin-left: 5%
  z-index:999
  
  
  &:hover
    background: #323333
    color:#ffff
    cursor: pointer

.infor_btn
  width:30%
  height:30%

// @media (min-width: 576px) 


@media (min-width: 768px)

.Banner 
  width: 30%
  height: 10%
  margin-left:1rem
  margin-top:-3%
  display: flex
  flex-direction:row
  // background:#f5da42


.picface
  width: 15%
  height: 90%
  margin-left:-.5rem
  // background-image:url('https://image.flaticon.com/icons/svg/356/356779.svg')
  // background:#eb4034

img
  width:100%
  height: 100%

.title_name
  width: 30%
  height: 80%
  margin-left: .2rem
  color: #2A3561
  // background:#ebb9b9
  font-size: 100%
  font-weight: bold
  text-align: left

.time_btn
  width: 50%
  height: 50%
  margin: 2%
  margin-left:-1rem
  margin-top: 5%
  // background:#038cfc
  display: flex
  font-size: 100%
  color: #000000
  text-align: center

#now_btn
  width: 35%
  height: 92%
  // background: #c40000
  border: 2px solid #323333
  border-radius: 10px
  margin-left: 3%
  transition: .3s
  z-index:999

  &:hover
    background: #323333
    color:#ffff
    cursor: pointer
   
    
#predict_btn
  width: 35%
  height: 92%
  // background:#fce303
  border: 2px solid #323333
  border-radius: 10px
  margin-left: 5%
  z-index:999
  
  
  &:hover
    background: #323333
    color:#ffff
    cursor: pointer

.infor_btn
  width:30%
  height:30%


@media (min-width: 992px) 


@media (min-width: 1200px) 

</style>
