<script lang="ts" setup>
import FontAwesome from './FontAwesome.vue';

const socials = [
  { icon: 'facebook', url: '#' },
  { icon: 'instagram', url: '#' },
  { icon: 'youtube', url: '#' },
]

const menus = [
  {
    title: 'Landings',
    items: [
      { title: 'Saas', to: '#' },
      { title: 'Software Company', to: '#' },
      { title: 'Finance', to: '#' },
      { title: 'Digital Agency', to: '#' },
      { title: 'Conference', to: '#' },
    ]
  },
   {
    title: 'Accounts',
    items: [
      { title: 'Register', to: '#' },
      { title: 'Login', to: '#' },
      { title: 'Forgot Password', to: '#' },
      { title: 'Reset Password', to: '#' },
      { title: 'Profile', to: '#' },
    ]
  },
{
  title: 'Resources',
    items: [
      { title: 'Docs', to: '#' },
      { title: 'Support', to: '#' },
      { title: 'Changelog', to: '#' },
      { title: 'Help Center', to: '#' },
      { title: 'Community', to: '#' },
       { title: 'Webinars', to: '#' }
    ]
  },
]
</script>

<template>
  <footer class="footer mt-5 py-3 border border-top-3">
    <BContainer>
      <BRow>
        <BCol cols="12">
          <BNavbarBrand class="py-0 mb-3 mb-md-4">
           <span>NVerse</span>
          </BNavbarBrand>
        </BCol>

        <BCol md="4" lg="3" class="pb-2 pb-md-0 mb-4 mb-md-0">
          <p class="fs-sm">
            "As good minimalists, we have reduced this page to nothing. Another try?”
          </p>

          <p>
            Avenida Campos Salles,
            <br>
            CEP: 86720-000
            <br>
            Super Copo Acrílico
            <br>
            CNPJ: 20.661.615/001-76
          </p>

          <div class="d-flex">
            <template v-for="social in socials">
              <NuxtLink :to="social.url" class="rounded-circle btn-icon text-center" target="_blank" variant="secondary">
                <FontAwesome :name="social.icon" mode="brands" class="fs-4" variant="white" />
              </NuxtLink>
            </template>
          </div>
        </BCol>

        <BCol lg="7" md="8" offset-lg="2" offset-xl="3" xl="6">
          <BRow cols="1" cols-sm="3">
            <template v-for="(menu, key) in menus">
                <BCol class="mb-4 mb-md-0">
                    <h4 class="h6 fw-bold pb-lg-1">
                        <span v-text="menu.title"/>
                    </h4>

                    <BNav vertical>
                      <template v-for="(item, id) in menu.items">
                        <BNavItem link-classes="py-1 px-0" :to="item.to">
                          <div class="opacity-80" v-text="item.title" />
                        </BNavItem>
                      </template>
                    </BNav>
                </BCol>
            </template>
          </BRow>
        </BCol>
      </BRow>
    </BContainer>
  </footer>
</template>