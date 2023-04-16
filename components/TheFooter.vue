<template>
    <div class="w-100 bg-dark text-white d-flex align-items-center justify-content-center  fixed-bottom">
         <h1>Footer {{ title }}</h1>
    </div>
 </template>

 <script>
    export default {
        props: {
            title:{
                type: String,
                required: true,
                default: 'Nav'
            }
        }
    }
</script>