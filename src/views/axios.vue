<template></template>
<script lang="ts">
import { defineComponent } from 'vue'
import axios from '../utils/axios'

export default defineComponent({
  setup() {
    console.log('axios', axios)
    axios
      .get('/users/monstereat')
      .then((res) => {
        console.log('res: ', res)
      })
      .catch((err) => {
        console.log('err: ', err)
      })
  },
})
</script>
