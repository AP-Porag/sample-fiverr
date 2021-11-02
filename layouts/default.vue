<template>
  <v-app>
    <v-navigation-drawer
      v-model="drawer"
      temporary
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      class="nav-bar"
      :clipped-left="clipped"
      fixed
      app
      flat
    >
      <v-toolbar-title class="text-uppercase title" v-text="title" />
      <img @click.stop="drawer = !drawer" class="mr-3 menu_icon" :src="require('~/static/hamburger.png')"/>
      <v-toolbar-title class="subtitle-1" v-text="subtitle" />
      <v-spacer />
    </v-app-bar>
    <v-main>
      <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      title: 'Menscript',
      subtitle:'Account Menu'
    }
  }
}
</script>

<style scoped lang="scss">
.theme--light.v-application{
  background: #fafafa;
}
.nav-bar{
  background: #fafafa !important;
}
.title{
  font-family: WorkSans !important;
  font-size: 18px !important;
  line-height: 21px !important;
  letter-spacing: 3px !important;
  color: #2A2A2A !important;
  font-weight: 600;
}
.subtitle-1{
  font-family: Inter !important;
  font-style: normal !important;
  font-weight: normal !important;
  font-size: 15px !important;
  color: #2A2A2A !important;
}
.menu_icon{
  height: 8px;
  width: 25px;
  cursor: pointer;
  margin-left: 30px;
  margin-right: 10px;
}
</style>
