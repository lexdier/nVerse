<script lang="ts" setup>
import FontAwesome from './FontAwesome.vue';

const cards = [
  { 
    price: '559',
    items: [
        "full acces",
        "Browse Website with ads",
        "Build static sites",
        "1 space",
        "10 MB storage",
        "75 MB data / month",
        "500 requests / month",
        "Subdomain",
    ]
  },
  { 
    price: '699',
    items: [
        "Browse Website with ads",
        "Build static sites",
        "10 space",
        "3 GB storage",
        "15 GB data / month",
        "200 000 requests / month",
        "Subdomain",
        "SSL certificate",
        "Access to HTML video",
        "Priority support",
    ]
  },
  { 
    price: '899',
    items: [
        "Browse Website with ads",
        "Build static sites",
        "20 spaces",
        "10 GB storage",
        "200 GB data / month",
        "500 000 requests / month",
        "Subdomain",
        "SSL certificate",
        "Access to HTML video",
        "Priority support",
        "Analytics"
    ]
  },
];
</script>

<template>
  <BRow style="gap: 1em;">
    <BCol cols="12" class="text-center">
      <h1>Services and pricing</h1>
    </BCol>
      <template v-for="card in cards">
        <BCol>
          <BCard class="shadow-lg gradient text-white" style="border-radius: 2em;">
            <BCardTitle class="text-center">
              <span>$</span>
              <span v-text="card.price" class="font-weight-bold"/>
              <span class="text-muted">/pack</span>
            </BCardTitle>
            <BCardBody>
             <BListGroup tag="ul">
              <template v-for="(item, index) in card.items">
                <BListGroupItem :class="`text-${item} p-2`" class="border-0 fs-xs gradient" tag="li">
                  <FontAwesome name="check"/>
                  <span v-text="item"/>
                </BListGroupItem>
               </template>
              </BListGroup>
            </BCardBody>
          </BCard>
        </BCol>
    </template>
  </BROw>
</template>

<style> 
.gradient{
    background: -webkit-linear-gradient(left, #1d40da, #0d1b6b) !important; 
    background: linear-gradient(to right, #1d40da, #0d1b6b) !important; 
}
</style>
