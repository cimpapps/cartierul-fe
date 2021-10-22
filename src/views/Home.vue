<template>
  <cio-blank-layout title="My Home Title">
    <slot>

    </slot>
  </cio-blank-layout>
</template>

<script lang="ts">
import { defineComponent } from "vue";

import CioBlankLayout from "../components/common/CioBlankLayout.vue";

export default defineComponent({
  components: {
    CioBlankLayout,
  },
});
</script>

<style scoped>
#container {
  text-align: center;

  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;

  color: #8c8c8c;

  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>