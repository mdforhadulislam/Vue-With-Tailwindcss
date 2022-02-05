<template>
  <Card
    name="Forhadul Islam"
    title="Frontend Developer"
    year="20"
    mobileNo="01930XXXXXX"
    :skills="[
      'HTML',
      'CSS ',
      'SCSS ',
      'JAVASCRIPT ',
      'BOOTSTRAP',
      'TAILWINDCSS',
      'REACT JS ',
      ' NEXT JS',
      'VUE JS',
      'REACT REDUX',
      'PYTHON',
    ]"
  />
</template>

<script>
import Card from "./Components/Card.vue";

export default {
  components: {
    Card,
  },
};
</script>
