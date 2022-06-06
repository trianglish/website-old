<template>
  <v-card>
    <div class="mx-auto">
      <app-logo />
    </div>
    <!-- <v-card-title primary-title class="p-8"> -->
    <!-- <h1 class="headline text-xs-center">{{ cardTitle }}</h1> -->
    <!-- <p class="body-1 text-xs-center">{{ cardDescription }}</p> -->
    <!-- </v-card-title> -->
    <v-card-text>
      <!-- <div>Word of the Day</div> -->
      <h1 class="text-h4 text--primary pb-4">
        {{ cardTitle }} Marketing
        <!-- Tri•ang•l•ish -->
      </h1>
      <!-- <p>noun</p> -->
      <div class="text--primary">
        {{ cardDescription }}
        <!-- "a benevolent smile" -->
      </div>
    </v-card-text>
    <v-list two-line>
      <!-- <v-list-item>
        <v-list-item-icon>
          <v-icon color="indigo">
            mdi-phone
          </v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>(+44) 0161 375 1234</v-list-item-title>
          <v-list-item-subtitle>Work</v-list-item-subtitle>
        </v-list-item-content>

        <v-list-item-icon>
          <v-icon>mdi-message-text</v-icon>
        </v-list-item-icon>
      </v-list-item> -->

      <!-- <v-list-item>
        <v-list-item-action></v-list-item-action>

        <v-list-item-content>
          <v-list-item-title>(323) 555-6789</v-list-item-title>
          <v-list-item-subtitle>Work</v-list-item-subtitle>
        </v-list-item-content>

        <v-list-item-icon>
          <v-icon>mdi-message-text</v-icon>
        </v-list-item-icon>
      </v-list-item> -->

      <!-- <v-divider inset></v-divider> -->

      <v-list-item>
        <v-list-item-icon>
          <v-icon color="indigo">
            mdi-email
          </v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>wearetranglish@gmail.com</v-list-item-title>
          <!-- <v-list-item-subtitle>Work</v-list-item-subtitle> -->
        </v-list-item-content>
      </v-list-item>

      <!-- <v-list-item>
        <v-list-item-action></v-list-item-action>

        <v-list-item-content>
          <v-list-item-title>ali_connors@example.com</v-list-item-title>
          <v-list-item-subtitle>Work</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item> -->

      <v-divider inset></v-divider>

      <v-list-item>
        <v-list-item-icon>
          <v-icon color="indigo">
            mdi-map-marker
          </v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>8 Buxton Street</v-list-item-title>
          <v-list-item-subtitle>Manchester, UK SK8 4NW</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-list>
    <!-- <app-stack v-bind:stack="cardTechnologyStack" class="pb-8 px-8"></app-stack> -->
  </v-card>
</template>

<script>
export default {
  name: 'HelloCard',
  components: {
    AppLogo: () => import('~/components/ui/AppLogo.vue')
    // AppStack: () => import('~/components/placeholder/Stack.vue')
  },
  props: {
    cardTitle: { type: String, default: 'Trianglish' },
    cardDescription: {
      type: String,
      default: 'A full-featured boilerplate for static websites.'
    },
    cardTechnologyStack: {
      type: Array,
      default: () => [
        {
          name: 'Email',
          description: '',
          icon: 'mdi-mail',
          color: 'cyan',
          url: ''
        },
        {
          name: 'Node.js',
          description: '',
          icon: 'mdi-nodejs',
          color: 'green'
        },
        {
          name: 'NuxtJS',
          description: '',
          icon: 'mdi-nuxt',
          color: 'teal'
        },
        {
          name: 'Vue.js',
          description: '',
          icon: 'mdi-vuejs',
          color: 'teal'
        },
        {
          name: 'Vuetify',
          description: '',
          icon: 'mdi-vuetify',
          color: 'blue lighten-2'
        }
      ]
    }
  }
}
</script>

<style>
.v-card__text,
.v-card__title {
  word-break: normal;
}
</style>
