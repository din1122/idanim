<template>
<v-container grid-list-md grid-list-xl grid-list-xs fluid>
<Scrollama @step-enter="stepEnterHandler">
<v-layout row wrap>



<v-flex xs12 xl3 md4 offset-md1 offset-xs0 offset-xl1  data-step="2"  ref="rightbox" class="right-section m-pt-5 m-pb-5">
    <v-card >
    <v-card-title class="white--text">מנהלים</v-card-title>
    <v-card-text >
    <v-layout align-center >
    <v-flex>
        <v-layout row wrap>   
        <v-flex xs12 pa-3>
                    <img :src="require('@/assets/buiss.png')" alt="home-1-idanim" class="Profile-img">
                      <v-flex xs12 class="text-xs-right">
                        <span class="body-2 underline">נועם אשכנזי</span><br>
                        <p>
                        בעלים ומנכ"ל הקבוצה,<br>
                        נועם צבר נסיון רב בכל הקשור לתחום נקיון כבישים ומדרכות, נחשב לאחד המומחים בתחום רכבי הטיאוט
                        מכל הסוגים.
                    </p>
            </v-flex>
        </v-flex>   
          
        </v-layout>
    </v-flex>

    </v-layout>
    </v-card-text>
    </v-card>
</v-flex>

<v-flex xs12 xl7 md7 ref="leftbox" data-step="1">
<v-card class="left-card">
<v-card-text>
<div class="pb-4"><span class="display-2 about-title"> עלינו</span></div>
    <p>חברת עידנים עבודות ציבוריות בע"מ נוסדה ע"י נועם אשכנזי לפני כ 25 שנים.
במשך כל השנים מאז הקמתה עסקה החברה במתן שירותי טיאוט כבישים ומדרכות לעיריות שונות כגון,  ראשון לציון, נס ציונה, יהוד, סביון, תל אביב ועוד, וכל זאת באמצעות מטאטאי כביש מסוגים שונים ומאות עובדים מסורים. 
חברת עידנים תשתיות בע"מ היא היבואן המורשה והבלעדי של חברת "טיסאן" www.tisan.eu  המייצרת מטאטאי כבישים בגדלים שונים, מכונות קרצוף ושטיפה בלחץ של כבישים ומדרכות, מכונות שטיפה של פחי אשפה ועוד. 
 וכן של חברת קדמה www.kademe.com.tr  המייצרת מכונות טיאוט ומתקני טיאוט המורכבים על משאיות בנפחים שונים, כן מייצרת החברה משאיות לפינוי אשפה, טרקטורים ומכונות שטיפה וקרצוף. 
עידנים תשתיות בע"מ עוסקת מזה מספר שנים ביבוא של מטאטאי כביש יעודיים בנפח של החל מ 1 מ"ק עד 5 מ"ק.
וגם מתקני טיאוט המורכבים על משאיות מסוגים שונים, בנפח של החל מ 4 מ"ק ועד 8 מ"ק.
כמו כן מייבאת החברה עגלות ניקיון המשמשות את עובדי הנקיון לניקוי הרחובות ואביזרים שונים הקשורים לתחום ניקוי כבישים ומדרכות.
</p>
</v-card-text>
</v-card>
</v-flex>




</v-layout>
</Scrollama>
</v-container>
</template>

<script>
import 'intersection-observer'
import Scrollama from 'vue-scrollama'
export default {
  data() {
    return {
  
    }
  },
  components:{
      Scrollama
  },
  methods: {
    stepEnterHandler ({element, index, direction}) {
        const timeline = new TimelineLite() 
        const { leftbox } = this.$refs;
        const { rightbox } = this.$refs;
        const x = index;
        switch(x){
            case 0:
               timeline.to(leftbox, 2, { 
               
                ease: Power2.easeOut,
                opacity:1,
                });
                timeline.to(rightbox, 2, { 
                ease: Power2.easeNone,
                opacity:1,
                delay:-1.5
                });
                break;
             
         
               
        }
    }
  },
}
</script>


<style scoped>

.v-card__title{
background: #78b821;
}
.Profile-img{
     width: 100%;
     height:40%;
    object-fit:cover;
}
.left-section{
    border:solid 1px #A3D855;
    background:white;
    -webkit-box-shadow: 0px 2px 1px -1px rgba(0,0,0,0.2), 0px 1px 1px 0px rgba(0,0,0,0.14), 0px 1px 3px 0px rgba(0,0,0,0.12);
    box-shadow: 5px 7px 13px -1px rgba(0,0,0,0.2), 0px 1px 1px 0px rgba(0,0,0,0.14), 0px 1px 3px 0px rgba(0,0,0,0.12);
    opacity:0;
}
.left-card{
        border:solid 1px #A3D855;

}
.right-section{
    opacity:1
}
.about-title{
    border-right: 3px solid #78B821;
    padding-right: 15px;
}
p{
    font-size:1.5em;
}
</style>