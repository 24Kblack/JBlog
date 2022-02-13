<template>
  <v-app style="background: lightgray">
    <v-app-bar app
               dense
               color="yellow"
               elevation="1">
      <v-row
          justify="center"
          no-gutters
      >

        <v-col
            class="text-center"
            cols="12"
        >
          欢迎访问24Kblack的个人网站
        </v-col>
      </v-row>
    </v-app-bar>

    <v-main class="justify-center align-center">
      <v-container>
        <v-row class="text-center">
          <v-col>
            <v-icon
                size="130"
                color="red"
            >
              mdi-alert-octagon
            </v-icon>
          </v-col>
        </v-row>
        <v-row>
          <h1 style="margin: auto">网站正在建设中</h1>
        </v-row>
      </v-container>

    </v-main>

    <v-footer
        color="blue"
        padless
        app

    >
      <v-row
          justify="center"
          no-gutters
      >

        <v-col
            class="py-4 text-center white--text"
            cols="12"
        >
          <a class="white--text" href="https://beian.miit.gov.cn/">苏ICP备2022005009号</a>
        </v-col>
      </v-row>
    </v-footer>
  </v-app>

</template>



<script>
export default {
  name: 'Home',
  components: {
  }
}
</script>