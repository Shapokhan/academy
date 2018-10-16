<template>
  <b-navbar toggleable="md" type="dark" class="siteheader">

  <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

  <b-navbar-brand href="/">KPCoders</b-navbar-brand>

  <b-collapse is-nav id="nav_collapse">
    <b-navbar-nav class="navbaritems">
      <b-nav-item><nuxt-link to="/Academics">Academics</nuxt-link></b-nav-item>
      <b-nav-item><nuxt-link to="/Accounts">Accounts</nuxt-link></b-nav-item>
      <b-nav-item><nuxt-link to="/Students">Students</nuxt-link></b-nav-item>
      <b-nav-item><nuxt-link to="/HumanResources">HumanResource</nuxt-link></b-nav-item>
    </b-navbar-nav>

    <!-- Right aligned nav items -->
    <b-navbar-nav class="ml-auto">

      <b-nav-form>
        <b-form-input size="sm" class="mr-sm-2" type="text" placeholder="Search"/>
        <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
      </b-nav-form>

      <b-nav-item-dropdown text="Lang" right>
        <b-dropdown-item href="#">EN</b-dropdown-item>
        <b-dropdown-item href="#">ES</b-dropdown-item>
        <b-dropdown-item href="#">RU</b-dropdown-item>
        <b-dropdown-item href="#">FA</b-dropdown-item>
      </b-nav-item-dropdown>

      <b-nav-item-dropdown right>
        <!-- Using button-content slot -->
        <template slot="button-content">
          <em>User</em>
        </template>
        <b-dropdown-item href="#">Profile</b-dropdown-item>
        <b-dropdown-item href="#">Signout</b-dropdown-item>
      </b-nav-item-dropdown>
    </b-navbar-nav>

  </b-collapse>
</b-navbar>
</template>

<script>
export default {

}
</script>

<style <style lang="scss" scoped>
@import "./assets/_variables";
.navbaritems
{
  a{
    color: white;
    :hover{
      text-decoration: none;
      color: black;
    }
  }

}
.siteheader
{
  background-color: #282828;
  border: 1px solid black;
  margin: $margin;
  
}


</style>
