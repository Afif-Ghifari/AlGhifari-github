<template>
    <section class="footer-section">
        <div class="footer-container">
            <div class="disclaimer">
                <h2 class="mb-3 font-bold">Thank You!</h2>
                <h4>Thank you for visiting my website, this website is still not perfect, sorry for the inconvenience while experiencing this website.</h4>
            </div>
            <div class="use-links">
                <h4>This site was made by:</h4>
                <ul>
                    <li>
                        <p>Vue JS</p>
                    </li>
                    <li>
                        <p>Vite JS</p>
                    </li>
                    <li>
                        <p>Tailwind CSS</p>
                    </li>
                </ul>
            </div>
        </div>
            <h5 class="footer-copyright">© Copyright 2023, All Rights Reserved by Afif Al Ghifari</h5>
    </section>
</template>

<style lang="postcss" scoped>
.footer-section{
    @apply flex flex-col w-full h-fit px-0 md:px-10 lg:px-20 py-16 bg-slate-200 content-center align-middle items-center text-slate-800
}

.footer-copyright{
    @apply my-5 mx-3 md:mx-0 text-center
}

.footer-container{
    @apply flex flex-col md:flex-row justify-between w-11/12 px-5 py-4 border-b border-slate-800
}
.footer-container .disclaimer{
    @apply w-full md:w-3/5 lg:w-2/5 my-3
}
.footer-container .use-links{
    @apply w-full md:w-2/5 lg:w-1/5 my-3
}
.footer-container ul{
    @apply my-5
}
.footer-container ul li{
    @apply my-2
}
</style>