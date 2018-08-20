<template>
  <div>
    <h1>Map</h1>

  </div>
</template>

<script>

import ChildMarker from './ChildMarker'
import Heatmap from './Heatmap'
export default {
  props: {
    markers: Array
  },
  data(){
    return {
      mapConfig: {
        zoom: 12,
        center: this.markers[0]
      }
    }
  },
  components: {
    ChildMarker,
    Heatmap
  }
}
</script>

