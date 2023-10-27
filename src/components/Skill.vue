<template>
    <section class="skill-section">
        <div class="mb-16 text-center">
            <h1>Skills</h1>
            <br>
            <hr class="w-54 sm:w-72 border border-slate-700">
        </div>

        <div class="skill-row">
            <div class="mx-4" v-for="skill in Skills" :key="skill.name">
                <img :src="getImg(skill.img)" class="skill-img" :alt="skill.alt"><h4>{{skill.name}}</h4>
            </div>
            
        </div>
    </section>
</template>

<script>
import {Skills} from '../data/skills.json'
export default {
    data(){
        return{
            Skills  
        }
    },
    setup(){
        const getImg = (path) => {
            return new URL(`../assets/img/skill-icons/${path}`, import.meta.url).href
        }

        return {getImg}
    }
}

</script>


<style lang="postcss" scoped>
.skill-section {
    @apply flex flex-col w-full h-fit px-0 md:px-24 py-16 bg-slate-200 content-center align-middle items-center text-slate-800
}

.skill-row{
    @apply flex flex-row flex-[0_0_calc(20%-40px)] flex-wrap justify-center max-w-sm gap-8 h-fit text-center
}
.skill-row .skill-img{
    @apply mx-auto w-14 
}
</style>