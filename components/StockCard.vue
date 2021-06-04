<template>
    <div>
        
        <div class="nav">
            <div>
                <ul>
                    <nuxt-link to="/"><li>Home</li></nuxt-link>
                    <nuxt-link to="https://www.pexels.com/discover/"><li>Discover</li></nuxt-link>
                    <nuxt-link to="https://www.pexels.com/videos/"><li>Videos</li></nuxt-link>
                    <nuxt-link to="https://www.pexels.com/leaderboard/"><li>Leaderboard</li></nuxt-link>
                    <nuxt-link to="https://www.pexels.com/challenges/"><li>challenges</li></nuxt-link>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    
    .nav{
        display: grid;
        place-items: center;
    }
    ul{
        display: flex;

    }
    li{
        padding-left: 10px;
    }

</style>