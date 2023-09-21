<template>
  <nav class=" nav-bar">
    <NavItem text="Serviços" to="/services" />
    <NavItem text="Sobre mim" to="/about" />
    <NavItem text="Cases" to="/cases" />
    <NavItem text="Contato" to="/contact" />
  </nav>
  </template>
  
  <script lang="ts">
  import { defineComponent } from 'vue'
  import { NavItem } from '@/components/atoms'
  
  export default defineComponent({
  components:{
    NavItem
  }
  })
  </script>

  <style lang="scss" scoped>
    @mixin sm {
  @media (max-width: 575px) {
    @content;
  }
}
  .nav-bar {
    @include sm{
      display:none
    }
  width: max-content;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 2.5rem;
}
  </style>