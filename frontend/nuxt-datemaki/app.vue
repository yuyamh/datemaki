<template>
  <div>
    <p>{{data}}</p>
  </div>
</template>

<script setup>
    const config = useRuntimeConfig();
    const {data} = await useFetch(config.public.url + '/check');
</script>
