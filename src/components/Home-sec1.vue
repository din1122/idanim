<template>
<div>
   <v-layout row wrap>
    <v-flex text-xs-center>
    <div class="img-container" ref="img">
     </div>
    </v-flex>
    <div class="floating-text-1" ref="Txtone">
    <span class="float-title body-2">Main title</span><br>
    <v-flex xs4>
    <span class="float-text">Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem</span>
   </v-flex>
    </div>
<div class="text-line">
<svg height='500' width='500' class="top-right-svg" ref="svg1">
 <path  d="M 50 350 Q 150 200 200 100 L 450 100 " data-reactid=".0.0.0.0.1"></path>
 <g data-v-a83bd3b0="" data-reactid=".0.0.0.0.2.2" class="ad-PointGroup  is-active">
<circle data-v-a83bd3b0="" cx="450" cy="100" r="8" data-reactid=".0.0.0.0.2.2.0" class="ad-Point"></circle>
</g>
</svg>
 <svg height='500' width='500' class="top-left-svg" ref="svg2">
 <path d="M 50 100 Q 150 100 350 100 L 500 250 " data-reactid=".0.0.0.0.1"></path>
 <g class="ad-PointGroup  is-active" data-reactid=".0.0.0.0.2.2">
 <circle class="ad-Point" cx="50" cy="100" r="8" data-reactid=".0.0.0.0.2.2.0"></circle></g>
</svg>
   <div class="green-circle">
   </div>
   </div>
    <div class="floating-text-2 ma-0" ref="TxtTwo">
    <span class="float-title body-2">Main title</span><br>
    <v-flex xs6>
    <span class="float-text">Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem</span>
   </v-flex>
    </div>
    <div class="floating-text-3" ref="TxtThree">
    <span class="float-title body-2">Main title</span><br>
    <v-flex xs4>
    <span class="float-text">Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem</span>
   </v-flex>
    </div>
<svg height='500' width='600' class="bottom-right-svg" ref="svg3">
 <path  d="M 50 100 L 250 300 L 450 300  " data-reactid=".0.0.0.0.1"></path>
<g data-v-a83bd3b0="" data-reactid=".0.0.0.0.2.2" class="ad-PointGroup  is-active">
<circle data-v-a83bd3b0="" cx="450" cy="300" r="8" data-reactid=".0.0.0.0.2.2.0" class="ad-Point"></circle>
</g></svg>
</svg>
<svg data-v-a83bd3b0="" height="600" width="500" class="bottom-left-svg" ref="svg4">
<path data-v-a83bd3b0="" d="M 50 300 L 250 300 L 440 150 " data-reactid=".0.0.0.0.1"></path>
<g data-v-a83bd3b0="" data-reactid=".0.0.0.0.2.2" class="ad-PointGroup  is-active">
<circle data-v-a83bd3b0="" cx="50" cy="300" r="8" data-reactid=".0.0.0.0.2.2.0" class="ad-Point"></circle>
</g></svg>
    <div class="floating-text-4" ref="TxtFour">
    <span class="float-title body-2">Main title</span><br>
    <v-flex xs4>
    <span class="float-text">Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse sed nibh faucibus, hendrerit massa sed, mollis nisl. In interdum volutpat lorem</span>
   </v-flex>
    </div>
   </v-layout>
   <Mhome />
</div>
</template>
<script>
import Mhome from '@/components/Mhome'
import { TimelineLite } from 'gsap'
export default {
    data(){
        return{
            
        }
    },
    components:{
        Mhome
    },
    mounted(){
         const { svg1 } = this.$refs
         const { svg2 } = this.$refs
         const { svg3 } = this.$refs
         const { svg4 } = this.$refs
         const { img } = this.$refs
         const { Txtone } = this.$refs
         const { TxtTwo } = this.$refs
         const { TxtThree } = this.$refs
         const { TxtFour } = this.$refs
        const timeline = new TimelineLite() 

        timeline.to([img], 1, { 
            ease: Power0.easeNone,
            opacity:1,
            delay:0.5,
        });
        timeline.to([Txtone,TxtFour], 1, { 
            x:-10,
            ease: Power0.easeNone,
            opacity:1,
           
        });
        timeline.to([TxtTwo,TxtThree], 1, { 
            x:10,
            ease: Power0.easeNone,
            opacity:1,
            delay:-1,
           
        }); 
        timeline.to([svg2,svg1,svg3,svg4], 1,{ 
            opacity:1,
                }
        ); 


    }
}
</script>
<style scoped>
.ad-Point:hover, .ad-PointGroup.is-active .ad-Point {
    fill: #78B821;
   stroke: white;
}
.ad-point{
   cursor: pointer;
    fill: #fff;
    stroke: #555;
    stroke-width: 5px;
    -webkit-transition: fill .2s;
    transition: fill .2s;
}
.top-left-svg{
   position: absolute;
   top: 11vh;
   left: 33vh;
   opacity:0;
}
.top-right-svg{
    position: absolute;
    top: 1vh;
   right: 36vh;
   opacity:0;
}
.bottom-left-svg{
    position: absolute;
   top: 38vh;
    left: 38vh;
    opacity:0;
}
.bottom-right-svg{
        position: absolute;
    top: 42vh;
    right: 27vh;
    opacity:0;
}
.home-1{
   border-radius:50%;
   height:588px;
    width:588px;
   border: solid 2px #78B821;
   padding:10px;
 
}
.img-container{
  margin-top: 100px;
  padding:10px;
opacity:0;
}
.floating-text-1{
    opacity:0;
    z-index: 1;
    position: absolute;
    left: 38vh;
    top: 24vh;
    transform: matrix(1, 0, 0, 1, -450, 0);
}
.floating-text-2{
    opacity:0;
   z-index: 1;
    position: absolute;
left: 68%;
    top: 13vh;
      transform: matrix(1, 0, 0, 1, 450, 0);
}
.floating-text-3{
    opacity:0;
   z-index: 1;
    position: absolute;
  right: -41vh;
    top: 75vh;
      transform: matrix(1, 0, 0, 1, 450, 0);
}
.floating-text-4{
    opacity:0;
   z-index: 1;
    position: absolute;
        left: 45vh;
    top: 73vh;
      transform: matrix(1, 0, 0, 1, -450, 0);
}
path {
    stroke: #cdcdcd;;
    stroke-width: 4px;
    fill: none;
}
</style>
