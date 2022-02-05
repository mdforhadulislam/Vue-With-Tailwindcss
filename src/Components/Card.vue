<template>
  <div
    class="w-1/4 p-4 border rounded-xl font-sans shadow m-4 inline-block relative"
  >
    <div class="mb-2">
      <div class="p-3 border shadow rounded bg-emerald-600">
        <span class="text-3xl font-semibold text-blue-50">{{ name }}</span>
        <span class="ml-1 font-medium text-blue-50">{{ year }}years</span>
      </div>
      <div class="block font-medium text-base">{{ title }}</div>
    </div>
    <div class="text-lg font-medium">Mobile No: {{ mobileNo }}</div>
    <div class="mb-2 mt-1">
      <span class="font-medium text-lg">Sklls: </span>
      <div v-for="skill in skills" :key="skill" class="inline-block">
        <Skill :skill="skill" />
      </div>
    </div>
    <div class="w-full h-16"></div>
    <div
      class="w-full h-20 shadow bg-emerald-600 rounded-br-xl rounded-bl-xl absolute bottom-0 left-0"
    ></div>
  </div>
</template>

<script>
import Skill from "./Skill.vue";
export default {
  name: "Card",
  props: ["title", "name", "year", "mobileNo", "skills"],
  components: {
    Skill,
  },
};
</script>
