<template>
    <nav class="sticky" >
        <div class="flex flex-wrap">
            <NuxtLink class="  flex ml-5 mt-2" to="/"><svg xmlns="http://www.w3.org/2000/svg" width="32px" height="32px" class="rounded-md"
                viewBox="0 0 32 32">
                <path d="M2 0h28a2 2 0 0 1 2 2v28a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2a2 2 0 0 1 2-2z" fill="#05A081"></path>
                <path d="M13 21h3.863v-3.752h1.167a3.124 3.124 0 1 0 0-6.248H13v10zm5.863 2H11V9h7.03a5.124 5.124 0 0 1 .833 10.18V23z" fill="#fff"></path>
                </svg> <h2 class="text-white ml-3 mt-1 text-sm">Pexels</h2>
            </NuxtLink>

        <div class=" flex items-center justify-center">
                    <div class=" overflow-hidden flex flex-wrap">
                    <form action="" class="p-2 my-2 justify-between border-0 text-base bg-white rounded-md">
                            <input autocapitalize="none" 
                            autocomplete="off" 
                            autofocus="" 
                            id="search" 
                            name="s" 
                            placeholder="Search for free photos" 
                            required="required" type="search" value="">
                            
                    <button class="justify-center ">
                        <svg class="h-5 w-5 text-black" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M16.32 14.9l5.39 5.4a1 1 0 0 1-1.42 1.4l-5.38-5.38a8 8 0 1 1 1.41-1.41zM10 16a6 6 0 1 0 0-12 6 6 0 0 0 0 12z"/></svg>
                    </button>
                </form>
                </div>
                </div>
                

    <div class="" >
        <ul class="flex text-white text-lg">
            <li class="">
                <NuxtLink to="/products" class=""><div class="dropdown">
                        <span>Explore</span>
                        <div class="dropdown-content">
                        <p class="text-gray-500"> <nuxt-link to="">Discover Photos</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Popular Searches</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Leaderboard</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Challenges</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Free Videos</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Pixels Blog</nuxt-link> </p>
                        </div>
                        </div> <span class="sr-only">(current)</span></NuxtLink>
            </li>
            <li class="">
                <NuxtLink to="/my-items" class="">License <span class="sr-only">(current)</span></NuxtLink>
            </li>
            <li class="nav-item active">
                <NuxtLink to="/my-items" class="">Upload <span class="sr-only">(current)</span></NuxtLink>
            </li>
            <li class="">
                <NuxtLink to="/products" class=""><div class="dropdown">
                        <span>...</span>
                        <div class="dropdown-content">
                        <p class="text-gray-500"> <nuxt-link to="">Login</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Join</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Change Language</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">images & Videos Api</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Apps & Plugins</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">FAQ</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Partnerships</nuxt-link> </p>
                        <p class="text-gray-500"> <nuxt-link to="">Imprint & Terms  </nuxt-link> </p>
                        </div>
                        </div> <span class="sr-only">(current)</span></NuxtLink>
            </li>
            <li><button class="bg-green h-6 w-10 btn2" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon">Join</span>
    </button></li>
        </ul>
    </div>
        </div>
    </nav>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>


    nav{
        background-color: #333;
        position: sticky;
        top: 0;
    
    }
    ul{
        position: absolute;
        right:0;
        top: 4%;
        
    }
    li{
        padding-left: 20px;
    }

    .btn2{
        background-color: #05a081;
        height: 40px;
        width: 100px;
        padding-top: 5px;
        padding-bottom: 5px;
        border-radius: 4px;
        
    }
   
   .dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  right: 0;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  padding: 12px 16px;
  z-index: 1;
}

.dropdown:hover .dropdown-content {
  display: block;
}

 form{
        /* width: 33em; */
        margin-top: 10px;
        /* padding-top: 1rem; */
        /* padding-bottom: 1rem; */
        height: 40px;
        margin-left: 20px;
    }

    input{
        
        
        padding-left: 1rem;
        width: 43em;
        outline: none;
    }
    
    input:hover{
        text-decoration: none;
    }
</style>