<template>
    <section class="hero-backdrop">
        <div class="hero-text">
            <h1 class="hidden sm:block">Muhammad Afif Al Ghifari</h1>
            <h1 class="sm:hidden block">Muhammad Afif <br> Al Ghifari</h1>
            <h2>Front End Developer</h2>
            <button class="resume-button">Download Resume</button>
        </div>
    </section>
</template>

<style lang="postcss" scoped>
.hero-backdrop{
    @apply flex items-center w-full h-screen bg-slate-700 text-white
}

.hero-text{
    @apply mx-auto text-center h-64 px-5
}
.hero-text h1{
    @apply my-4 text-4xl sm:text-5xl
}
.hero-text h2{
    @apply my-4 text-xl sm:text-3xl
}

.resume-button{
    @apply h-14 mx-auto my-10 sm:py-8 sm:px-6 py-6 px-4 flex items-center text-xl border-2 bg-transparent border-slate-200 
    text-slate-200 hover:text-slate-600 hover:bg-slate-200
}
</style>