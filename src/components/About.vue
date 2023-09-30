<template>
        <section class="about-section">
            <div class="about-me">
                <h1 class="mx-auto">About Me</h1>
                <br>
                <hr class="border border-slate-700 w-54 sm:w-72">
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
        @apply flex flex-col w-full h-fit px-0 md:px-24 py-16 bg-slate-200 content-center align-middle items-center text-slate-800
    }
    .about-me{
        @apply text-center my-10
    }
    .about-me-desc{
        @apply max-w-md md:max-w-2xl h-fit mx-5 my-2 flex content-center align-middle items-center 
    }
    .about-me-desc p{
        @apply text-justify px-7 md:px-0 mx-auto
    }
</style>