<template>
    <div class="review-card">
        <div class="image-container">
            <img :src="bobo.url" alt="">
            <!-- <p>{{head}}</p> -->
            
            
        </div>
       <h2>hello</h2>
    </div>
</template>

<script>
    export default {
        // props: ['head'],
        
        
    }
</script>

<style scoped>
    .review-card {
        margin-top: 1.5rem;
        display: flex;
        flex-wrap: wrap;
        
    }
    
    img {
        width: 10rem;
        height: 10rem;
    }
    
</style>