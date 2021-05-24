<template>
  <div id="app">
    <v-navigation-drawer app permanent>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="title">
            Application
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>
      <v-divider></v-divider>
      <v-list dense nav>
        <router-link
        v-for="item in pages"
        :key="item.name"
        :to="{ name: item.name }">
          <v-list-item link>
              <v-list-item-content>
                <v-list-item-title>
                    {{ item.name }}
                </v-list-item-title>
              </v-list-item-content>
          </v-list-item>
        </router-link>
      </v-list>
    </v-navigation-drawer>

    <v-main>
      <router-view/>
    </v-main>
  </div>
</template>
<script>
export default ({
  data() {
    return {
      pages: [
        { name: 'Home' },
        { name: 'About' },
        { name: 'Page1' },
        { name: 'Page2' },
        { name: 'Page3' }
      ]
    }
  }
})
</script>

<style lang="scss">
</style>
