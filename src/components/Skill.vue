<template>
    <section class="skill-section">
        <div class="mb-16 text-center">
            <h1>Skills</h1>
            <br>
            <hr class="w-54 sm:w-72 border border-slate-700">
        </div>

        <div class="skill-row">
            <div class="mx-4"><img src="../assets/img/skill-icons/icons8-html-logo.svg" class="skill-img" alt="HTML 5"><h4>HTML 5</h4></div>
            <div class="mx-4"><img src="../assets/img/skill-icons/icons8-css-logo.svg" class="skill-img" alt="CSS"><h4>CSS</h4></div>
            <div class="mx-4"><img src="../assets/img/skill-icons/icons8-javascript.svg" class="skill-img" alt="JavaScript"><h4>JavaScript</h4></div>
            <div class="mx-4"><img src="../assets/img/skill-icons/icons8-vue-js.svg" class="skill-img" alt="Vue JS"><h4>Vue JS</h4></div>
            <div class="mx-4"><img src="../assets/img/skill-icons/icons8-shopify.svg" class="skill-img" alt="Shopify"><h4>Shopify Liquid</h4></div>
        </div>
    </section>
</template>

<style lang="postcss" scoped>
.skill-section {
    @apply flex flex-col w-full h-fit px-0 md:px-24 py-16 bg-slate-200 content-center align-middle items-center text-slate-800
}

.skill-row{
    @apply grid grid-cols-2 md:grid-cols-3 justify-between w-1/2 h-fit text-center
}
.skill-row .skill-img{
    @apply mx-auto w-14 
}
</style>