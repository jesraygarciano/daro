<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/> -->
    <Dashboard msg="Welcome to Dashboard" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
// import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import Dashboard from '@/components/Dashboard.vue'

@Component({
  components: {
    // HelloWorld,
    Dashboard
  },
})
export default class Home extends Vue {}
</script>
