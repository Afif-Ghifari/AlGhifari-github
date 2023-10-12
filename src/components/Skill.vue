<template>
    <section class="projects-section">
        <div class="mb-16 text-center">
            <h1>Skills</h1>
            <br>
            <hr class=" w-54 sm:w-72 border border-slate-700">
        </div>

        <div class="skill-row">
            <img src="../assets/img/skill-icons/icons8-html-logo.svg" class="skill-img" alt="">
            <img src="../assets/img/skill-icons/icons8-css-logo.svg" class="skill-img" alt="">
            <img src="../assets/img/skill-icons/icons8-javascript.svg" class="skill-img" alt="">
            <img src="../assets/img/skill-icons/icons8-vue-js.svg" class="skill-img" alt="">
            <img src="../assets/img/skill-icons/icons8-shopify.svg" class="skill-img" alt="">
        </div>
    </section>
</template>

<style lang="postcss" scoped>
.projects-section {
    @apply flex flex-col w-full h-fit px-0 md:px-24 py-16 bg-slate-200 content-center align-middle items-center text-slate-800
}

.skill-row{
    @apply grid grid-flow-row-dense grid-cols-2 md:grid-cols-3 w-1/2 h-fit
}
.skill-row .skill-img{
    @apply mx-auto
}
</style>