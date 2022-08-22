<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          달력을 만들어보자!
        </h1>


        <p class="subheading font-weight-regular">
          1. 달력 <br>
          1-1. 지점이름<br>
          1-2. 직원들 일한 시간<br>
          1-3. 시급<br>
          1.4. 총 하루 일당<br>
          <br>
          2. 지점등록<br>
          3. 직원 등록<br>
          4. 지점에 직원등록<br>
          5. 시급등록
        </p>
      </v-col>
      <v-col class="mb-5" cols="12">
        <h2 class="headline font-weight-bold mb-5">
          Dev Page
        </h2>
        <v-row justify="center">
          <li v-for='(list,i) in DevPage' :key="i">
            <router-link :to='list.href' >{{ list.text }}</router-link>
          </li>

        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang='ts'>
import { defineComponent } from 'vue'


export default defineComponent({
  name: 'HelloWorld',

  data () {
    return {
      DevPage: [
        {
          text: 'Main',
          href: '/main',
        }
      ]
    }
  },
})
</script>
