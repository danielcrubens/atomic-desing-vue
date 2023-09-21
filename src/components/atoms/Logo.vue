<template>
  <img class="logo" src="@/assets/images/logo.svg" alt="Marcos" />
</template>


<style lang="scss" scoped>
@mixin md {
  @media (max-width: 1024px) {
    @content;
  }
}
.logo {
  @include md{
    width: 70%;
   
  }
  width: 100%;
}
</style>

