<template>
  <header class="radius element2">
    <div class="bg-dark-blue element2 md:pr-2">
        <span class="nav-item logo" data-id="er_menu" aria-controls="er_menu"></span>

      <scrollactive class="vam nav scroll element2 font-display font-bold" active-class="active"
  :offset="80"
  :duration="800"
  bezier-easing-value=".5,0,.35,1">
        <a class="nav-item scrollactive-item" href='#edgeryders'>Welcome</a>
        <a class="nav-item scrollactive-item" href='#current'>Upcoming</a>
        <a class="nav-item scrollactive-item" href='#people'>People</a>
        <a class="nav-item scrollactive-item" href='#connect'>Connect</a>
        <a class="nav-item scrollactive-item" href='#mission'>Mission</a>
        <a class="nav-item scrollactive-item" href='#projects'>Projects</a>
        <a class="nav-item scrollactive-item" href='#social'>Follow Us</a>
</scrollactive>

    </div>
    </div>

  </header>
</template>

<script>
/**
 * Used as main page navigation in templates.
 */
export default {
  name: "Navigation",
  status: "ready",
  release: "1.0.0",
  model: {
    prop: "activeNav",
  },
  inheritAttrs: true,
  data() {
    return {
      active: 'welcome'
    }
  },
  methods: {
    activate:function(el){
        this.active = el;
    },
    emit: function() {
      this.$emit('event_child', 1)
    }
  },
   mounted: function () {

  },
  computed: {
    localActive: {
      get() {
        return this.active
      },
      set(val) {
        this.$emit("input", val)
      },
    },
  },
}
</script>

<style lang="scss" scoped>


.scroll {
  white-space: nowrap;
  overflow-x: scroll;
  width: auto;
  overflow-y: hidden;
  -webkit-overflow-scrolling: touch;
  -ms-overflow-style: -ms-autohiding-scrollbar; 
  .nav-item {
    height: 45px;
    display: inline-flex; 
    align-items: center;
    color: black !important;
    border-right: 1px solid rgba(0,0,0,0.05) !important
  }
}
  
.nav-item.active {
  color: #fff !important;
 border-radius: 5px;
  background-color: black; }

.bg-dark-blue {
  background-color: #fff;
  display: flex;
  position: fixed;
  top: 0;
  border-bottom: 1px solid rgba(0,0,0,0.05) !important;
  z-index: 11;
  justify-content: space-between;
  width: 100%;
  align-items: center;
  }

.nav-item {
  display: inline-block;
  vertical-align: middle; }
  
/**
 * Example specific
 */
.logo {
  min-width: 65px; 
  height: 60px;
  padding: 0 50px 0 20px;
background: url("data:image/svg+xml,%3Csvg viewBox='0 0 500 500' version='1' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='orangered' d='M0 250a250 250 0 1 1 500 0 250 250 0 0 1-500 0zm250 183V250H67a183 183 0 1 1 183 183z' fill-rule='evenodd'/%3E%3C/svg%3E") no-repeat center #fafafa;
background-size: 45%;transition: none;
box-shadow: none !important;
left: 0;
z-index: 99999;
}
.logo.active {
  background: url("data:image/svg+xml,%3Csvg viewBox='0 0 500 500' version='1' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='white' d='M0 250a250 250 0 1 1 500 0 250 250 0 0 1-500 0zm250 183V250H67a183 183 0 1 1 183 183z' fill-rule='evenodd'/%3E%3C/svg%3E") no-repeat center orangered;
border-right: 1px solid #727c87 !important;
box-shadow: none !important;
background-size: 45%;
transition: none;
}
/**
 * Visual style
 */
.logo {

  border-right: 1px solid rgba(255,255,255,0.28);
  }

.nav-item {
  cursor: pointer;
  padding: 16px 16px 14px; }

.nav-item:not(:last-child) {
  border-right: .5px solid rgba(255,255,255,0.2); }
  
  .bg-grey .nav-item { color: #fff; }


header,
nav {
  font-size: 0; }

.logo,
.nav-item {
  font-size: 16px; }


/**
 * Setup
 */
* {
  box-sizing: border-box; }

a { 
  color: #fff;
  text-decoration: none; }

ul, li { list-style: none; margin: 0; padding: 0; }


@media only screen and (max-width: 600px) {
    .featured {
      width: 85%;
      float: none;
    }
}

// Demo purposes only, proceed with caution on Windows!
.scroll::-webkit-scrollbar {
  display: none; }


</style>
