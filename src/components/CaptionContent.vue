<template>
    <div>
     <slot name="content">
        <img src="https://images.pexels.com/photos/50594/sea-bay-waterfront-beach-50594.jpeg?cs=srgb&dl=pexels-pixabay-50594.jpg&fm=jpg">;
     </slot>
     
     <p>
        <slot name="caption" v-bind:source="source">Caption</slot>
     </p>
    </div>
</template>

<script>
export default {
data() {
return {
  source: 'pixels.com',
  }
 },
}
</script>

<style>
img {
    width: 100%;
}
</style>