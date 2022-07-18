<template>
	<nav class="navbar navbar-expand d-flex flex-column" id="sidebar">
<a href="#" class="navbar-brand text-light mt-5">
    <div class="display-5 text-center textclr navhead fw-bold"><h1>JESSE</h1></div>
</a>
<ul class="mb-5 navbar-nav d-flex flex-column mt-5 w-100">
    <li class="nav-item py-1 w-100">
        <a href="#home"  class="nav-link fw-bold textclr pl-4">
          <i class="pe-2 fa-solid fa-house"></i>
          <router-link class="nav-link active" to="/">HOME</router-link>
          </a>
    </li>
    <li class="nav-item py-1 w-100">
        <a class="nav-link fw-bold textclr pl-4"><i class="pe-2 fa-solid fa-user"></i>
        <router-link class="nav-link active" to="/About">ABOUT</router-link>
        </a>
    </li>
    <li class="nav-item py-1 w-100">
        <a class="nav-link fw-bold textclr pl-4"><i class="pe-2 fa-solid fa-hammer"></i>
        <router-link class="nav-link active" to='/ProjectsView'>PROJECTS</router-link>
        </a>
    </li>
    
    <li class="nav-item py-1 w-100">
        <a href="#testimonials" class="nav-link fw-bold textclr pl-4"><i class="pe-2 fa-solid fa-comments"></i>
        <router-link class="nav-link active" to='/Testimonials'>TESTIMONIALS</router-link>
        </a>
    </li>
    
    <li class="nav-item py-1 w-100">
        <a href="#contact" class="nav-link fw-bold textclr pl-4"><i class="pe-2 fa-solid fa-paper-plane"></i>
        <router-link class="nav-link active" to='/Contact'>CONTACT</router-link>
        </a>
    </li>
</ul>

    <h5 class="mt-5 text-center textclr"><span class="text-muted">☚</span>Jesse Spence<span class="text-muted">☛</span></h5>
    <p class="text-center text-muted">copyright Design by</p> <p class="text-center text-muted">© Joshua Davids</p>
        
</nav>
    <button class="btn my-4" id="menu-btn">Toggle Sidebar</button>
</template>

<script>
	export default {
		components: {},

    methods: {

      
    },
    computed:{

    }
	};
</script>

<style>
.navhead{
border-bottom: 5px var(--el-color) solid;
border-left: 5px var(--el-color) solid;
padding-left:10px;
}
body::-webkit-scrollbar {
  width: 12px;               /* width of the entire scrollbar */
}
body::-webkit-scrollbar-track {
  background: -webkit-linear-gradient(rgb(5, 202, 156), rgb(184, 14, 184));       /* color of the tracking area */
}
ul::-webkit-scrollbar-track {
  background: -webkit-linear-gradient(rgb(5, 202, 156), rgb(184, 14, 184));       /* color of the tracking area */
}
body::-webkit-scrollbar-thumb {
  background-color: rgb(0, 0, 0);    /* color of the scroll thumb */
  border-radius: 20px;       /* roundness of the scroll thumb */
  border: 2px solid rgb(255, 255, 255);  /* creates padding around scroll thumb */
}
.navbar{
    width:250px;
    height: 100vh;
    position:fixed;
    background-color: var(--text-mute);
    transition: 0.5s;
}
#sidebar ul li a{
  color: var(--text-color) ;
    transition:0.5s;
    font-weight: 500;
}

/* #sidebar ul li a:hover{
    margin-left: 3%;
    color: var(--highlight-color)!important;

} */
/* #sidebar ul li a:focus{
    margin-left: 3%;
    color: var(--highlight-color)!important;
} */

/* #sidebar li a:active{
    margin-left: 3%;
    color: var(--highlight-color)!important;
} */



.my-container{
    overflow: hidden;
    margin-left: 250px;
    
}

#menu-btn{
    display: none;
}

@media (max-width: 1199px){
    .navbar{
        width:250px;
        height: 100vh;
        position:fixed;
        margin-left: -300px;
        background-color: var(--nav-color);
        transition: 0.5s;
    }
    .my-container{
        margin: 0%;
        transition: 0.4s;
    }
    
    .active-nav{
        margin-left: 0%;
    }
    
    .active-cont{
        margin-left: 250px;
    }
    #menu-btn{
        display:inline;
        position: fixed;
        background-color: lightgray;
    }
    #menu-btn:focus{
        box-shadow: 0 0 0 0.25rem gray;
    }
}
	
</style>
