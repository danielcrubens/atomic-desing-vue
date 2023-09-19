<template>
  <div class="socialNetworks">
    <SocialLink name="GitHub" link="https://github.com" icon="github.svg" />
    <SocialLink name="Facebook" link="https://facebook.com" icon="facebook.svg" />
    <SocialLink name="Twitter" link="https://twitter.com" icon="twitter.svg" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { SocialLink } from "@/components/atoms";

export default defineComponent({
  components: { SocialLink }
});
</script>

<style lang="scss" scoped>
.socialNetworks {
  display: grid;
  grid-gap: 1rem;
}
</style>