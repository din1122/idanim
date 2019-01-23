<template>
<v-container pa-5 grid-md-list class="mnp2">
<Scrollama @step-enter="stepEnterHandler" :offset="0.5">
<v-layout row wrap>



<v-flex xs12 xl3 offset-xs0 offset-xl2  data-step="2"  ref="rightbox" class="right-section m-pt-5">
    <v-card >
    <v-card-title class="white--text">צור קשר</v-card-title>
   
        <v-layout row wrap fill-height pa-3>   
        <v-flex xl12 pt-5>
                  <v-text-field outline label="שם" text-xs-right>
                  </v-text-field>
                  <v-text-field outline label="אימייל" text-xs-right>
                  </v-text-field>           
                  <v-flex pt-5>
                  <v-btn block large style="font-size:1.4em;" class="white--text">שלח</v-btn>
                  </v-flex>
        </v-flex>   
   
        <v-flex xs12 text-xs-center id="contact-text">
      
        <span>טלפון: </span> <span>03-6208656/7</span><br>
       <span>idanim11@gmail.com</span>
    
        </v-flex>      
        </v-layout>
    
    </v-card>
</v-flex>

<v-flex xs12 xl7 class="border-left fill-height pa-5 mnp2 left-section" ref="leftbox" data-step="1">
  <Gmap />
    <div class="pb-3 pt-3"><span class="display-2 about-title "> המקום </span></div>
    <p>
קבוצת עידנים רואה את נושא השירות ואיכות העבודה כיעד ראשון.
החברות השונות מעסיקות מנהלי עבודה שכל מטרתם היא לפקח ולייעל את איכות העבודה והשרות שהקבוצה מעניקה ללקוחות השונים.
עידנים עבודות ציבוריות בע"מ מפעילה רכבי טיאוט חדישים בגדלים שונים, מעסיקה מכונאים, מנהלים ועובדים מיומנים והכל בכדי לוודא שהעבודה תתנהל ברמה הגבוהה ביותר.
עידנים תשתיות בע"מ המשווקת מטאטאי כביש וציוד ניקיון נוסף, מפעילה מערך שירות של מכונאים בעלי נסיון של שנים רבות.
לרשות החברה עומד מוסך מצוייד היטב, המאוייש במכונאים ואנשי שירות ותיקים ומנוסים.
בנוסף, מפעילה החברה ניידת שירות המאובזרת בציוד וכלים הטובים ביותר ומשמשת מעין מוסך נייד,
כמו כן יש בניידת השירות מגוון עצום של חלקים המאפשר לבצע את הטיפולים והתיקונים הנדרשים במקום הימצאו של הכלי ובזמן הקצר ביותר. 
 החברה מתחייבת להעניק שירות וטיפול ללא הגבלה לשביעות רצון הלקוח.
 </p>
<p class="font-weight-bold">"אנחנו תמיד משתדלים יותר"</p>

    
</v-flex>




</v-layout>
</Scrollama>
</v-container>
</template>

<script>
import 'intersection-observer'
import Scrollama from 'vue-scrollama'
import Gmap from '@/components/Gmap'
export default {
  data() {
    return {
  
    }
  },
  components:{
      Scrollama, Gmap
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
#contact-text{
    font-size:1.4em;
}
>>>.theme--light.v-card{
    height:100%;
}
>>>.v-card__text{
    height:100%;
}
>>>.theme--light.v-btn{
    background: #78b821 !important;
}
>>>.v-label{
right:0px !important;
left:unset !important;
}

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
      background:white;
    -webkit-box-shadow: 0px 2px 1px -1px rgba(0,0,0,0.2), 0px 1px 1px 0px rgba(0,0,0,0.14), 0px 1px 3px 0px rgba(0,0,0,0.12);
      box-shadow: 5px 7px 13px -1px rgba(0,0,0,0.2), 0px 1px 1px 0px rgba(0,0,0,0.14), 0px 1px 3px 0px rgba(0,0,0,0.12);
      opacity:0;
}
.right-section{
    opacity:1
}
.about-title{
    border-right: 3px solid #78B821;
    padding-right: 15px;
}
p{
    font-size:1.2em;
}
</style>