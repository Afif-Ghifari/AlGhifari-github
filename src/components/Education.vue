<template>
    <section class="education-section">
        <div class="mb-6 text-center">
            <h1>Education</h1>
            <br>
            <hr class="border border-slate-700 w-54 sm:w-72">
        </div>

        <div class="education-exp">
            <div class="work-timeline">
                <h3 class="text-center mx-auto">July 2020 - March 2023</h3>
            </div>
            <div class="work-desc">
                <h3 class="text-center my-2 font-semibold">Malang Telkom Vocational High School</h3>
                <h4 class="my-2">Software Development</h4>
                <p class="my-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat iusto saepe, officiis necessitatibus
                    aspernatur placeat.</p>
            </div>
        </div>
    </section>
</template>

<style lang="postcss" scoped>
.education-section{
    @apply flex flex-col w-full h-fit px-0 md:px-10 lg:px-20 py-16 bg-slate-200 content-center align-middle items-center text-slate-800
}

.education-exp{
    @apply my-14 h-fit md:h-72 md:my-0 flex-col md:flex-row flex content-center align-middle items-center
}

.work-exp{
    @apply my-14 h-fit md:h-72 md:my-0 flex-col md:flex-row flex content-center align-middle items-center
}
.work-timeline{
    @apply w-2/3 md:w-1/3 h-fit my-2 pb-5 md:pb-0 flex content-center align-middle items-center text-center md:border-0 border-b-2 border-slate-700 
}
.work-desc{
    @apply w-3/4 md:w-2/3 h-full px-0 py-0 md:py-16 md:px-10 flex flex-col content-center align-middle border-0 md:border-l-2 border-slate-700
}
.work-desc h4{
    @apply indent-0 md:indent-10 text-center md:text-left
}
.work-desc p{
    @apply pl-0 md:pl-5 lg:pl-10 pr-0 md:pr-5 lg:pr-40
}
</style>