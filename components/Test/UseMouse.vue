<template>
<div>
  <p>Mouse: X: {{ x }}, y:{{ y }}</p>
</div>
</template>

<script>
import {useMouse} from "@vueuse/core";

export default {
  name: "TestUseMouse",
  setup() {
      const { x, y } = useMouse()

      return {
        x, y
      }
  }

}
</script>

<style scoped>

</style>
