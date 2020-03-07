<template>
  <div class='Bigboard'>
    <div class='board'>
      <div class='weather'><b>·現在天氣·</b>
      </div>
      <div class='digitboard'>
        <div class='temp_title'>溫度</div>
        <div class='temp_title'>體感溫度</div>
        <div class='temp'>27.5</div>
        <hr class= 'theline' width=".5" size="25" color="#323333">
        <div class='temp'>28</div>
      </div>
      <div class='detailboard'>
        <table>
          <tr>
            <th>濕度</th>
            <th>雨量</th>
            <th>紫外線</th>
            <th>平均風</th>
          </tr>
          <tr>
            <th>49</th>
            <th>0</th>
            <th>4</th>
            <th>1.6</th>
          </tr>
          <tr class = 'unit'>
            <th>%</th>
            <th>mm</th>
            <th>中量</th>
            <th>m/s</th>
          </tr>
        </table>
      </div>
    </div>
    
    <div class='board'>
      <div class='region'>
        <div class='icon'>
          <img src ='https://image.flaticon.com/icons/svg/365/365229.svg' alt=''>
        </div>
        <div class='content'>
          <div class='today_title'>·今天白天·</div>
          <div class='figure'>24°~27°</div>
          <div class='describle'>多雲時晴</div>
        </div>
      </div>
      <div class='region'>
      <div class='icon'>
          <img src ='https://image.flaticon.com/icons/svg/2413/2413547.svg' alt=''>
      </div>
        <div class='content'>
          <div class='today_title'>·今天晚上·</div>
          <div class='figure'>18°~23°</div>
          <div class='describle'>晴時多雲</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="sass">

html,body
  height: 100%
  width: 100%
  margin: 0

.Bigboard
  width: 30%
  height: 50%
  // background: #f9e1d5
  margin-top: 5%
  margin-left: .5rem
  justify-content: center

.board
  width: 60%
  height: 49%
  // background: #abd2ff
  margin: .5%
  margin-left: 12%

.weather
  width: 45%
  height: 10%
  // background: #c9abc8
  margin-left: 28%
  margin-top: 20px
  font-size: 14px
  z-index: 9999


.digitboard

  width: 78%
  height: 40%
  // background: #c9abc8
  margin-left: 11%
  margin-top: 2%
  display: flex



.detailboard
  width: 78%
  height: 40%
  // background: #c9abc8
  margin-left: 11%
  margin-top: 2%



img
  width: 100%
  height: 100%

// @media (min-width: 576px) 


@media (min-width: 768px)

.Bigboard
  width: 40%
  height: 68%
  // background: #f9e1d5
  margin-top: 5.6%
  margin-left: .5rem
  justify-content: center
 

.board
  width: 45%
  height: 40%
  // background: #cccc
  margin-left: 5%
  text-align: center
  border: .6px solid #2A3561
  border-radius: 10px


.weather
  width: 40%
  height: 10%
  // background: #c9abc8
  margin-left: 29%
  margin-top: 1.8%
  font-size: 16px
  color: #1F5984
  text-align: center


.digitboard
  display: flex
  flex-wrap: wrap
  width: 90%
  height: 40%
  font-weight: bold
  // background: #9c3273
  margin-left: 5%
  margin-top: 3%



.temp_title
  text-align: center
  width: 35%
  height: 30%
  font-size: 14px
  // background: #c7ffeb
  margin: 7%
  margin-top: 1.8%

  


.temp
  width: 28%
  height: 60%
  margin: 10%
  margin-top: -4%
  // background: #5a57ff
  font-size: 20px

hr
  margin-top: -2%


.detailboard
  width: 90%
  height: 40%
  // background: #c9abc8
  margin-left: 2.8%
  margin-top: 1.5%
  font-size: 12px

table
  width: 180px

.unit
  font-size: 8px

.region
  width: 90%
  height: 48%
  // background: #f5cee4
  margin-top: .5%
  margin-left: 5%
  display: flex

.icon
  width: 28%
  height: 68%
  // background: #529fe3
  margin-top: 12% 

.content
  width: 60%
  height: 100%
  // background: #9a52e3
  margin: .8%


.today_title
  width: 100%
  height: 28%
  // background: #e6eef5
  font-size: 16px
  margin-left: -.5%
  font-weight: bold
  text-align: left
  color: #1F5984

.figure
  width: 100%
  height: 46%
  // background: #e6eef5
  margin: 1%
  font-size: 20px
  font-weight: bold
  text-align: center
  line-height: 155%

.describle
  width: 100%
  height: 20%
  // background: #e6eef5
  margin: 1%
  font-size: 10px
  font-weight: bold


@media (min-width: 992px) 


@media (min-width: 1200px) 


</style>