<template>
<div>
<v-container grid-list-xs grid-list-md>
		<v-layout justify-space-around row wrap>
		<v-flex xs12 xl4 md5>
			<v-card >
			<div class="img-box" @click="dialog1 = true">
				<v-img
				:src="require('@/assets/H4/h4-0.jpg')"
				aspect-ratio="2.5"
				class="article-img"
				> </v-img>
				</div>
				<v-card-title>
                    <span class="product-title black--text">דגם H4  מכונת קירצוף ושטיפה בלחץ מתוצרת "טיסאן"</span>
                </v-card-title>
						<v-card-text pa-0 >
                        <v-flex  xs12 pa-2 class="npm">
                            <span>
							 מכונת קירצוף ושטיפה בלחץ הידרוסטטית , .
							מנוע פרקינס או איווקו, משאבות הידראוליות מתוצרת .BOSCH
							הנעה אחורית.</span>
							<v-flex xs12 text-xs-left>
							<a @click="dialog1 = true"><p class="pa-2">קרא עוד</p></a>
							</v-flex>
                        </v-flex>
					</v-card-text>
			</v-card>
		</v-flex>
		<v-dialog v-model="dialog1" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">H4 - מפרט טכני </span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog1 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs12 xl8 ma-auto>
				<v-img :src="require('@/assets/H4/h4-0.jpg')" aspect-ratio="2"> </v-img>
			</v-flex>
			<v-flex xs12 xl8 ma-auto>
			<span class="display-2">H4</span>
			<p>
			מכונת קירצוף ושטיפה בלחץ הידרוסטטית , .
			מנוע פרקינס או איווקו, משאבות הידראוליות מתוצרת .BOSCH
			הנעה אחורית.
			4X4
			הכלי רחב יותר מדגם H3 הרגיל וכולל מנוע גדול יותר. 
			כולל מערכת לשאיבת המיים המלוכלכים.
			מערכת לחימום המיים לשטיפה עד 80 מעלות צלסיוס.
			2 הליקופטרים מסתובבים בחזית הכלי לקירצוף הכביש, עם מערכת מתזים.
			רוחב קירצוף 1.3 מטר.
			הליקופטר קירצוף ידני נוסף תלוי באחורי המכונה.
			מתזי מיים הממוקמים בחזית הכלי מפזרים רסס מיים כדי לספוג את האבק בזמן פעולת הקירצוף.
			ה H3 קירצוף ושטיפה כולל מערכת נוספת לשטיפה בלחץ עם צינור באורך של 50 מטר ושני אקדחי שטיפה בלחץ גבוה. המערכת מורכבת על גג הכלי ומאפשרת שטיפה בכל הכיוונים.
			תא נהג פנורמי, מבודד מפגעי מזג אויר, רעשים, אבק וגזי פליטה.
			תא הנהג כולל מערכת מיזוג אויר, כיסא נהג קפיצי, מתכוונן ונוח במיוחד. וכן כיסא נוסף לאיש צוות שני.
			רדיו ומצלמה אחורית עם מסך צבעוני.
			וכן מערכת שליטה ותפעול של מערכת השטיפה והקירצוף.
			</p>
			<img :src="require('@/assets/H4/h4-1.jpg')" alt="idanim-h4">
			<img :src="require('@/assets/H4/h4-2.jpg')" alt="idanim-h4">
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
		<v-flex xs12 xl4 md5>
				<v-card class="green-bg" >
				<Div class="img-box">
				<v-img @click="dialog1 = true"
				:src="require('@/assets/d4000/d4000-0.jpg')"
				aspect-ratio="2.5"
				class="article-img"
				> </v-img>
				</Div>
				<v-card-title>
                    <span class="product-title">דגם D4000  מתוצרת "טיסאן"</span>
                </v-card-title>
						<v-card-text pa-0 >
                        <v-flex  white--text xs12 pa-2 class="npm">
						<span>
						משאית לטיאוט כבישים בנפח של  4.5 מ"ק.
מתקן הטיאוט מורכב על גבי שילדה מתוצרת "הינו טויוטה"
כולל 2 מברשות צדדיות הנעות לכל הכיוונים, מברשת גלילית מרכזית ופיית יניקה בעלת כושר יניקה גבוה במיוחד,

						</span>
							<v-flex xs12 text-xs-left>
							<a @click="dialog2 = true"><p class="pa-2">קרא עוד</p></a>
							</v-flex>
                        </v-flex>
					</v-card-text>
			</v-card>
		</v-flex>
		<v-dialog v-model="dialog2" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">H3 - מפרט טכני </span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog2 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs12 xl8 ma-auto>
				<v-img :src="require('@/assets/d4000/d4000-0.jpg')" aspect-ratio="2"> </v-img>
			</v-flex>
			<v-flex xs12 xl8 ma-auto>
			<span class="display-2">H3</span>
			<p>
			משאית לטיאוט כבישים בנפח של  4.5 מ"ק.
מתקן הטיאוט מורכב על גבי שילדה מתוצרת "הינו טויוטה"
כולל 2 מברשות צדדיות הנעות לכל הכיוונים, מברשת גלילית מרכזית ופיית יניקה בעלת כושר יניקה גבוה במיוחד,
מתזי מיים הממוקמים בחזית ובמרכז הכלי מפזרים רסס מיים כדי לספוג את האבק בזמן פעולת הטיאטוא.
מיכל המיים גדול במיוחד ונותן אפשרות לעבודת שטיפה רציפה לאורך זמן.
ה D4000 כולל מערכת נוספת לשטיפה בלחץ עם צינור באורך של 15 מטר ואקדח שטיפה בלחץ גבוה. המערכת מורכבת על גג הכלי ומאפשרת שטיפה בכל הכיוונים.
וכן צינור שאיבה גדול המותקן באחורי המשאית.
תא הנהג מבודד מפגעי מזג אויר, רעשים, אבק וגזי פליטה.
תא הנהג כולל מערכת מיזוג אויר, כיסא נהג קפיצי, מתכוונן ונוח במיוחד. וכן כיסא נוסף לאיש צוות שני. 
רדיו ומצלמה אחורית עם מסך צבעוני.
וכן מערכת שליטה ותפעול של המברשות, השטיפה וריקון מיכל האשפה.
			</p>
			<v-img :src="require('@/assets/d4000/d4000-1.jpg')" alt="idanim-h4"> </v-img>
			<v-img :src="require('@/assets/d4000/d4000-2.jpg')" alt="idanim-h4"> </v-img>
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
</v-layout>
</v-container>

<v-container grid-list-xs grid-list-md>
		<v-layout justify-space-around row wrap>
		<v-flex xs12 xl4 md5>
			<v-card >
			<div class="img-box" @click="dialog3 = true">
				<v-img
				:src="require('@/assets/d4000b/d4000-0.jpg')"
				aspect-ratio="1.5"
				class="article-img"
				> </v-img>
				</div>
				<v-card-title>
                    <span class="product-title black--text">דגם D4000  מתוצרת "קדמה"</span>
                </v-card-title>
						<v-card-text pa-0 >
                        <v-flex  xs12 pa-2 class="npm">
						<span>
	משאית לטיאוט כבישים בנפח מיכל של  4.5 מ"ק ועד 8 מ"ק.
מתקן הטיאוט מורכב על גבי שילדה מתוצרת "הינו טויוטה" או "דאף", תלוי בגודל המיכל.
כולל 2 מברשות צדדיות הנעות לכל הכיוונים, מברשת גלילית מרכזית ופיית יניקה בעלת כושר יניקה גבוה במיוחד,
						</span>
							<v-flex xs12 text-xs-left>
							<a @click="dialog3 = true"><p class="pa-2">קרא עוד</p></a>
							</v-flex>
                        </v-flex>
					</v-card-text>
			</v-card>
		</v-flex>
		<v-dialog v-model="dialog3" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">דגם D4000  מתוצרת "קדמה"</span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog3 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs12 xl8 ma-auto>
				<v-img :src="require('@/assets/d4000b/d4000-0.jpg')" aspect-ratio="2"> </v-img>
			</v-flex>
			<v-flex xs12 xl8 ma-auto>
			<span class="display-2">דגם D4000  מתוצרת "קדמה"</span>
			<p>
		משאית לטיאוט כבישים בנפח מיכל של  4.5 מ"ק ועד 8 מ"ק.
מתקן הטיאוט מורכב על גבי שילדה מתוצרת "הינו טויוטה" או "דאף", תלוי בגודל המיכל.
כולל 2 מברשות צדדיות הנעות לכל הכיוונים, מברשת גלילית מרכזית ופיית יניקה בעלת כושר יניקה גבוה במיוחד,
מתזי מיים הממוקמים בחזית ובמרכז הכלי מפזרים רסס מיים כדי לספוג את האבק בזמן פעולת הטיאטוא.
מיכל המיים גדול במיוחד 1,200 ליטר ונותן אפשרות לעבודת שטיפה רציפה לאורך זמן.
ה D4000 כולל מערכת נוספת לשטיפה בלחץ עם צינור באורך של 15 מטר ואקדח שטיפה בלחץ גבוה. המערכת מורכבת על גג הכלי ומאפשרת שטיפה בכל הכיוונים.
וכן צינור שאיבה גדול המותקן באחורי המשאית.
תא הנהג מבודד מפגעי מזג אויר, רעשים, אבק וגזי פליטה.
תא הנהג כולל מערכת מיזוג אויר, כיסא נהג קפיצי, מתכוונן ונוח במיוחד. וכן כיסא נוסף לאיש צוות שני. 
רדיו ומצלמה אחורית עם מסך צבעוני.
וכן מערכת שליטה ותפעול של המברשות, השטיפה וריקון מיכל האשפה.
			</p>
			
			</v-flex>
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
		<v-flex xs12 xl4 md5>
				<v-card class="green-bg" >
				<Div class="img-box">
				<v-img @click="dialog4 = true"
				:src="require('@/assets/cart/1.jpg')"
				aspect-ratio="1.5"
				class="article-img"
				> </v-img>
				</Div>
				<v-card-title>
                    <span class="product-title">עגלות לטיאטוא מדרכות</span>
                </v-card-title>
						<v-card-text pa-0 >
                        <v-flex  white--text xs12 pa-2 class="npm">
						<span>
						מגוון רחב של עגלות לשימוש ממושך עמידות לכל פגעי מזג אויר
						העגלות כוללות מתקן מיוחד למטאטא וליעה.
						ניתן לקבלן בגדלים ובצבעים שונים.
						</span>
							<v-flex xs12 text-xs-left>
							<a @click="dialog4 = true"><p class="pa-2">קרא עוד</p></a>
							</v-flex>
                        </v-flex>
					</v-card-text>
			</v-card>
		</v-flex>
		<v-dialog v-model="dialog4" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">עגלות לטיאטוא מדרכות </span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog4 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs12 xl8 ma-auto>
				<v-img :src="require('@/assets/cart/1.jpg')" aspect-ratio="2"> </v-img>
			</v-flex>
			<v-flex xs12 xl8 ma-auto>
			<span class="display-2">H3</span>
			<p>
			מגוון רחב של עגלות לשימוש ממושך עמידות לכל פגעי מזג אויר
			העגלות כוללות מתקן מיוחד למטאטא וליעה.
			ניתן לקבלן בגדלים ובצבעים שונים.
			</p>
			<v-img :src="require('@/assets/cart/2.jpg')" alt="idanim-h4"></v-img>
			<v-img :src="require('@/assets/cart/3.jpg')" alt="idanim-h4"></v-img>
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
</v-layout>
</v-container>
</div>
</template>

<script>
export default {
	data(){
		return{
			dialog1:false,
			dialog2:false,
			dialog3:false,
			dialog4:false,
		}
	}
}
</script>
<style scoped>
.green-bg{
    background:#A3D855 !important;
}
.article-img {
width: 100%;
height: 270px;
transition: all 0.2s ease-out;
object-fit: cover;
cursor: pointer;
}

.article-img:hover {
-webkit-transform: scale(1.05);
-ms-transform: scale(1.05);
transform: scale(1.05);
transition: all 0.2s ease;
cursor: pointer;
}
	.img-box {
		overflow: hidden;
		transition: all 0.2s ease-out;
		box-shadow: -15px 10px 30px -10px #00000099;
		height: 95%;
	}
</style>