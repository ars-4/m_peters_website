<template>
  <NavigationBar />
  <router-view/>
  <div class="footer bg-dark text-light small text-center">
    <span>Copyright © All Rights Reserved {{ new Date().getFullYear() }}</span>
  </div>
</template>

<script>

import { defineComponent } from 'vue';

import NavigationBar from '@/components/NavBar.vue';

export default defineComponent({
  components: {
    NavigationBar
  }
})

</script>

