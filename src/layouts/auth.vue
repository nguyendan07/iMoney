<template>
  <brand-navigation />
  <slot />
</template>

<script>
import BrandNavigation from "../components/BrandNavigation.vue";

export default {
  components: { BrandNavigation },
};
</script>
