<template>
  <div>
    <navbar name="Home" :num="index" />
    <tutorial :date="data" @dataHere="dataget" />
    <div>{{ ahmed }}</div>
    <div>
      <div>
        <ul v-for="(item , index) in array" :key="index">
          <li>{{ index }} {{ item.name }} {{ item.age }}</li>
        </ul>
      </div>
    </div>
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
  methods: {
    dataget(data){
      console.log(data)
      this.array = data
    }
  },

}
</script>
