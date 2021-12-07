<template>
  <div class="parent py-9 work">
    <v-container>
      <v-row class="intro">
        <v-col cols="12">
          <h2 class="mb-4">Work Experiences</h2>
          <p>
            This is the retrospective of my professional experiences in a
            company, you can also download my CV for more details
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
            <v-btn
              depressed
              outlined
              class="my-5 btn"
              large
              href="bitotalaurene-cv-web-dev.pdf"
              download
            >
              Download CV
            </v-btn>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
import 'animate.css'
export default {
  data() {
    return {
      items: [
        {
          color: '#db2951',
          date: 'January 2021 to Present',
          entreprise: 'Kinshasa Digital',
          poste: 'Web Developer',
          descriptif:
            'I am a FrontEnd developer of internal projects for the company or those of our clients',
        },
        {
          color: '#FFCF00',
          date: 'September 2020 to December 2020',
          entreprise: 'Kinshasa Digital',
          poste: 'Web Developer Trainee',
          descriptif:
            'I worked there as a Frontend trainee developer on projects for the client company',
        },
        {
          color: '#db2951',
          date: 'November 2018 to Septembre 2020',
          entreprise: 'Diamond Touristic',
          poste: 'Commerciale & Projet',
          descriptif:
            'I worked there as a project manager for the planning and implementation of internal and external projects of the company as well as the implementation of business strategies for the various tourism activities of the company.',
        },
        {
          color: '#FFCF00',
          date: 'October 2017 to December 2017',
          entreprise: 'Banque Centrale of Congo',
          poste: 'Developer Trainee',
          descriptif:
            'I worked there as a trainee developer and assisted in the management of certain software within the IT department (Application service for accounting, financial and management systems).',
        },
      ],
    }
  },
}
</script>
<style>
.work {
  background-image: linear-gradient(rgb(245 245 245 / 90%), rgb(245 245 245)),
    url('~/assets/images/12.jpg') !important;
  background-position: center center;
  background-repeat: no-repeat;
  background-size: contain;
}
</style>
