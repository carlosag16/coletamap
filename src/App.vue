<template>
  <div id="material-kit">
    <div :class="{ 'nav-open': NavbarStore.showNavbar }">
      <router-view name="header" />
      <div>
        <router-view />
      </div>
      <router-view name="footer" />
    </div>
  </div>
  
</template>

<script>
// import Map from './components/Map';
// export default {
//   name: 'App',
//   components: {
//     Map
//   }
// }
</script>

