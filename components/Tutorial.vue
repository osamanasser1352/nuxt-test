<!-- Please remove this file from your project -->
<template>
  <div class="h-100">
    <div>
      <h1>tutoril</h1>
      <div v-if="date">
        <ul v-for="(item , index) in date" :key="index">
          <li>{{ index }} {{ item.name }} {{ item.age }}</li>
        </ul>
      </div>
      <div v-else>No Data</div>
    </div>

    <div>
      <a class="btn btn-danger btn-sm" @click="clickHere">Click</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NuxtTutorial',
  props: {
    date:{
          type: Array,
          required: false,
          default: []
      }
  },
  data() {
    return {
      array:[
      {
          name:'nasser',
          age:'15'
        },
        {
          name:'nasser 2',
          age:'15'
        },
        {
          name:'nasser 3',
          age:'15'
        }
      ]
    }
  },
  methods: {
    clickHere(){
      this.$emit('dataHere',this.array)
    }
  },
}
</script>
