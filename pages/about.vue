<template>
    <div>
      <navbar name="About" />
      <tutorial @dataHere="myData" />
      <div>
        <ul v-for="(item , index) in myArray" :key="index">
          <li>{{ index }} {{ item.name }} {{ item.age }}</li>
        </ul>
      </div>
      <the-footer />
    </div>
</template>
  
  <script>
  export default {
    // name: 'IndexPage'
    data() {
        return {
            myArray:[]
        }
    },
    methods: {
        myData(data){
            this.myArray = data
        }  
    },
    created() {
        
    },
    mounted() {
        
    },
  }
  </script>
  