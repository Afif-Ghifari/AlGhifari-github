<template>
    <section class="projects-section">
        <div class="mb-16 text-center">
            <h1>Projects</h1>
            <br>
            <hr class=" w-54 sm:w-72 border border-slate-700">
        </div>
        
        <div class="project-card">
            <div class="bg-img"></div>
            <div class="card-body">
                <div class="card-desc">
                    <h3>Lorem, ipsum.</h3>
                    <br>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae, nesciunt.</p>
                </div>
                <div class="card-btn">
                    <a class="link-btn" href="">View Project</a>
                </div>
            </div>
        </div>

        <div class="project-card">
            <div class="bg-img"></div>
            <div class="card-body">
                <div class="card-desc">
                    <h3>Lorem, ipsum.</h3>
                    <br>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae, nesciunt.</p>
                </div>
                <div class="card-btn">
                    <a class="link-btn" href="">View Project</a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
</script>

<style>
.bg-img {
    background: url('../assets/img/project-vue-recipe.png') no-repeat center;
    background-size: cover;
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