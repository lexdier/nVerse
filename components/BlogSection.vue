
<script lang="ts" setup>

</script>

<template>
    <BContainer>
    <BRow class="py-5">
      <BCol lg="6" md="12" class="d-flex flex-column">
          <span class="h3 font-weight-bolder">Blog</span>
          <BCard style="border-radius: 1em;" class="mt-3 w-75 align-self-center shadow-lg">
              <p>
                  Our philosophy is based on the idea
                  that to reveal the greatness of what
                  we can see and experience, we must
                  rst understand and appreciate the
                  tiniest, most hidden details.
                  Our philosophy is based on the idea
                  that to reveal the greatness of what
                  we can see and experience, we must
                  rst understand and appreciate the
                  tiniest, most hidden details. 
              </p>
          </BCard>
      </BCol>
      <BCol lg="6" md="12" class="d-flex flex-column align-items-center mt-3" style="gap: 1em;">
          <BCard class="rounded-pill w-75 h-100 gradient"/>
          <BCard class="rounded-pill w-75 h-100 gradient"/>
          <BCard class="rounded-pill w-75 h-100 gradient"/>
      </BCol>
    </BRow>
    </BContainer>
</template>

<style>
.gradient{
    background: -webkit-linear-gradient(left, #1d40da, #071042); 
    background: linear-gradient(to right, #1d40da, #071042); 
}
</style>