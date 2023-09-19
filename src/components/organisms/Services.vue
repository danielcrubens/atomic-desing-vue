<template>
  <div class=" services">
    <Service title="Front End"
      description="Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reiciendis officia, corrupti similique eligendi animi porro quibusdam et temporibus aperiam magni? Enim nihil, consequuntur eos ex nobis officia magni voluptatibus itaque!" />

    <Service title="Back End"
      description="Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reiciendis officia, corrupti similique eligendi animi porro quibusdam et temporibus aperiam magni? Enim nihil, consequuntur eos ex nobis officia magni voluptatibus itaque!" />

    <Service title="Manutenção"
      description="Lorem ipsum dolor, sit amet consectetur adipisicing elit. Reiciendis officia, corrupti similique eligendi animi porro quibusdam et temporibus aperiam magni? Enim nihil, consequuntur eos ex nobis officia magni voluptatibus itaque!" />
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
.services {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 5rem;
}</style>