<script lang="ts" setup>

</script>

<template>
  <BContainer>
    <BRow class="py-5">
      <BCol md="12" lg="5" class="d-flex flex-column justify-content-center align-items-center">
        <span class="text-uppercase font-weight-bolder h1 fs-1 text-gradient" style="font-size: 7em;">NVerse</span>
        <p class="h6">From the invisible to the immense</p>
      </BCol>
      <BCol md="12" lg="7" class="d-flex w-100 align-items-center" style="column-gap: 2em;">
        <BCard class="rounded-pill gradient w-100" style="height: 14em;"></BCard>
        <BCard class="rounded-pill gradient w-100" style="height: 20em;"></BCard>
        <BCard class="rounded-pill gradient w-100" style="height: 17em;"></BCard>
        <BCard class="rounded-pill gradient w-100" style="height: 12em;"></BCard>
      </BCol>
    </BRow>
  </BContainer>
</template>

<style>
.gradient{
    background: -webkit-linear-gradient(left, #1d40da, #071042); 
    background: linear-gradient(to right, #1d40da, #071042); 
}
.text-gradient{
  background: linear-gradient(45deg, #071042, #1d40da);
  -webkit-background-clip: text;
  background-clip: text; /* Clip de fondo al texto */
  color: transparent; 
}
</style>
