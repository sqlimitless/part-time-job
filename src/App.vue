<template>
  <v-app>
    <v-main>
      <window-bar/>
      <left-menu/>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import LeftMenu from './components/leftMenu/LeftMenu.vue';
import WindowBar from './components/windowBar/WindowBar.vue';

export default defineComponent({
  name: 'App',

  data () {
    return {
      //
    }
  },
  components: {
    LeftMenu,
    WindowBar
  },
})
</script>
