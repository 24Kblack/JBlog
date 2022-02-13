<template>
    <v-navigation-drawer
        color="grey darken-1"
        app
        clipped>
      <v-list-item style="justify-content: right">
        <v-btn class="fold_button" icon tile large plain>
          <v-icon color="grey lighten-2" size="38">
            mdi-backburger
          </v-icon>
        </v-btn>
      </v-list-item>
      <v-list-item>
        <v-list-item-content class="top_avatar">
          <v-list-item-title class="text-h6">
            <v-avatar
                color="primary"
                size="84"
            >
              <v-icon dark size="56">
                mdi-account-circle
              </v-icon>
            </v-avatar>
          </v-list-item-title>
          <v-list-item-title style="color: rgb(211,211,211);margin-top:10px">
            用户名
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list
          dense
          nav
      >
        <v-list-item
            v-for="item in items"
            :key="item.title"
            link
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
</template>

<script>
export default {
  data () {
    return {
      items: [
        { title: 'Dashboard', icon: 'mdi-view-dashboard' },
        { title: 'Photos', icon: 'mdi-image' },
        { title: 'About', icon: 'mdi-help-box' },
      ],
      right: null,
    }
  },
}
</script>

<style scoped>
.fold_button{
  border-radius: 8px;
  margin-top: 5px;
}

.fold_button:hover{
  background: gray;
}

.top_avatar{
  margin: 0 0 20px 0;
}
</style>