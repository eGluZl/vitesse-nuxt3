<template>
  <div class="p-4">
    ha ha ha
  </div>
</template>

<script setup>
import { testAPI } from '~~/server/api/common'

const { data } = await useFetch(testAPI, {
  method: 'POST',
  params: {
    holder: '233',
  },
})

console.log(data.value)

</script>
