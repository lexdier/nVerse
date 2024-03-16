<script setup lang="ts">
</script>

<template>
  <section>
    <BContainer class="py-2">
      <BRow align-v="center" class="justify-content-between">
        <BCol cols="auto">
          <BNavbarBrand>
            <span class="text-uppercase h1 user-select-none cursor-pointer">NVerse</span>
          </BNavbarBrand>
        </BCol>
        <BCol cols="8">
          <BForm class="d-none d-md-inline-block w-100">
            <div class="input-group input-group-merge">
              <input
                type="text"
                class="form-control bg-light-green border-light-green w-250px"
                placeholder="Search..."
                aria-label="Search for any term"
              />
            </div>
          </BForm>
        </BCol>
        
        <BCol cols="auto">
          <BDropdown
            no-caret
            size="sm"
            toggle-class="text-decoration-none"
            variant="link">
            <template #button-content>
              <BAvatar class="avatar-img avatar-lg rounded-circle" size="40px" style="background-color: #0d1b6b;"/>
            </template>
          
            <BDropdownItem>
              <span>Log In</span>
            </BDropdownItem>
            <BDropdownItem>
              <span>Log Out</span>
            </BDropdownItem>
          </BDropdown>
        </BCol>
      </BRow>
    </BContainer>
  </section>
</template>