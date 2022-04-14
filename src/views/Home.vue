<template>
  <div class="home">
    <Intro/>
    <Work/>
  </div>
</template>

<script>
// @ is an alias to /src
import Intro from '@/components/Intro.vue';
import Work from '../components/Work.vue';

export default {
  name: 'Home',
  components: {
    Intro,
    Work
  }
}
</script>
