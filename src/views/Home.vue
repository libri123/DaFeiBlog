<template>
  <div class="home">
    <Intro/>
    <Work/>
    <Education/>
  </div>
</template>

<script>
// @ is an alias to /src
import Intro from '@/components/Intro.vue';
import Work from '../components/Work.vue';
import Education from '../components/Education.vue';

export default {
  name: 'Home',
  components: {
    Intro,
    Work,
    Education
  }
}
</script>
