<template>

    <button class="navbar-btn-sm" @click="toggleNavbar" v-if="showNavbarBtn"></button>

    <div class="navbar-backdrop" v-if="showNavbar"></div>
    <div class="dropbar" v-if="showNavbar">
        <ul>
            <div class="w-full mt-6"><div class="w-full text-right text-2xl"><button class="mr-[54px]" @click="toggleNavbar">X</button></div></div>
            <li><a>About</a></li>
            <li><a>Experience</a></li>
            <li><a>Education</a></li>
            <li><a>Projects</a></li>
            <li><a>Skills</a></li>
            <li><a>Contacts</a></li>
        </ul>
    </div>
    
    <div class="navbar-lg">
        
        <div class="w-1/12 hidden lg:inline">LOGO</div>
        
        <ul>
            <li><a>About</a></li>
            <li><a>Experience</a></li>
            <li><a>Education</a></li>
            <li><a>Projects</a></li>
            <li><a>Skills</a></li>
            <li><a>Contacts</a></li>
        </ul>
    
    </div>

</template>

<script setup>
import { ref } from 'vue';

const showNavbar = ref(false)
const showNavbarBtn = ref(true)

const toggleNavbar = () => {
    showNavbarBtn.value = !showNavbarBtn.value
    showNavbar.value = !showNavbar.value
}
</script>

<style lang="postcss" scoped>
.navbar-btn-sm{
    @apply fixed inline md:hidden top-8 right-8 h-14 w-14 bg-slate-200 hover:bg-slate-400 border shadow-md border-black rounded-full z-20
}
.dropbar{
    @apply w-full fixed inline md:hidden h-[450px] bg-slate-200 py-5 z-20
}
.dropbar ul{
    @apply flex flex-col 
}
.dropbar ul li{
    @apply flex items-center w-full my-1 py-3 cursor-pointer hover:bg-white
}
.dropbar ul li a{
    @apply text-base text-center
}
.navbar-backdrop{
    @apply bg-slate-900 w-screen h-screen fixed opacity-25 z-10 inline md:hidden
}


.navbar-lg{
    @apply hidden md:flex flex-row justify-between h-24 w-full py-7 px-10 bg-slate-200 border 
    border-black mx-auto shadow-lg fixed
}
.navbar-lg ul{
    @apply grid grid-cols-6 lg:mx-0 mx-auto md:w-9/12 lg:w-1/2
}
.navbar-lg ul li{
    @apply flex items-center w-full cursor-pointer hover:bg-white
}
.navbar-lg ul li a{
    @apply text-base text-center mx-auto 
}
</style>