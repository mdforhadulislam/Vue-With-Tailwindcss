<template>
  <li
    class="list-none w-auto pl-2 pr-2 pt-1 pb-1 shadow rounded inline-block m-1"
  >
    {{ skill }}
  </li>
</template>
<script>
export default {
  name: "Skill",
  props: ["skill"],
};
</script>
