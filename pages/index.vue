<script setup lang="ts">
import BlogSection from '~/components/BlogSection.vue';
import CarouselSection from '~/components/CarouselSection.vue';
import PresentationSection from '~/components/PresentationSection.vue';
import PricingSection from '~/components/PricingSection.vue';
import ServicesSection from '~/components/ServicesSection.vue';

</script>

<template>
  <main style="overflow: hidden;">
    <PresentationSection/>

    <ServicesSection/>

    <PricingSection/>

    <CarouselSection/>

    <BlogSection/>
  </main>
</template>