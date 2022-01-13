<template>
  <div class="p-4">
    ha ha ha
  </div>
</template>

<script setup>
import { testAPI } from '~~/server/api/common'

onBeforeUnmount(async() => {
  const { data } = await useFetch(testAPI, {
    method: 'GET',
  })
  localStorage.setItem('kjok', JSON.stringify(data.value))
})

</script>
