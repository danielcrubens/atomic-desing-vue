<template>
  <div class=" components">
    <Header />
    <Presentation />
    <Services/>
    <Container></Container>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { Header } from '@/components/organisms'
import { Presentation } from '@/components/organisms'
import { Services } from '@/components/organisms'
import { Container } from '@/components/bosons'



export default defineComponent({
  components: { Header, Presentation,Services,Container }
})
</script>
<style lang="scss" scoped>
.components {
  margin: 3rem;
}
</style>
