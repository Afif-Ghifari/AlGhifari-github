<template>
    <button class="navbar-btn-sm" @click="toggleNavbar" v-if="showNavbarBtn"><i
            class="bi bi-list text-3xl font-bold"></i></button>

    <div class="navbar-backdrop" v-if="showNavbar"></div>
    <div class="dropdown" v-if="showNavbar">
        <ul>
            <div class="w-full mt-6">
                <div class="w-full text-right text-2xl"><button class="close-btn" @click="toggleNavbar"><i
                            class="bi bi-x-lg"></i></button></div>
            </div>
            <li><a href="#about">About</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#skill">Skills</a></li>
            <li><a>Contacts</a></li>
        </ul>
    </div>

    <div class="navbar-lg">

        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#skill">Skills</a></li>
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
.navbar-btn-sm {
    @apply fixed inline md:hidden top-11 right-8 h-14 w-14 bg-slate-100 hover:bg-slate-400 border shadow-md border-black z-20
}

.dropdown {
    @apply w-full fixed inline md:hidden h-[450px] bg-slate-200 py-5 z-20
}

.dropdown ul {
    @apply flex flex-col
}

.dropdown ul .close-btn{
    @apply mr-8 inline md:hidden h-14 w-14 border shadow-md border-black 
}

.dropdown ul li {
    @apply flex items-center w-full my-1 py-3 cursor-pointer hover:bg-white
}

.dropdown ul li a {
    @apply text-base text-center mx-auto
}

.navbar-backdrop {
    @apply bg-slate-900 w-screen h-screen fixed opacity-25 z-10 inline md:hidden
}


.navbar-lg {
    @apply hidden md:flex flex-row justify-evenly h-24 w-5/6 lg:w-2/3 py-7 px-10 left-1/2 right-1/2 transform 
    -translate-x-1/2 bg-slate-100 rounded-b-md shadow-lg fixed
}

.navbar-lg ul {
    @apply grid grid-cols-6 lg:mx-0 mx-auto w-full
}

.navbar-lg ul li {
    @apply flex items-center w-full cursor-pointer hover:bg-white
}

.navbar-lg ul li a {
    @apply text-base text-center mx-auto
}</style>