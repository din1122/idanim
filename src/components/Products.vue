<template>

<v-container grid-list-xs pa-5>

	<v-layout row wrap>
		<v-flex xs12 pa-5 >
		<span class="section-title">הדגמים שלנו</span>
		</v-flex>
		<v-flex xs12 pa-5>
		<v-layout>
		<v-flex xs12 xl3 @click="dialog1 = true">
				<div class="img-box">
					<img :src="require('@/assets/main.jpg')" alt="home-1-cannabis" class="article-img">
				</div>
		</v-flex>
			<v-flex xs10 xl8 class="article-text" pr-3>
			<div  class="fade-prod-bg">
			<span class="product-title">H3 - מפרט טכני</span>
			</div>
				<p @click="dialog1 = true">
				לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר
				</p>
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
			<v-flex xs8 ma-auto>
				<v-img :src="require('@/assets/main.jpg')" aspect-ratio="2"> </v-img>
			</v-flex>
			<v-flex xs8 ma-auto>
			<span class="display-2">H3</span>
			<p>
			לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר
			</p>
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
		<v-flex xs12 pa-5>
		<v-layout>

			<v-flex xs10 xl8 class="article-text" pr-3>
			<div  class="fade-prod-bg-l  text-xs-left">
			<span class="product-title">H1 - מפרט טכני</span>
			</div>
				<p @click="dialog2 = true">
				לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר
				</p>
			</v-flex>
				<v-flex xs12 xl3 @click="dialog2 = true">
				<div class="img-box">
					<img :src="require('@/assets/h1.jpg')" alt="home-1-cannabis" class="article-img">
				</div>
		</v-flex>
		</v-layout>
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
			<v-flex xs8 ma-auto>
				<v-img :src="require('@/assets/h1.jpg')" aspect-ratio="2"> </v-img>
			</v-flex>
			<v-flex xs8 ma-auto>
			<span class="display-2">H3</span>
			<p>
			לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר
			</p>
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
	<v-flex xs12 pa-5>
		<v-layout>
		<v-flex xs12 xl3 @click="dialog3 = true">
				<div class="img-box">
					<img :src="require('@/assets/h5.jpg')" alt="home-1-cannabis" class="article-img">
				</div>
		</v-flex>
			<v-flex xs10 xl8 class="article-text" pr-3>
			<div  class="fade-prod-bg">
			<span class="product-title">H3 - מפרט טכני</span>
			</div>
				<p @click="dialog3 = true">
				לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר
				</p>
			</v-flex>
		</v-layout>
		<v-dialog v-model="dialog3" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">H3 - מפרט טכני </span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog3 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs8 ma-auto>
				<v-img :src="require('@/assets/h5.jpg')" aspect-ratio="2"> </v-img>
			</v-flex>
			<v-flex xs8 ma-auto>
			<span class="display-2">H3</span>
			<p>
			לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר
			</p>
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