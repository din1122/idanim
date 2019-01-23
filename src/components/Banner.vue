  <v-flex xs12 grow class="banner align-end" mt-5 >
            <v-flex text-xs-center xs12>
            <span class="white--text bannerMain-title" >דברים שכדאי לדעת עלינו</span>
            </v-flex>
            <v-layout  align-center justify-space-around row fill-height>
            <v-flex xs2 text-xs-center v-for="text in texts" >
            <v-layout >
            <v-flex text-xs-right>
            <span class="banner-number"style="font-size:3em">{{text.number}}</span>
            </v-flex>
            <v-divider vertical></v-divider>
            <v-flex  d-inline text-xs-right mr-2>
            <span class="font-weight-bold banner-title">{{text.title}}</span><br>
            <span class="font-weight-thin banner-subtitle">{{text.subtitle}}</span>
            </v-flex>
            </v-layout>
            </v-flex>
            </v-layout>
            </v-flex>