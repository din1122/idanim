<template>
  <v-app>
    <v-content>
    <ToolBar/>
      <router-view> </router-view>
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import 'intersection-observer'
import Scrollama from 'vue-scrollama'
import { TimelineLite } from 'gsap'
import ToolBar from '@/components/ToolBar'
import Footer from '@/components/footer'
export default {
  name: 'App',
  components: {
    ToolBar,Footer, Scrollama
  },
  data () {
    return {
      //
    }
  }
}
</script>
