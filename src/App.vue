<template>
  <div class=" components">
    <Header />
    <Presentation />
    <Services/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Header } from '@/components/organisms'
import { Presentation } from '@/components/organisms'
import { Services } from '@/components/organisms'


export default defineComponent({
  components: { Header, Presentation,Services }
})
</script>
<style lang="scss" scoped>
.components {
  margin: 3rem;
}
</style>
