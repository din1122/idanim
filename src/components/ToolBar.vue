<template>
<div>
  <v-toolbar fixed>
  
 <v-toolbar-side-icon  @click.stop="drawer = !drawer" class="hidden-md-and-up"></v-toolbar-side-icon>
    <v-toolbar-items class="hidden-sm-and-down RTL" >
      <v-btn flat v-scroll-to="{
        el:'#one',
      }
      "
      >בית</v-btn>
      <v-btn flat v-scroll-to="{
        el:'#two',
      offset: -70,
      }
      "
      >מוצרים</v-btn>
      <v-btn flat v-scroll-to="{
        el:'#four',
        offset: -70,
      }
      ">עלינו</v-btn>
      <v-btn flat v-scroll-to="{
        el:'#six',
        offset: -70,
      }
      ">צור קשר</v-btn> 

    </v-toolbar-items>

    <v-spacer></v-spacer>
    <div class="topbar-contact hide-om pl-2">
    <span>כתובת</span>: <span>בעל העקידה 57</span><br>
    <span>idanim11@gmail.com</span>
    </div>
    <div class="topbar-contact ">
    <span>טלפון</span>: <span>03-6208656/7</span><br>
    <div class="hide-om"><span>פקס</span>: <span> 03-6208660</span></div>
    </div>
    <img class="logo" :src="require('@/assets/trans.png')">
    
    
  </v-toolbar>
      <v-navigation-drawer
    class="indigo accent-3"
    dark
     v-model="drawer"
      absolute
      temporary
      style="position:fixed; top:0; left:0; overflow-y:scroll;"
  >
    <v-list>
      <v-list-tile @click.prevent="drawer = !drawer" v-scroll-to="{
        el:'#one',
         
      }
      ">
        <v-list-tile-content>
          <v-list-tile-title>
         בית
          </v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>
      <v-list-tile @click.prevent="drawer = !drawer" v-scroll-to="{
        el:'#two',
        offset: -100,
      }
      ">
        <v-list-tile-content>
          <v-list-tile-title>
          מוצרים
          </v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>
      <v-list-tile @click.prevent="drawer = !drawer" v-scroll-to="{
        el:'#four',
        offset: -100,
      }
      ">
        <v-list-tile-content>
          <v-list-tile-title>
          עלינו
          </v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>
      <v-list-tile @click.prevent="drawer = !drawer" v-scroll-to="{
        el:'#six',
        offset: -100,
      }
      ">
        <v-list-tile-content>
          <v-list-tile-title>
          צור קשר
          </v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>
    </v-list>
  </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data(){
    return{
        drawer: null,
    }
  }
}
</script>
<style scoped>
.v-btn{
  font-size: 1.2em;
}
>>>.v-list__tile__title{
  font-size: 1.2em;
}
>>>.theme--light.v-toolbar{
background:#1B19FD;
opacity:0.8;
color:white;
}
>>>.theme--light.v-btn{
  color:white;
}
</style>