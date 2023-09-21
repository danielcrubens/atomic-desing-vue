<template>
  <div class=" container">
  <slot/>
  </div>
  </template>  
  
  <style lang="scss" scoped>
    @mixin sm {
  @media (max-width: 575px) {
    @content;
  }
}
 .container {
  @include sm{
    width: 95%;
  }
  width: 85%;
  max-width: 1150px;
  margin: 0 auto;
}
  </style>