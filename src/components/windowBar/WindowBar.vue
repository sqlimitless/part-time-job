<template>
  <div>
    <v-system-bar
        window
        dark
        style="-webkit-app-region: drag;"
    >
      <v-icon>mdi-message</v-icon>
      <span>10 unread messages</span>
      <v-spacer></v-spacer>
      <v-icon @click="minimize">mdi-minus</v-icon>
      <v-icon>mdi-checkbox-blank-outline</v-icon>
      <v-icon @click="close">mdi-close</v-icon>
    </v-system-bar>
  </div>
</template>

<script>
// import windowBar from "@/components/windowBar/windowBar.ts";
// const { ipcRenderer } = require("electron");
// import { ipcRenderer } from 'electron'

export default {
  name: "WindowBar",
  methods: {
    minimize() {
      // windowBar.minimize()
      // ipcRenderer.send('min', 'send');
    },
    close() {
      // windowBar.close()
      // ipcRenderer.send('min', 'send');
    }
  }
}
</script>

<style scoped>

</style>