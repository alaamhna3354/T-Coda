<template>
    <div id="projects">
      <img class="body-cover absolute" src="@/assets/img/global/grid.svg" alt="">
        <HeadSection :Title="`Projects`" />
      <Index />
     </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
  name: 'Projects Page',
  data(){
    return{
    }
  },
  components: {
    Index: defineAsyncComponent( () => import(/* webpackChunkName: "App" */'@/components/Pages/Projects/index.vue') ),
    HeadSection: defineAsyncComponent(() => import(/* webpackChunkName: "App" */'@/components/Global/HeadSection.vue')),

  },
 
}
</script>
