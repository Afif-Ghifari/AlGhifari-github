<template>
        <section class="about-section">
            <div class="about-me">
                <h2 class="mx-auto">About Me</h2>
            </div>
            <div class="about-me-desc">
                <p>
                    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rerum quaerat cum enim doloribus 
                    exercitationem nihil inventore sapiente nostrum voluptatum perspiciatis a eaque dolorem 
                    quis minima omnis laborum unde odit nemo soluta molestiae, quae harum vero. Dolores sed 
                    dicta fugiat.
                </p>
            </div>
        </section>
</template>

<style lang="postcss" scoped>
    .about-section{
        @apply flex flex-col md:flex-row w-full h-fit px-2 md:px-24 py-16 bg-slate-200 content-center align-middle items-center text-slate-800
    }
    .about-me{
        @apply w-2/3 md:w-1/3 h-fit my-2 pb-5 md:pb-0 flex content-center align-middle items-center text-center md:border-0 border-b-2 border-slate-700 
    }
    .about-me-desc{
        @apply w-2/3 h-fit my-2 flex content-center align-middle items-center border-0 md:border-l-2 border-slate-700
    }
    .about-me-desc p{
        @apply pl-1 md:pl-10 lg:pl-10 pr-2 md:pr-20 lg:pr-40 text-justify mx-auto
    }
</style>