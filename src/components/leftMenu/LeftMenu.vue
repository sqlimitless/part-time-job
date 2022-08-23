<template>
  <div class="ma-12 pa-12">
    <v-card>
      <v-navigation-drawer
          permanent
          expand-on-hover
      >
        <v-list>
          <v-list-item class="px-2">
            <v-list-item-avatar>
              <v-img src="@/sources/salt_farm_slave.jpg"></v-img>
            </v-list-item-avatar>
          </v-list-item>

          <v-list-item link>
            <v-list-item-content>
              <v-list-item-title class="text-h6">
                염전 대장
              </v-list-item-title>
              <v-list-item-subtitle>jangbro88@naver.com</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-list>

        <v-divider></v-divider>

        <v-list
            nav
            dense
        >
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-folder</v-icon>
            </v-list-item-icon>
            <v-list-item-title>염전노예 매장</v-list-item-title>
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-account-multiple</v-icon>
            </v-list-item-icon>
            <v-list-item-title>염전노예 직원</v-list-item-title>
          </v-list-item>
        </v-list>
        <v-list>
          <v-calendar ref="calendar"></v-calendar>
        </v-list>
      </v-navigation-drawer>
    </v-card>

  </div>
</template>

<script>
import 'v-calendar/dist/style.css';
export default {
  name: 'CalendarMain',
  data: () => ({
  })
}
</script>