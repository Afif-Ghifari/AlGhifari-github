<template>
    <section class="experience-section">
        <div class="work-exp">
            <div class="work-timeline">
                <h3 class="text-center mx-auto">July 2022 - December 2022</h3>
            </div>
            <div class="work-desc">
                <h3 class="text-center my-2">PT. Lorem Ipsum Dolor</h3>
                <h4 class="my-2">Intern Front End Developer</h4>
                <p class="my-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat iusto saepe, officiis necessitatibus
                    aspernatur placeat.</p>
            </div>
        </div>
        <div class="work-exp">
            <div class="work-timeline">
                <h3 class="text-center mx-auto">July 2022 - December 2022</h3>
            </div>
            <div class="work-desc">
                <h3 class="text-center my-2">PT. Lorem Ipsum Dolor</h3>
                <h4 class="my-2">Intern Front End Developer</h4>
                <p class="my-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat iusto saepe, officiis necessitatibus
                    aspernatur placeat.</p>
            </div>
        </div>
        <!-- <div>
            <div></div>
            <div></div>
        </div> -->
    </section>
</template>

<style lang="postcss" scoped>
.experience-section{
    @apply flex flex-col w-screen h-fit px-2 md:px-24 py-16 bg-gray-300 content-center align-middle items-center text-slate-800 
}
.work-exp{
    @apply my-7 h-72 md:my-0 flex-col md:flex-row flex content-center align-middle items-center
}
.work-timeline{
    @apply w-2/3 md:w-1/3 h-fit my-2 pb-5 md:pb-0 flex content-center align-middle items-center text-center md:border-0 border-b-2 border-slate-700 
}
.work-desc{
    @apply w-3/4 md:w-2/3 h-full px-2 py-0 md:py-16 md:px-10 flex flex-col content-center align-middle border-0 md:border-l-2 border-slate-700
}
.work-desc h4{
    @apply indent-10
}
.work-desc p{
    @apply pl-1 md:pl-5 lg:pl-10 pr-1 md:pr-5 lg:pr-40
}
</style>