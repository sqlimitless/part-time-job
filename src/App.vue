<template>
  <v-app>
    <v-main>
      <left-menu/>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import LeftMenu from './components/leftMenu/LeftMenu.vue';

export default defineComponent({
  name: 'App',

  data () {
    return {
      //
    }
  },
  components: {
    LeftMenu
  },
})
</script>
