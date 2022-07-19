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

    <h5 class="text-center textclr"><span class="elcolor">☚</span>Jesse Spence<span class="elcolor">☛</span></h5>
    <p class="text-center elcolor">copyright Design by</p> <p class="text-center elcolor">© Jesse at Lifechoices</p>
        
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
router-link{
  position: absolute;
}
.navhead{
border-bottom: 5px var(--el-color) solid;
border-left: 5px var(--el-color) solid;
padding-left:10px;
}

.navbar{
    width:250px;
    height: 100vh;
    position:fixed;
    background-color: var(--text-mute) !important;
    transition: 0.5s;
    text-shadow: 1px 2px 3px var(--el-color);
}
#sidebar ul li a{
  color: var(--text-color) ;
    transition:0.5s;
    font-weight: 500;
}

#sidebar ul li a:hover{
    margin-left: 3%;
    color: var(--highlight-color)!important;

} 
#sidebar ul li a:focus{
    margin-left: 3%;
    color: var(--highlight-color)!important;
}

#sidebar li a:active{
    margin-left: 3%;
    color: var(--highlight-color)!important;
}

</style>
