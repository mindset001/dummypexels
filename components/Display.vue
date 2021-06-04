<template>
    <div>
        <h3>Customer Reviews</h3>
        <!-- <img src="bobo.photographers" alt=""> -->
        <!-- <div v-if="headers.results" > -->
            
            <!-- <p>{{bobo}}</p> -->
            <div v-for = "(picture, pictureIndex) in gallery"
            :key= "pictureIndex">
            <img :src= "picture.url" alt="">
            <p>{{ picture.src }}</p>

            </div>
            
        </div>
        
        <!-- <h1>gfdsxcvbnmjhf</h1> -->
    <!-- </div> -->
</template>

<script>

    export default {
        
        
        
        data(){

            return {
                gallery: []

            }
        },
       
        async fetch (){
           this.gallery= await fetch ("https://api.pexels.com/v1/curated", {
                            headers: {
                            Authorization: '563492ad6f91700001000001068b977417d84c53b0267c7831566d11'
                            }})
                            .then(response => response.json())
                        
                            .then((result) => {
                                let bobo = [];
                                bobo = result.photos;
                                console.log(bobo)
                                this.gallery=bobo;
                                // return bobo;
                            } )
                            
                        // console.log(result.photos)
                        
                         .catch(err => console.log(err))
    }

        

    }
</script>

<style scoped>
</style>