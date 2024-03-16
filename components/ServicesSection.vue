<script lang="ts" setup>
import { BButton, BCardBody } from 'bootstrap-vue';


</script>

<template>
    <BRow class="py-5">
      <BCol cols="6" class="d-flex flex-column justify-content-between">
        <BCard no-body class="rounded-pill h-100 my-2 gradient text-white contenedor">
          <BCardBody class="d-flex align-items-center">
              <span class="text-uppercase font-weight-bolder h5">Services</span>
              <div class="previsualizacion">
              <p>Preview</p>
            </div>
          </BCardBody>
        </BCard>

        <BCard no-body class="rounded-pill h-100 d-flex my-2 w-25 gradient text-white contenedor">
          <BCardBody class="d-flex align-items-center">
            <span class="text-uppercase font-weight-bolder h5">Blog</span>
            <div class="previsualizacion">
              <p>Preview</p>
            </div>
          </BCardBody>
        </BCard>

        <BCard no-body class="rounded-pill h-100 my-2 w-50 gradient text-white contenedor">
          <BCardBody class="d-flex align-items-center">
            <span class="text-uppercase font-weight-bolder h5">Projects</span>
            <div class="previsualizacion">
              <p>Preview</p>
            </div>
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
                  type="text"
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
}
.contenedor {
    position: relative;
    width: 200px; /* Ancho de ejemplo */
    height: 200px; /* Altura de ejemplo */
    overflow: hidden;
    transition: 0.3s ease;
}

.imagen {
    width: 100%;
    height: 100%;
    transition: transform 0.3s ease;
}
.previsualizacion {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.7);
    color: white;
    opacity: 0;
    transition: opacity 0.3s ease;
    display: flex;
    justify-content: center;
    align-items: center;
}

.contenedor:hover {
  transform: scale(1.2);
}

.contenedor:hover .previsualizacion {
    opacity: 1;
}
</style>