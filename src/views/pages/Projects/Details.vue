<template>
    <div id="projects-details">
      <img class="body-cover absolute" src="@/assets/img/global/grid.svg" alt="">
        <HeadSection :Title="`Project Details`" />
      <Details />
     </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
  name: 'Project Details Page',
  data(){
    return{
    }
  },
  components: {
    Details: defineAsyncComponent( () => import(/* webpackChunkName: "App" */'@/components/Pages/Projects/Details/Details.vue') ),
    HeadSection: defineAsyncComponent(() => import(/* webpackChunkName: "App" */'@/components/Global/HeadSection.vue')),

  },
 
}
</script>
