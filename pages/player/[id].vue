<script setup lang="ts">
const route = useRoute();
let urlSlug = route.params.id;

let { data } = useFetch(`${process.env.API_URL}/api/player/${urlSlug}`);

console.log(urlSlug);
</script>

<template>
  <div>
    {{ data }}
  </div>
</template>