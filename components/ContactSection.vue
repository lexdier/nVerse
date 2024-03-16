<script lang="ts" setup>
import { BButton, BCardBody } from 'bootstrap-vue';


</script>

<template>
    <BRow class="py-5">
      <BCol cols="6" class="d-flex flex-column justify-content-between">
        <BCard no-body class="rounded-pill h-100 my-2 gradient text-white">
          <BCardBody>
            <div class="text-center text-uppercase font-weight-bolder">
              <span>Services and pricing</span>
            </div>

            <div class="d-flex justify-content-around">
              <div>
                <span class="font-weight-bolder">559</span>
                <span>$/pack</span>
              </div>
              <div>
                <span class="font-weight-bolder">699</span>    
                <span>$/pack</span>
              </div>
              <div>
                <span class="font-weight-bolder">899</span>
                <span>$/pack</span>
              </div>
            </div>
          </BCardBody>
        </BCard>

        <BCard no-body class="rounded-pill h-100 d-flex my-2 w-25 gradient text-white">
          <BCardBody class="d-flex align-items-center">
            <span class="text-uppercase font-weight-bolder h5">Blog</span>
          </BCardBody>
        </BCard>

        <BCard no-body class="rounded-pill h-100 my-2 w-50 gradient text-white">
          <BCardBody class="d-flex align-items-center">
            <span class="text-uppercase font-weight-bolder h5">Projects</span>
          </BCardBody>
        </BCard>
      </BCol>

      <BCol cols="6">
        <BRow style="gap: 2em;">
          <BCol cols=12>
            <BForm class="d-none d-md-inline-block w-100">
              <span class="h4">Contact direct by mail</span>
              <div class="input-group input-group-merge mt-3">
                <input
                  type="text"
                  class="form-control bg-light-green border-light-green w-250px"
                  placeholder="@your.email..."
                  aria-label="Search for any term"
                />
              </div>
            </BForm>
          </BCol>

          <BCol cols="12">
            <BForm class="d-none d-md-inline-block w-100">
              <span class="h4">Did you want call you back?</span>
              <div class="input-group input-group-merge mt-3">
                <input
                  type="number"
                  class="form-control bg-light-green border-light-green w-250px"
                  placeholder="let your phone number"
                  aria-label="Search for any term"
                />
              </div>
            </BForm>
          </BCol>

          <BCol>
            <div class="f-flex flex-column">
              <div class="text-uppercase font-weight-bolder">
                <span>No have time? Direct contact</span>
              </div>
              <div class="d-flex justify-content-between mt-3">
                <BButton variant="dark" class="rounded-pill">
                  <span>+1 786 353 5916</span>
                </BButton>
                <BButton variant="dark" class="rounded-pill">
                <span>info@nvers.com</span>
                </BButton>
              </div>
            </div>
          </BCol>
        </BRow>
      </BCol>
    </BRow>
</template>

<style>
.gradient{
    background: -webkit-linear-gradient(left, #1d40da, #0d1b6b); 
    background: linear-gradient(to right, #1d40da, #0d1b6b); 
}</style>