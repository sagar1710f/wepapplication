<template>
<div>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#">Movies</b-navbar-brand>
    <b-navbar-brand href="#"></b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
        </b-nav-form>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>    
</template>

<script>
export default {
 name: 'Navigation',
}
</script>

<style>

</style>
