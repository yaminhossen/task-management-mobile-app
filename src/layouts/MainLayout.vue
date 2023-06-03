<template>
  <q-layout view="lHh Lpr lFf">
    <q-header >
     
        
        <div class="navbar">
          <div>
            
        <button class="menu"  @click="toggleLeftDrawer"><i class="fa-solid fa-bars"></i></button>
        </div>
       

        <div class="logo">
          <img src="expert-1.jpg" alt="">
        </div>
        </div>
      
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
    >
      <q-list>
        <q-item-label
          header
        >
          Essential Links
        </q-item-label>

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
      <div>
      </div>
    </q-page-container>
  </q-layout>
</template>


<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'

const linksList = [
  {
    title: 'Docs',
    caption: 'quasar.dev',
    icon: 'school',
    link: 'https://quasar.dev'
  },
  {
    title: 'Github',
    caption: 'github.com/quasarframework',
    icon: 'code',
    link: 'https://github.com/quasarframework'
  },
  {
    title: 'Discord Chat Channel',
    caption: 'chat.quasar.dev',
    icon: 'chat',
    link: 'https://chat.quasar.dev'
  },
  {
    title: 'Forum',
    caption: 'forum.quasar.dev',
    icon: 'record_voice_over',
    link: 'https://forum.quasar.dev'
  },
  {
    title: 'Twitter',
    caption: '@quasarframework',
    icon: 'rss_feed',
    link: 'https://twitter.quasar.dev'
  },
  {
    title: 'Facebook',
    caption: '@QuasarFramework',
    icon: 'public',
    link: 'https://facebook.quasar.dev'
  },
  {
    title: 'Quasar Awesome',
    caption: 'Community Quasar projects',
    icon: 'favorite',
    link: 'https://awesome.quasar.dev'
  }
]

export default defineComponent({
  name: 'MainLayout',

  components: {
    EssentialLink
  },

  setup () {
    const leftDrawerOpen = ref(false)

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>
<style scoped>
.navbar{
  background-color: white;
  display: flex;
  justify-content: space-between;
  padding-top: 10px;
  /* border: 1px solid red; */
  align-items: center;
  
  
}
.menu{
  color: rgb(38, 35, 35);
  margin-left: 20px;
  background-color: white;
  font-size: 18px;
  margin-bottom: 5px;
 border: 1px solid rgb(14, 65, 175);
 border-radius: 5px;
}
.menu i{
  /* font-size: 20px; */
  /* background-color: white; */
  /* padding: 2px; */
  /* border: none; */
  /* margin-bottom: 3px; */
}
.logo img{
  width: 40px;
  border-radius: 30%;
  margin-right: 20px;
}
</style>
