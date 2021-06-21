<template>
  <g-map
  :disableUI="false"
  :zoom="12"
  mapType="roadmap"
  :center="{ lat: 38.8977859, lng: -77.0057621 }">
</g-map>
</template>

<script>


import Gmap from '../components/Gmap.vue'

export default defineComponent({
  components: { GoogleMap, Marker },
  setup() {
    const center = { lat: 40.689247, lng: -74.044502 }

    return { center }
  },
  name: 'App',
  components: {
    Gmap
  },
})
</script>