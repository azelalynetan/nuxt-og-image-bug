<template>
  <div>
    <h1>Nuxt Og Image Bug Reproduction</h1>
    <div>
      <iframe
        src="/__og_image__"
        style="width: 100%; border: none; height: 800px"
      >
      </iframe>
    </div>
  </div>
</template>

<script setup>
defineOgImageStatic({
  component: 'SampleOgImage',
  name: 'My Profile 😊',
  description: 'Sample Description 🖊',

});

useHead({
  title: 'My Profile 😊',
  meta: [
    {
      name: 'description',
      content: 'Sample Description 🖊',
    },
    {
      property: 'og:title',
      content: 'My Profile 😊',
    },
    {
      property: 'og:description',
      content: 'Sample Description 🖊',
    },
  ],
});
</script>