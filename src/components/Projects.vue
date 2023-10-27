<template>
    <section class="projects-section">
        <div class="mb-16 text-center">
            <h1>Projects</h1>
            <br>
            <hr class=" w-54 sm:w-72 border border-slate-700">
        </div>
        
        <div class="project-card" v-for="project in Projects" :key="project.title">
            <div class="bg-img" :style="{'background': 'url('+getImg(project.img)+') no-repeat center', 'background-size': 'cover'}"></div>
            <div class="card-body">
                <div class="card-desc">
                    <h3>{{ project.title }}</h3>
                    <br>
                    <p>{{ project.desc }}</p>
                </div>
                <div class="card-btn">
                    <a class="link-btn" :href="project.link">View Project</a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import { Projects } from "../data/projects.json";
export default {
    data(){
        return{
            Projects
        }
    },
    setup(){
        const getImg = (path) =>{
            return new URL(`../assets/img/${path}`, import.meta.url).href
        }

        return{getImg}
    }
}
</script>
<style>
.bg-img2 {
    display: block;
    height: 240px;
    width: 100%;

    @media screen and (min-width: 768px) {
        width: 33.3%;

    }
}
</style>
<style lang="postcss" scoped>
.projects-section {
    @apply flex flex-col w-full h-fit px-0 md:px-24 py-16 bg-gray-300 content-center align-middle items-center text-slate-800
}

.project-card {
    @apply flex flex-col my-5 md:flex-row w-3/4 md:w-full lg:w-3/4 h-[450px] md:h-full border shadow-lg hover:shadow-xl shadow-slate-400 transition-shadow hover:shadow-slate-400 bg-slate-200
}

.card-body {
    @apply py-5 px-4 sm:px-8 min-h-fit min-w-full md:min-w-min sm:w-96 md:w-2/3 flex flex-col justify-between
}
.bg-img{
    @apply block h-60 md:w-1/3 w-full 
}
.card-body .card-desc{
    @apply my-2
}
.card-body .card-btn{
    @apply mt-4 h-16 flex content-center items-center justify-center
}
.card-body .link-btn{
    @apply mx-auto w-11/12 sm:w-72 px-1 sm:px-3 py-3 border-2 text-center hover:text-slate-100 border-slate-700 bg-transparent hover:bg-slate-700
}
</style>