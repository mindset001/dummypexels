<template>
    <div class="hero2">
        <div >
             <Nav 
             v-on:scroll = "handleScroll"
             />
             <!-- <NewNav/> -->
              </div>
        <div class="container2 ">
            <div>
                <h1 class="text-4xl text-white font-bold">The best free stock photos & videos <br> shared by talented creators.</h1>

                <div class=" flex items-center justify-center">
                    <div class=" overflow-hidden flex flex-wrap">
                    <form action="" class="p-2 my-2 justify-between border-0 text-base bg-white rounded-md">
                            <input autocapitalize="none" 
                            autocomplete="off" 
                            autofocus="" 
                            id="search" 
                            name="s" 
                            placeholder="Search for free photos and videos" 
                            required="required" type="search" value="">
                            
                    <button class="justify-center ">
                        <svg class="h-5 w-5 text-black" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M16.32 14.9l5.39 5.4a1 1 0 0 1-1.42 1.4l-5.38-5.38a8 8 0 1 1 1.41-1.41zM10 16a6 6 0 1 0 0-12 6 6 0 0 0 0 12z"/></svg>
                    </button>
                </form>
                </div>
                </div>

            <div class="text-white">
                <ul class="text-smd font-thin">
                    <span class="font-bold ">Suggested: </span>
                    <li class="opacity-70 "> fish,</li>
                    <li class="opacity-70">cute baby,</li>
                    <li class="opacity-70">india,</li>
                    <li class="opacity-70">youtube,</li>
                    <li class="opacity-70">blur,</li>
                    <li class="opacity-70">nature,</li>
                    <li class="opacity-70">more</li>
                </ul>
            </div>
            <div>
                <nuxt-link  class="text-white opacity-50 alan text-sm" data-photo-modal="1142069" to="/photo/green-banana-leaf-1142069/" data-photo-modal-initialized="true">Photo by Alan Cabello</nuxt-link>
            </div>
            </div>
            
            
        </div>
        <div class="nav">
                <ul class="text-lg font-semibold tracking-wide">
                    <nuxt-link to="/"><li class="list">Home</li></nuxt-link>
                    <nuxt-link to="https://www.pexels.com/discover/"><li>Discover</li></nuxt-link>
                    <nuxt-link to="https://www.pexels.com/videos/"><li>Videos</li></nuxt-link>
                    <nuxt-link to="https://www.pexels.com/leaderboard/"><li>Leaderboard</li></nuxt-link>
                    <nuxt-link to="https://www.pexels.com/challenges/"><li>Challenges</li></nuxt-link>
                </ul>
                </div>
                
                <section class="mx-10 mt-5">
                    <div class=" split">
                    <div class="stock"> <h3>Free Stock Photos</h3> </div>
                    <div class="dropdown">
  <div class="dropbtn text-sm "> <div class="flex">
      <h1 >Trending</h1> 
      <div><span class="icon text-black circle ml-2"><font-awesome-icon :icon="['fas', 'caret-down']"/></span></div>
  </div>
  <div class="dropdown-content dropdown-content-3  text-black ">
  <a href="#" class="hone w-40">Trending</a><br>
  <a href="#" class="hone w-40">New</a>
  
  </div>
  </div>
</div>


                    </div>
                </section>
                
                <Display />
                <StockCard/>
            
    </div>
</template>

<script>
    export default {
        data() {
      return {
        // Initialize scroll position at [0, 0]
        // [handleScroll]: [0, 0]
      }
    },
  mounted () {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll (event) {
        console.log('scrolling');
      // Any code to be executed when the window is scrolled
      this.isUserScrolling = (window.scrollY > 0);

      
    }
  }
}
    
</script>

<style scoped>

    .hero2{
        min-height: 100vh;
        min-width: 100vw;
        height: 100vh;
        width: 100vw;
        /* overflow: hidden; */
    }
    .container2{
        background-image: url('../assets/pexels-photo-1142069 (1).jpeg');
        background-size: cover;
        background-repeat: no-repeat;
        width: 100%;
        height: 55vh;
        /* justify-content: center; */
        display: grid;
        place-items: center;
    }
    .hone:hover{
        background-color: #d1d5db ;
        /* margin-left: -18px; */
    }
    
    form{
        /* width: 43em; */
        font-size: 14px;
        margin-top: 10px;
        height: 40px;
    }

    input{
        
        
        padding-left: 1rem;
        width: 43em;
        outline: none;
    }
    
    input:hover{
        text-decoration: none;
    }
    ul{
        margin-top: 10px;
        display: flex;
    }
    li{
        margin-left: 5px;
    }
    .alan{
        position: absolute;
        top: 53%;
        right: 0;
    }
    .nav{
        display: grid;
        place-items: center;
        margin-top: 20px;
        /* padding-bottom: 20px ; */
        border-bottom: 1.5px solid rgba(22, 22, 22, 0.1) ;
    }
    .nav li{
        padding-left: 20px;
    }
    .nav li:hover{
        color: blue;
    }
    .list{
        border-bottom: 3px solid #0064f9;
        color: #0064f9;
        padding-bottom: 15px;
        width: 5em;
        display: grid;
        place-items: left;

    }

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content, 
.dropdown-content-3 {
  display: none;
  position: absolute;
  right: 0;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  padding: 12px 16px;
  z-index: 1;
}
 
.dropdown-content-3::before{
      content: '';
    position: absolute;
    display: block;
    width: 15px;
    height: 15px;
    top: -13px;
    right: 22px;
    clip-path: polygon(100% 100%, 54% 43%, 0 100%);
    background: rgb(36, 39, 224);
}

.dropdown:hover .dropdown-content {
  display: block;
}

section{
    display: flex;
    flex-direction: row;
}
select{
    outline: none;
    
}
option{
    outline: none;
}
.split{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
}
.new{
    width: fit-content;
    position: relative;
    /* transform: translateX(1800%); */
}
.stock{
    width: 10rem;
    position: relative;
}
</style>