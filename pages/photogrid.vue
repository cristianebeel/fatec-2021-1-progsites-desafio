<template>
  <div>
    <PG-Header />
    <div class="grid grid-cols-3 gap-6">
      <Photo-Card v-for="item of photos" :key="item.title"
      :image="item.image"
      :alt="item.title"
      :title="item.title"
    />
    </div>
  </div>
</template>

<script>
import { mapState } from "vuex";

export default {
  name: "photogrid",

  computed: {
    ...mapState({
      photos: (state) => state.photos.photos
    })
  }
}
</script>