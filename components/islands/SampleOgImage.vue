<template>
  <div
    :style="{
      position: 'relative',
      backgroundColor: '#aacaef',
      width: '100%',
      height: '100%',
      display: 'flex',
      flexDirection: 'column',
      padding: '60px',
    }"
  >
    <div
      :style="{
        height: '100%',
        paddingBottom: '120px',
        display: 'flex',
        flexDirection: 'column',
        justifyContent: 'center',
        alignItems: 'center',
        position: 'relative',
      }"
    >
      <div
        :style="{
          display: 'flex',
          flexDirection: 'column',
          justifyContent: 'center',
          alignItems: 'center',
          maxWidth: '680px',
        }"
      >
        <p
          :style="{
            fontSize: '72px',
            fontWeight: '700',
            marginTop: '0',
            marginBottom: '10px'
          }"
        >
          {{ name }}
        </p>
        <p
          :style="{
            fontSize: '40px',
            fontWeight: '400',
            margin: '0',
            textAlign: 'center',
          }"
        >
          {{ description }}
        </p>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  name: String,
  description: String,
});
</script>