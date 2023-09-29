<template>
  <div>
    <select v-model="$i18n.locale">
      <option v-for="(lang, i) in langs" :key="`lang-${i}`" :value="lang.value">
        {{ lang.name }}
      </option>
    </select>
  </div>
</template>

<script setup>
import { reactive } from "vue";

const langs = reactive([
  {
    name: "english",
    value: "en",
  },
  {
    name: "indonesia",
    value: "id",
  },
]);
</script>
