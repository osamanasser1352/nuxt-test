<!-- Please remove this file from your project -->
<template>
  <div class="h-100">
    <h1>tutoril</h1>
    <div v-if="date">
      <ul v-for="(item , index) in date" :key="index">
        <li>{{ index }} {{ item.name }} {{ item.age }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NuxtTutorial',
  props: {
    date:{
          type: Array,
          required: true
      }
  }
}
</script>
