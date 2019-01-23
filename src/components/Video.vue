<template>
<v-container fluid grid-md-list fill-height>

<v-layout row wrap text-xs-center align-center>

<v-flex xs12>
  <Scrollama @step-enter="stepEnterHandler" :offset="0.5">
  	<v-flex xs12 pa-5>
		<span class="section-title">צפו בהדגמה</span>
		</v-flex>
    <div class="padding-box" ref="video" data-step="1">
    <div  class="video-box">
    
   <youtube :video-id="videoId" ref="youtube"  class="player" fitParent></youtube>
    </div>
    </div>
</Scrollama>
</v-flex>
</v-layout>
</v-container>
</template>

<script>
import 'intersection-observer'
import Scrollama from 'vue-scrollama'
export default {
  data() {
    return {
      videoId: 'qzNzVCQdF6E',
  
    }
  },
  components:{
      Scrollama
  },
  methods: {
   

    stepEnterHandler ({element, index, direction}) {
        const timeline = new TimelineLite() 
        const { video } = this.$refs;
        const x = index;
        switch(x){
            case 0:
               timeline.to(video, 2, { 
                y:-10,
                ease: Power2.easeOut,
                opacity:1,
                });
                break;
        }
    }
  },
  computed: {
    player() {
      return this.$refs.youtube.player
    }
  }
}
</script>

<style scoped>

.video-box{
    width:1000px;
  
    display:inline-block;
}
.padding-box{
    display:inline-block;
    padding:15px;
    border:#78b82196 solid 2px;
    opacity:0;
}
</style>