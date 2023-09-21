<template>
  <div class=" services">
    <Service title="Front End"
      description="Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reiciendis officia, corrupti similique eligendi animi porro quibusdam et temporibus aperiam magni? Enim nihil, " />

    <Service title="Back End"
      description="Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reiciendis officia, corrupti similique eligendi animi porro quibusdam et temporibus aperiam magni? Enim nihil, " />

    <Service title="Manutenção"
      description="Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reiciendis officia, corrupti similique eligendi animi porro quibusdam et temporibus aperiam magni? Enim nihil, " />
  </div>
</template>
  
<script lang="ts">
import { defineComponent } from 'vue'
import { Service } from '@/components/molecules'

export default defineComponent({
  components: { Service }
})
</script>
<style lang="scss" scoped>
  @mixin sm {
  @media (max-width: 575px) {
    @content;
  }
}
.services {
  @include sm{
    grid-template-columns: repeat(1, 1fr);
    grid-gap: 1rem;
  }
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 5rem;
}</style>