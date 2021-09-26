<template>
  <div class="home" style="height: 100vh; background: rgba(34, 34, 34, 1)">
    <b-container fluid class="h-100">
      <b-row cols="12" class="h-100">
        <b-col cols="3" class="text-light">
          <h1>sidebar</h1>
        </b-col>
        <b-col cols="9" class="h-100" style="">
          <b-navbar toggleable="lg" type="dark">
            <b-navbar-brand href="#">NavBar</b-navbar-brand>
          </b-navbar>
            <div
              class="d-inline-block w-100 bg-light p-4"
            >
              <h1>Home</h1>
            </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {};
</script>
