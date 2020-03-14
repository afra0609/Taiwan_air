<template>
  <div class= "localboard" >
    <div class= "datetime">
      <div id="clock" class="clock">loading ...
      </div>
    </div>
    <div class= "blackline">
    </div>
    <div class= "localname">
    </div>
    <div class= "pm_num">PM2.5指數
    </div>
    <div class= "vision_num">

      <div class="ia-radial red">
        <svg viewBox="0 0 100 100">
          <circle r="4" cx="50" cy="50" id="pie" />
        </svg>
        <div id="precent">93</div>
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

@media (min-width: 768px)


.localboard
  width: 18%
  height: 55%
  // background: #fa0068
  margin-top: -38.5%
  margin-left: 70%
  padding: 0 .2% .2% 0
  border: 1px solid #323333 
  border-radius: 8px


.datetime
  width: 100%
  height: 12%
  background: #ffe0d
  margin: .5%



.blackline
  width: 100%
  height: 2%
  background: #ffe0ed
  margin: .5%
  margin-top: 10%
  border: 0
  height: 1.5px
  background-image: linear-gradient(to right, #ccc, #323333, #ccc)


.localname
  width: 100%
  height: 15%
  // background: #ffe0ed
  margin: .5%



.pm_num
  width: 100%
  height: 14%
  // background: #ffe0ed
  margin: .5%
  font-size: 1.3rem
  margin-top: 3%



.vision_num
  width: 100%
  height: 45%
  // background: #ffe0ed
  margin-top: -28%
  margin-left: -6%

.clock 
  height: 98%
  width: 98%
  line-height: 28px 
  margin-left: 1%
  margin-bottom: -1% 
  // background: #222
  color: #323333
  text-align: center


.ia-radial
  width: 200px
  position: relative
  display: inline-block
  margin-bottom: 20px
  text-align: center
  color: #777

  svg
    transform: rotate(-90deg)
    border-radius: 50%

    #pie
      fill: currentcolor
      stroke-width: 50
      stroke-dasharray: 0 158
      transition: stroke-dasharray 2s
      stroke: #777

  #precent
    position: absolute
    top: 49%
    left: 50%
    transform: translate(-50%, -50%)
    background: #fff
    width: 85px
    height: 85px
    line-height: 80px
    border-radius: 50%
    font-size: 2em
    font-weight: bold

    // &:after
    //   content: '%'

// .center
//   position: absolute
//   top: 10%
//   transform: translateY(-50%)
//   text-align: center
//   width: 100%
//   font-family: verdana

.ia-radial
  margin: 20px

  &.red
    color: #fd5b4e

    #pie
      stroke: #fd5b4e

  &.green
    color: #5BC89E

    #pie
      stroke: #5BC89E


</style>
