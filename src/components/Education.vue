<template>
    <section class="education-section">
        <div class="mb-6 text-center">
            <h1>Education</h1>
            <br>
            <hr class="border border-slate-700 w-54 sm:w-72">
        </div>

        <div class="education-exp" v-for="edu in Educations" :key="edu">
            <div class="education-timeline">
                <h3 class="text-center mx-auto">{{ edu.date }}</h3>
            </div>
            <div class="education-desc">
                <h3 class="text-center my-2 font-semibold">{{ edu.school }}</h3>
                <h4 class="my-2">{{ edu.department }}</h4>
                <p class="my-2">{{ edu.desc }}</p>
            </div>
        </div>
    </section>
</template>

<script>
import { Educations } from '../data/educations.json'
export default {
    data(){
        return{
            Educations
        }
    }
}
</script>

<style lang="postcss" scoped>
.education-section{
    @apply flex flex-col w-full h-fit px-0 md:px-10 lg:px-20 py-16 bg-slate-200 content-center align-middle items-center text-slate-800
}

.education-exp{
    @apply my-14 h-fit md:h-72 md:my-0 flex-col md:flex-row flex content-center align-middle items-center
}

.education-exp{
    @apply my-14 h-fit md:h-72 md:my-0 flex-col md:flex-row flex content-center align-middle items-center
}
.education-timeline{
    @apply w-2/3 md:w-1/3 h-fit my-2 pb-5 md:pb-0 flex content-center align-middle items-center text-center md:border-0 border-b-2 border-slate-700 
}
.education-desc{
    @apply w-3/4 md:w-2/3 h-full px-0 py-0 md:py-16 md:px-10 flex flex-col content-center align-middle border-0 md:border-l-2 border-slate-700
}
.education-desc h4{
    @apply indent-0 md:indent-10 text-center md:text-left
}
.education-desc p{
    @apply pl-0 md:pl-5 lg:pl-10 pr-0 md:pr-5 lg:pr-40
}
</style>