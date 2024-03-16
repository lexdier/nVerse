<script setup lang="ts">
import BlogSection from '~/components/BlogSection.vue';
import CarouselSection from '~/components/CarouselSection.vue';
import PresentationSection from '~/components/PresentationSection.vue';
import SectionContact from '~/components/SectionContact.vue';
import SectionPricing from '~/components/SectionPricing.vue';
import ServicesSection from '~/components/ServicesSection.vue';

</script>

<template>
  <main>
    <BContainer>
      <PresentationSection/>

      <ServicesSection/>

      <SectionContact/>

      <SectionPricing/>

      <CarouselSection/>

      <BlogSection/>
    </BContainer>
  </main>
</template>