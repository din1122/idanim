<template>
<v-container grid-list-xs>
		<v-layout justify-space-around>
		<v-flex xs4>
			<v-card >
			<div class="img-box" @click="dialog1 = true">
				<v-img
				:src="require('@/assets/main.jpg')"
				aspect-ratio="2.5"
				class="article-img"
				> </v-img>
				</div>
				<v-card-title>
                    <span class="product-title black--text">H3</span>
                </v-card-title>
						<v-card-text pa-0 >
                        <v-flex  xs12 pa-2>
                            <span>לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר</span>
							<a @click="dialog1 = true"><p class="left pa-2">קרא עוד</p></a>
                        </v-flex>
					</v-card-text>
			</v-card>
		</v-flex>
		<v-dialog v-model="dialog1" hide-overlay>
			<v-card>
			<v-toolbar>

			<v-toolbar-title>
			<span class=" black--text">H1 - מפרט טכני </span>
			</v-toolbar-title>
				<v-spacer></v-spacer>
			<v-toolbar-items>
		
			<v-icon @click="dialog1 = false">close</v-icon>
			</v-toolbar-items>
			</v-toolbar>
			<v-card-text>
			<v-container>
			<v-flex xs8 ma-auto>
				<v-img :src="require('@/assets/h5.jpg')" aspect-ratio="2"> </v-img>
			</v-flex>
			<v-flex xs8 ma-auto>
			<span class="display-2">H1</span>
			<p>
			לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר
			</p>
			
			</v-flex>
			
			</v-container>
			</v-card-text>
			</v-card>
		</v-dialog>
		<v-flex xs4>
				<v-card class="green-bg" >
				<Div class="img-box">
				<v-img @click="dialog1 = true"
				:src="require('@/assets/h1.jpg')"
				aspect-ratio="2.5"
				class="article-img"
				> </v-img>
				</Div>
				<v-card-title>
                    <span class="product-title">H1</span>
                </v-card-title>
						<v-card-text pa-0 >
                        <v-flex  white--text xs12 pa-2>
                            <span>לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית לורם איפסום דולור סיט אמט, קונסקטורר אדיפיסינג אלית. סת אלמנקום ניסי נון ניבאה. דס איאקוליס וולופטה דיאם. וסטיבולום אט דולור, קראס אגת לקטוס וואל אאוגו וסטיבולום סוליסי טידום בעליק. נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר, בנפת נפקט למסון בלרק - וענוף נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן נולום ארווס סאפיאן - פוסיליס קוויס, אקווזמן קוואזי במר מודוף. אודיפו בלאסטיק מונופץ קליר</span>
							<a @click="dialog2 = true"><p class=" pa-2 left">קרא עוד</p></a>
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
		</v-layout>
</v-layout>
</v-container>
</template>

<script>
export default {
	data(){
		return{
			dialog1:false,
			dialog2:false,
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