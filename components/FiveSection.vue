<template>
  <div class="parent py-9">
    <v-container>
      <v-row class="intro">
        <v-col cols="12">
          <h2>Work Experiences</h2>
          <p>
            Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
            officia deserunt mollit anim id est laborum. Sed ut perspiciatis
            unde omnis iste natur
          </p>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12">
          <v-timeline align-top :dense="$vuetify.breakpoint.smAndDown">
            <v-timeline-item
              v-for="(item, i) in items"
              :key="i"
              :color="item.color"
              fill-dot
            >
              <v-card :color="item.color" dark>
                <v-card-title class="text-h6"> {{ item.date }} </v-card-title>
                <v-card-text class="white text--primary pa-5">
                  <div class="d-flex">
                    <h3>{{ item.entreprise }} |</h3>
                    <p class="ml-1">{{ item.poste }}</p>
                  </div>
                  <p>
                    {{ item.descriptif }}
                  </p>
                </v-card-text>
              </v-card>
            </v-timeline-item>
          </v-timeline>
          <div class="d-flex justify-end">
            <v-btn depressed outlined class="my-5 btn" large>
              Download CV
            </v-btn>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          color: '#fe0872',
          date: 'Janvier 2021 to Present',
          entreprise: 'Kinshasa Digital',
          poste: 'Développeuse Web',
          descriptif:
            "Je suis développeuse front end de projets internes à l'entreprise ou ceux de nos clients",
        },
        {
          color: '#e301fffc',
          date: 'September 2020 to December 2020',
          entreprise: 'Kinshasa Digital',
          poste: 'Développeuse Web stagiaire',
          descriptif:
            "J'y ai travaillé en tant que développeuse stagiaire Frontend sur des projets pour l'entreprise clients",
        },
        {
          color: '#FFCF00',
          date: 'November 2018 to Septembre 2020',
          entreprise: 'Diamond Touristic',
          poste: 'Commerciale & Projet',
          descriptif:
            "J'y ai travaillé en tant que chef de projet pour les planifications  et les réalisations des projets internes et externes de l'entreprise  ainsi que la mise en place des stratégies commerciaux pour les différents activités touristiques de l'entreprise.",
        },
        {
          color: '#fe3a00fc',
          date: 'October 2017 to December 2017',
          entreprise: 'Banque Centrale of Congo',
          poste: 'Stagiaire Développeuse',
          descriptif:
            "J'y ai travaillé en tant que développeuse stagiaire et assister aux différents dans la gestion des certains logiciels au sein de la direction Informatique ; Service des applications des systèmes comptables, financiers et de gestion.",
        },
      ],
    }
  },
}
</script>
