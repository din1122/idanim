<template>
<v-container fluid grid-list-xs pa-0>
    <v-layout row wrap justify-start fill-height align-end>
    <v-flex  xs12 class="main-pic-m elevation-4">

    </v-flex>

            <v-flex xs12 xl4 md4 text-xs-center >
            <v-flex npm3 xs12>
                <span class="main-title">קבוצת</span>
                   <img class="logo-home" :src="require('@/assets/trans.png')">
                <div class="fade-bg mt-3">
                <span class="display-1">אנחנו תמיד משתדלים יותר</span>
                </div>
            </v-flex>
            <v-flex xs12 pt-5 >
            <v-layout row fill-height align-end justify-space-around >
            
            <v-flex xs3 class="blue-box npm" pa-3 elevation-2 v-for="item in texts" > 
           <v-layout row wrap justify-end fill-height> 
            <v-flex xs12   class="icon-box" text-xs-center>
            <span class="banner-number">{{item.number}}</span>
            </v-flex>
            <v-flex xs12>
            <v-divider dark></v-divider>
            </v-flex>
            <v-flex xs12 display-1 text-xl-right text-xs-center  white--text class="stats-text">
            <span class="font-weight-bold">{{item.title}}</span><br>
            <span class="font-weight-thin">{{item.subtitle}}</span>
            </v-flex>
            </v-layout>
            </v-flex>
            </v-layout>
            </v-flex>
            </v-flex>
            <v-flex  xs8 class="main-pic elevation-4">
            </v-flex>

          
    </v-layout>

    
</v-container>
</template>

<script>
export default {
    data(){
        return{
            items:[
                {imgsrc:'stats.png', title:'מקצועיות', subtitle:'מומחים'},
                {imgsrc:'id.png', title:'אמינות', subtitle:'ישרים'},
                {imgsrc:'medal.png', title:'מסירות', subtitle:'מבטיחים'}
            ],
            texts:[
                {title:'שנות', subtitle:'ניסיון', number:'25'},
                {title:'עובדים', subtitle:'בחברה', number:'308'},
                {title:'לקוחות', subtitle:'מרוצים', number:'2054'},
             
            ]
        }
    }
}
</script>
<style scoped>

.banner-number{
    color:white;
    font-size:3em 
}

.main-pic{
background-image: url("../assets/main.jpg"); /* The image used */
  background-color: #cccccc; /* Used if the image is unavailable */
    height: 75vh;
    background-position: center 40%;
    background-repeat: no-repeat;
    background-size: cover;
}
.float-box{
    position: absolute; 
    left: 50%; 
     top: 50%;
}
.float-text{
  border-radius:10px;
  height:200px;
  width:400px;
  padding:15px;
  background:#fff;
}
.main-title{
    padding-left:4%;
    font-size: 75px;
    line-height: 1.35;
}

.blue-box{
    background:#7AA7D7;
    height:228px;
}
.icon-img{
    float: left;
    width: 50%;
}

</style>