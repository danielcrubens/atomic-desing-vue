<template>
  <div class="presentation">
    <SocialNetworks />

    <img class="ilustration" src="@/assets/images/presentation.svg" alt="Apresentação" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { SocialNetworks } from "@/components/molecules";

export default defineComponent({
  components: { SocialNetworks }
});
</script>

<style lang="scss" scoped>
  @mixin sm {
  @media (max-width: 575px) {
    @content;
  }
}
.presentation {
  position: relative;
  display: grid;
  justify-content: center;

  .presentation {
    width: 100%;
    justify-self: center;
  }

  .socialNetworks {
    @include sm{
      display: none;
    }
    position: absolute;
    left: 0;
    top: 50%;
    transform: translateY(-50%);
  }

  .ilustration {
    @include sm{
      width: 100%;
    }
    width: 48rem;
  }
}
</style>