<template>
  <div class="slidev-layout video-fullscreen h-full relative overflow-hidden bg-black">
    <div class="absolute inset-0 flex items-center justify-center">
      <video 
        controls 
        autoplay
        class="w-full h-full object-contain"
      >
        <source :src="resolveAssetUrl(video)" type="video/mp4">
      </video>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  video: {
    type: String,
    required: true
  }
})

const resolveAssetUrl = (url) => {
  if (url.startsWith('/')){
    return import.meta.env.BASE_URL + url.slice(1)
  }
  return url
}
</script>
