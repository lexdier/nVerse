<script lang="ts" setup>
//@ts-ignore
import img1 from 'assets/img-1.jpg';
//@ts-ignore
import img2 from 'assets/img-2.jpg';
//@ts-ignore
import img3 from 'assets/img-3.jpg';
//@ts-ignore
import img4 from 'assets/img-4.jpg';

</script>

<template>
    <BRow class="py-5">
        <BCol cols="4" class="d-flex align-items-center">
            <span class="text-uppercase font-weight-bolder h2">
                nVerse was <br> born from <br> the need <br> to turn <br> digital noise <br> into clear <br> messages
            </span>
        </BCol>
        <BCol cols="8">
            <BCarousel
              :interval="4000"
              controls
              indicators
              background="#ababab"
              style="text-shadow: 1px 1px 2px #333;">
                <BCarouselSlide class="h-100">
                    <template #img>
                      <BImg
                        class="w-100"
                        fluid
                        :src="img1"
                        alt="image slot"
                        style="height: 25em;"
                      />
                    </template>
                  </BCarouselSlide>

                  <BCarouselSlide class="h-100">
                    <template #img>
                      <BImg
                        class="w-100"
                        fluid
                        :src="img2"
                        alt="image slot"
                        style="height: 25em;"
                      />
                    </template>
                  </BCarouselSlide>

                  <BCarouselSlide class="h-100">
                    <template #img>
                      <BImg
                        class="w-100"
                        fluid
                        :src="img3"
                        alt="image slot"
                        style="height: 25em;"
                      />
                    </template>
                  </BCarouselSlide>

                  <BCarouselSlide class="h-100">
                    <template #img>
                      <BImg
                        class="w-100"
                        fluid
                        :src="img4"
                        alt="image slot"
                        style="height: 25em;"
                      />
                    </template>
                </BCarouselSlide>
            </BCarousel>
        </BCol>
    </BRow>
</template>
