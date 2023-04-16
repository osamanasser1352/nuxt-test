<template>
  <div>
    <navbar name="Home" :num="index" />
    <tutorial :date="data" />
    <div>{{ ahmed }}</div>
    <the-footer :title="title" />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      index: 15,
      title:'home',
      ahmed:null,
      array:[],
      object:{},
      boolean:true,
      data:[
        {
          name:'ahmed',
          age:'15'
        },
        {
          name:'ahmed 2',
          age:'15'
        },
        {
          name:'ahmed 3',
          age:'15'
        }
      ]
    }
  },

}
</script>
