<template>
    <section class="projects-section">
        <div class="mb-6 text-center">
            <h1>Projects</h1>
            <br>
            <hr class=" w-54 sm:w-72 border border-slate-700">
        </div>
        <div class="project-card">
            <div class="card-img"><img src="../assets/img/project-vue-recipe.png" class="img" alt=""></div>
            <!-- <div class="card-img" style="background-image: url('../assets/img/project-vue-recipe.png');"></div> -->
            <div class="card-body">
                <h3>Lorem, ipsum.</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae, nesciunt.</p>
            </div>
        </div>
    </section>
</template>

<style lang="postcss" scoped>
.projects-section{
    @apply flex flex-col w-full h-fit px-0 md:px-24 py-16 bg-gray-300 content-center align-middle items-center text-slate-800 
}
.project-card{
    @apply flex flex-col md:flex-row w-3/4 border shadow-lg hover:shadow-xl bg-slate-200
}
.card-img{
    @apply block h-60 w-1/3 bg-no-repeat bg-cover bg-center
}
.card-img .img{
    @apply w-full max-h-60 object-cover object-center
}
.card-body{
    @apply py-5 px-8 w-2/3
}

</style>