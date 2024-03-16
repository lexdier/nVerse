<script setup lang="ts">
import CarouselSection from '~/components/CarouselSection.vue';
import SectionContact from '~/components/SectionContact.vue';
import SectionPricing from '~/components/SectionPricing.vue';

</script>

<template>
  <main>
    <BContainer>
      <SectionContact/>

      <SectionPricing/>

      <CarouselSection/>
    </BContainer>
  </main>
</template>