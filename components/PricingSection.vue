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
  <BContainer class="py-5" style="position: relative;">
    <BRow>
      <BCol lg="12" class="text-center">
        <h1>Services and pricing</h1>
      </BCol>
        <template v-for="card in cards">
          <BCol lg="4" md="12">
            <BCard class="shadow-lg gradient text-white text-md-center" style="border-radius: 2em;">
              <BCardTitle class="text-center">
                <span>$</span>
                <span v-text="card.price" class="font-weight-bold"/>
                <span class="text-muted">/pack</span>
              </BCardTitle>
              <BCardBody>
               <BListGroup tag="ul">
                <template v-for="(item, index) in card.items">
                  <BListGroupItem :class="`text-${item} p-2`" class="border-0 fs-xs bg-transparent" tag="li">
                    <FontAwesome name="check"/>
                    <span v-text="item"/>
                  </BListGroupItem>
                 </template>
                </BListGroup>
              </BCardBody>
            </BCard>
          </BCol>
      </template>
    </BRow>
    <BLink to="#" class="gradient link" style="
            position: absolute;
            height: 10em;
            width: 24em;
            cursor: pointer;
            top: 0px;
            right: -50%;
            border-radius: 40px 0 0 40px;
            "/>
    <BLink to="#" class="gradient" style="
            position: absolute;
            height: 5em;
            width: 25em;
            cursor: pointer;
            top: 0px;
            left: -50%;
            border-radius: 0 40px 40px 0;
            "/>
    <BLink to="#" class="gradient" style="
            position: absolute;
            width: 20em;
            height: 10em;
            cursor: pointer;
            bottom: 0px;
            left: -50%;
            border-radius: 0 40px 40px 0;
              "/>
    <BLink to="#" class="gradient" style="    
            position: absolute;
            width: 24em;
            height: 5em;
            cursor: pointer;
            right: -50%;
            bottom: 0px;
            border-radius: 40px 0 0 40px;
            "/>
  </BContainer>
</template>

<style> 
.gradient{
    background: -webkit-linear-gradient(left, #1d40da, #071042) !important; 
    background: linear-gradient(to right, #1d40da, #071042) !important; 
}
</style>
