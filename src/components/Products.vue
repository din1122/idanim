<template>

<v-container grid-list-xs grid-list-md  fluid>

	<v-layout row wrap justify-space-around>
		<v-flex xs12 pa-5 class="npm3" >
		<span class="section-title">הדגמים שלנו</span>
		</v-flex>
		<v-flex xs12 pa-5 class="npm">
		<v-layout row wrap>
		<v-flex xs12 xl3 md4 @click="dialog1 = true">
				<div class="img-box">
					<img :src="require('@/assets/main.jpg')" alt="home-1-model" class="article-img">
				</div>
		</v-flex>
			<v-flex xs12 xl8 md8 class="article-text npm" pr-3>
			<div  class="fade-prod-bg">
			<span class="product-title">H3 - מפרט טכני</span>
			</div>
			<v-layout column wrap justify-space-between>
				<v-flex>
					<p class="caption-text" @click="dialog1 = true">
				מטאטא כבישים הידרוסטטי , הכלי מיוצר בנפחים שונים, 3.2 – 3.5 – 4 מ"קמ
				מנוע פרקינס, משאבות הידראוליות מתוצרת .BOSCH
				הכלי צר ומתאים במיוחד לרחובות צרים ואזורים צפופים.
				כולל 4 מברשות הנעות לכל הכיוונים ופיית יניקה בעלת כושר יניקה גבוה במיוחד
					</p>
				</v-flex>
				<v-flex>
					<p @click="dialog1 = true" class="details-link">לפרטים נוספים..</p>
				</v-flex>
			</v-layout>
			</v-flex>
		</v-layout>
		</v-flex>
		<v-dialog v-model="dialog1" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">H3 - מפרט טכני </span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog1 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs12 xl8 ma-auto>
				<v-img :src="require('@/assets/H3/h3-0.jpg')"></v-img>
			</v-flex>
			<v-flex xs12 xl8 ma-auto>
			<span class="display-2">	דגם H3  מתוצרת "טיסאן" </span>
			<p>
						
			מטאטא כבישים הידרוסטטי , הכלי מיוצר בנפחים שונים, 3.2 – 3.5 – 4 מ"קמ
			מנוע פרקינס, משאבות הידראוליות מתוצרת .BOSCH
			הכלי צר ומתאים במיוחד לרחובות צרים ואזורים צפופים.
			כולל 4 מברשות הנעות לכל הכיוונים ופיית יניקה בעלת כושר יניקה גבוה במיוחד,
			מתזי מיים הממוקמים בחזית הכלי מפזרים רסס מיים כדי לספוג את האבק בזמן פעולת הטיאטוא.
			ה H3 כולל מערכת נוספת לשטיפה בלחץ עם צינור באורך של 15 מטר ואקדח שטיפה בלחץ גבוה. המערכת מורכבת על גג הכלי ומאפשרת שטיפה בכל הכיוונים.
			תא נהג פנורמי, מבודד מפגעי מזג אויר, רעשים, אבק וגזי פליטה.
			תא הנהג כולל מערכת מיזוג אויר, כיסא נהג קפיצי, מתכוונן ונוח במיוחד, רדיו ומצלמה אחורית עם מסך צבעוני.
			וכן מערכת שליטה ותפעול של המברשות, השטיפה וריקון מיכל האשפה.

			</p>
			<v-img :src="require('@/assets/H3/h3-1.jpg')"></v-img>
			<v-img :src="require('@/assets/H3/h3-2.jpg')"></v-img>
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
		<v-flex xs12 pa-5 class="npm">
		<v-layout row wrap>
			<v-flex xs12 xl3 md4  @click="dialog2 = true" class="r-product">
					<div class="img-box">
						<img :src="require('@/assets/H1/h1-0.jpg')" alt="home-1-idanim" class="article-img">
					</div>
			</v-flex>
			<v-flex xs12 xl8 md8 class="article-text npm" pl-3>
			<div  class="fade-prod-bg-l  text-xs-left">
			<span class="product-title">H1 - דגם תוצרת טיסאן <br></span>
			</div>
				<v-layout column wrap justify-space-between>
				<v-flex>
					<p class="caption-text" @click="dialog2 = true">
					דגם מסוג H1 מתאים למדרכות וכבישים קטנים בעל זרוע טיטוא אחת
					</p>
				</v-flex>
				<v-flex>
					<p @click="dialog2 = true" class="details-link">לפרטים נוספים..</p>
				</v-flex>
			</v-layout>
			</v-flex>
				<v-flex xs12 xl3 md4  @click="dialog2 = true" class="l-product">
				<div class="img-box">
					<img :src="require('@/assets/h1.jpg')" alt="home-1-idanim" class="article-img">
				</div>
				</v-flex>
		</v-layout>
		</v-flex>
		<v-dialog v-model="dialog2" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">H1 - מפרט טכני </span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog2 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs12 xl8 ma-auto>
				<v-img :src="require('@/assets/H1/h1-0.jpg')" aspect-ratio="1"> </v-img>
			</v-flex>
			<v-flex xs12 xl8 ma-auto>
			<span class="display-2">דגם H1 תוצרת "טיסאן"</span>
			<p>
				משאית לטיאוט כבישים ומדרכות
מהירות נסיעה 0-24 ק"מ
טיפוס: 22
קיבולת גורפת: 22,000 מ"ר
נתיב ניקוי: 1330-2350 מ"מ
מנוע דיזל 26,5
קיבולת הופר 550 ל
מטאטא ללא אבק עם מערכת סינון
מתאים לכל עונות השנה
כלל מברשת אחת המגיעה למרחק של עד 2350 מ"מ
			</p>
			<v-img :src="require('@/assets/H1/h1-1.jpg')" alt="home-1-idanim"> </v-img>
			<v-img :src="require('@/assets/H1/h1-2.jpg')" alt="home-1-idanim"> </v-img>
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
	<v-flex xs12 pa-5 class="npm">
		<v-layout row wrap>
		<v-flex xs12 xl3 md4  @click="dialog3 = true">
				<div class="img-box">
					<img :src="require('@/assets/H5/h5-0.jpg')" alt="home-1-H5" class="article-img">
				</div>
		</v-flex>
			<v-flex xs12 xl8 md8 class="article-text npm" pr-3>
			<div  class="fade-prod-bg">
			<span class="product-title">דגם H5  מתוצרת "טיסאן"</span>
			</div>
				<v-layout column wrap justify-space-between>
				<v-flex>
					<p class="caption-text" @click="dialog3 = true">
					ספינת הדגל של המפעל,
מטאטא כבישים הידרוסטטי עם מנוע חזק במיוחד, 
המיכל בנפח של 5 מ"ק.
מנוע פרקינס או איווקו, משאבות הידראוליות מתוצרת .BOSCH

					</p>
				</v-flex>
				<v-flex>
					<p @click="dialog3 = true" class="details-link">לפרטים נוספים..</p>
				</v-flex>
			</v-layout>
			</v-flex>
		</v-layout>
		<v-dialog v-model="dialog3" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">H5 - מפרט טכני </span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog3 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs12 xl8 ma-auto>
						<v-img :src="require('@/assets/H5/h5-0.jpg')"></v-img>
			</v-flex>
			<v-flex xs12 xl8 ma-auto>
			<span class="display-2">H5</span>
			<p>
			ספינת הדגל של המפעל,
מטאטא כבישים הידרוסטטי עם מנוע חזק במיוחד, 
המיכל בנפח של 5 מ"ק.
מנוע פרקינס או איווקו, משאבות הידראוליות מתוצרת .BOSCH
הכלי רחב יותר מדגם H4 וכולל מנוע גדול יותר. 
כולל מערכת יחודית של 2 מברשות הנעות ימינה ושמאלה להגדלת רוחב הטיאוט ופיית יניקה בעלת כושר יניקה גבוה במיוחד,
מתזי מיים הממוקמים בחזית הכלי מפזרים רסס מיים כדי לספוג את האבק בזמן פעולת הטיאטוא.
מיכל המיים גדול במיוחד ונותן אפשרות לעבודת שטיפה רציפה לאורך זמן.
ה H5 כולל מערכת נוספת לשטיפה בלחץ עם צינור באורך של 15 מטר ואקדח שטיפה בלחץ גבוה. המערכת מורכבת על גג הכלי ומאפשרת שטיפה בכל הכיוונים.
תא נהג פנורמי, מבודד מפגעי מזג אויר, רעשים, אבק וגזי פליטה.
תא הנהג כולל מערכת מיזוג אויר, כיסא נהג קפיצי, מתכוונן ונוח במיוחד. וכן כיסא נוסף לאיש צוות שני. 
רדיו ומצלמה אחורית עם מסך צבעוני.
וכן מערכת שליטה ותפעול של המברשות, השטיפה וריקון מיכל האשפה.

			</p>
				<v-img :src="require('@/assets/H5/h5-1.jpg')"></v-img>
				<v-img :src="require('@/assets/H5/h5-2.jpg')"></v-img>
				<v-img :src="require('@/assets/H5/H5-H4.jpg')"></v-img>
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
		</v-flex>
		<v-flex xs12>
			<v-divider class="sec-divider"></v-divider>
		</v-flex>
		</v-layout>
</v-container>
</template>

<script>
export default {
	data(){
		return{
			dialog1:false,
			dialog2:false,
			dialog3:false,
		}
	},
}
</script>

<style scoped>
.v-toolbar{
	border:none !important;
	background:#A3D855 !important;

}
.card-title{
	background:#A3D855 !important;
}
.sec-divider{
border-color:#86bf39;
}
	.aurtor {
		color: #78B821
	}

	.aurtor:hover {
		color: #78B821
	}

	.article-img {
	width: 100%;
	height: 270px;
	transition: all 0.2s ease-out;
    object-fit: cover;

	}

	.article-img:hover {
		-webkit-transform: scale(1.05);
		-ms-transform: scale(1.05);
		transform: scale(1.05);
		transition: all 0.2s ease;
		cursor: pointer;
	}


	.article-main-title {
		border-left: 3px solid #78B821;
		padding-left: 15px;
	}

	a {
		color: none !important;
	}

	.img-box {
		overflow: hidden;
		transition: all 0.2s ease-out;
		box-shadow: -15px 10px 30px -10px #00000099;
		height: 95%;
	}
</style>