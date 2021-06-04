<template>
    <nav class="sticky" >
        <div class="flex flex-wrap mr-5">
            <NuxtLink class="  flex ml-5 mt-2" to="/"><svg xmlns="http://www.w3.org/2000/svg" width="38px" height="38px" class="rounded-md"
                viewBox="0 0 32 32">
                <path d="M2 0h28a2 2 0 0 1 2 2v28a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2a2 2 0 0 1 2-2z" fill="#05A081"></path>
                <path d="M13 21h3.863v-3.752h1.167a3.124 3.124 0 1 0 0-6.248H13v10zm5.863 2H11V9h7.03a5.124 5.124 0 0 1 .833 10.18V23z" fill="#fff"></path>
                </svg> <h2 class="text-white ml-3 mt-3 text-sm">Pexels</h2>
            </NuxtLink>

                

    <div class="mt-50" >
        <ul class="flex text-white text-lg">
            <li class="">
                <NuxtLink to="/products" class=""><div class="dropdown">
                        <span class="navi-content">Explore</span>
                        <div class="dropdown-content text-base font-medium leading-9 w-40 rounded">
                        <p class="text-gray-500 hone w-30"> <nuxt-link to="">Discover Photos</nuxt-link> </p>
                        <p class="text-gray-500 hone w-30"> <nuxt-link to="">Popular Searches</nuxt-link> </p>
                        <p class="text-gray-500 hone w-30"> <nuxt-link to="">Leaderboard</nuxt-link> </p>
                        <p class="text-gray-500 hone w-30"> <nuxt-link to="">Challenges</nuxt-link> </p>
                        <p class="text-gray-500 hone w-30"> <nuxt-link to="">Free Videos</nuxt-link> </p>
                        <p class="text-gray-500 hone w-30"> <nuxt-link to="">Pixels Blog</nuxt-link> </p>
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
                        <span class="icon text-white circle"><font-awesome-icon :icon="['fas', 'circle']"/></span>
                        <span class="icon text-white circle"><font-awesome-icon :icon="['fas', 'circle']"/></span>
                        <span class="icon text-white circle"><font-awesome-icon :icon="['fas', 'circle']"/></span>
                        <div class="dropdown-content dropdown-content-2 text-base font-medium leading-9 w-80 rounded">
                        <p class="text-gray-500 hone w-70 "> <nuxt-link to="">Login</nuxt-link> </p>
                        <p class="text-gray-500 hone w-70"> <nuxt-link to="">Join</nuxt-link> </p>
                        <p class="text-gray-500 hone w-70"> <nuxt-link to="">Change Language</nuxt-link> </p>
                        <p class="text-gray-500 hone w-70"> <nuxt-link to="">images & Videos Api</nuxt-link> </p>
                        <p class="text-gray-500 hone w-70"> <nuxt-link to="">Apps & Plugins</nuxt-link> </p>
                        <p class="text-gray-500 hone w-70"> <nuxt-link to="">FAQ</nuxt-link> </p>
                        <p class="text-gray-500 hone w-70"> <nuxt-link to="">Partnerships</nuxt-link> </p>
                        <p class="text-gray-500 hone w-70"> <nuxt-link to="">Imprint & Terms  </nuxt-link> </p>
                        <div>
                           <span class="icon text-black mr-10"><font-awesome-icon :icon="['fab', 'facebook-f']"/></span>
                           <span class="icon text-black mr-10"><font-awesome-icon :icon="['fab', 'twitter']"/></span>
                           <span class="icon text-black mr-10"><font-awesome-icon :icon="['fab', 'instagram']"/></span>
                           <span class="icon text-black mr-10"><font-awesome-icon :icon="['fab', 'pinterest']"/></span>
                           <span class="icon text-black"><font-awesome-icon :icon="['fab', 'youtube']"/></span>
                        </div>
                        </div>
                        </div> <span class="sr-only">(current)</span></NuxtLink>
            </li>
            <li><button class="bg-green h-6 w-10" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
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
        background:transparent;
        position: absolute;
        width: 100%;
        top: 0;
    
    }
    .circle{
        font-size: 4px;
        margin-left: -2px;
    }
    ul{
        position: absolute;
        right:20px;
        top: 10%;
        /* left: ; */
        
    }
    li{
        padding-left: 20px;
    }

    .hone:hover{
        background-color: #d1d5db ;
        /* margin-left: -18px; */
    }
    button{
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

 
.dropdown-content::before{
      content: '';
    position: absolute;
    display: block;
    width: 15px;
    height: 15px;
    top: -13px;
    right: 22px;
    clip-path: polygon(100% 100%, 54% 43%, 0 100%);
    background: white;
}
.dropdown-content-2::before{
      content: '';
    position: absolute;
    display: block;
    width: 15px;
    height: 15px;
    top: -13px;
    right: 2px;
    clip-path: polygon(100% 100%, 54% 43%, 0 100%);
    background: white;
}

.dropdown-content, .dropdown-content-2 {
  display: none;
  position: absolute;
  right: 0;
  top: 33px;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  padding: 12px 16px;
  z-index: 1;
}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>