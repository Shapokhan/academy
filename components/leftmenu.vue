<template>
   
    <b-container id="left_sidebar">
    <b-container class="sidebar_menu">
            <a href="#" v-b-toggle.accordion1><i class="panel_summary__icon"> </i> Management </a>
      <b-collapse id="accordion1" >
          <nuxt-link to="/Academics/Instructor/ManageInstructor">Manage Intstructor</nuxt-link>
      </b-collapse>

      <b-collapse id="accordion1">
          <nuxt-link to="/Academics/Courses/ManageCourses">Manage Courses</nuxt-link>
      </b-collapse>

        <b-collapse id="accordion1">
          <nuxt-link to="/Academics/Levels/ManageLevels">Manage Levels</nuxt-link>
      </b-collapse>


        <b-collapse id="accordion1">
         <nuxt-link to="/Academics/Lectures/ManageLectures">Manage Lectures</nuxt-link>
        </b-collapse>

        <b-collapse id="accordion1">
         <nuxt-link to="/Academics/Contents/ManageContents">Manage Contents</nuxt-link>
        </b-collapse>

            <a href="#news">News</a>
            <a href="#contact">Contact</a>
            <a href="#about">About</a>
       
        </b-container>
    </b-container>


  
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {}
};
</script>
<style lang="scss" scoped>

#left_sidebar {
  background-color: #282828;
  min-height: 500px;
  float: left;
  .sidebar_menu {
    div {
      a {
        border-bottom: 1px solid #363636;
        background-color: black; 
      }
    }
    a {
      border-bottom: 1px solid #363636;
      text-decoration: none;
      display: block;
      color: white;
      padding: 16px;
    }
    a:hover {
      color: white;
      background-color: #363636;
    }
  }
  .card-text a:hover {
    text-decoration: none;
    display: block;
    color: white;
    padding: 16px;
    background-color: #363636;
  }
}
</style>