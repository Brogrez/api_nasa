<template>
  <div>
    <img :src="nasaData.url" alt="">
  </div>
</template>

<script>
export default {
name:"Image_Nasa",
data(){
    return {
        nasaData: {}
    }
},
methods:{
    async apiFetch(){
        try{
            let response = await fetch('https://api.nasa.gov/planetary/apod?api_key=NmsdTlDI4q2bfXFnXSsZETpkVlTLmH0HzkUPPAtd')
            let json =  await response.json();
            this.nasaData = json
            console.log(this.nasaData)
        } catch(error){
            console.log(error)
        }
    }
},
created(){
    this.apiFetch()
}
}

</script>

<style>

</style>