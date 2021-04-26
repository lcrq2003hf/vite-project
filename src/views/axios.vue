<template>
  <div>触发调试</div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
import axios from '../utils/axios'

export default defineComponent({
  setup() {
    axios
      .get('/users/XPoet')
      .then((res) => {
        // eslint-disable-next-line no-console
        console.log('res:', res)
      })
      .catch((err) => {
        // eslint-disable-next-line no-console
        console.error('err:', err)
      })
  }
})
</script>
