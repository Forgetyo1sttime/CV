<template>
  <div class="container-fluid">
     <div class="row ">
        <skill v-for="skill in skills" v-bind:skill="skill" :key="skill.title"></skill>
    </div>
  </div>
</template>


<script>
import Skill from './Skill'

export default {
  name: "Skills",
  props: ['skills'],
  components: {
    Skill
  },
  data() {
    return {
      msg: "Skills",
      
    };
  }
};
</script>

