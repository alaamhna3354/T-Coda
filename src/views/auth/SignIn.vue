<template>
    <div id="Auth">
        <SignIn />
    </div>
  </template>
  
  <script>
  import { defineAsyncComponent } from 'vue'
  
  export default {
    name: 'Sign In Page',
    data() {
      return {
      }
    },
    components: {
      SignIn: defineAsyncComponent(() => import(/* webpackChunkName: "App" */'@/components/auth/SignIn.vue')),
  
    },
  
  }
  </script>
  