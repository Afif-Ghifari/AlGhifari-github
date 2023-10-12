<template>
    <section class="contact-section">
        <div class="mb-16 text-center">
            <h1>Contact Me</h1>
            <br>
            <hr class=" w-54 sm:w-72 border border-slate-700">
        </div>

        <form action="" class="form-container">
            <input type="text" placeholder="Your email" class="input-field">
            <textarea class="input-field" name="" id="" cols="30" rows="10" placeholder="Your message"></textarea>
            <button type="submit" class="send-button">Send</button>
        </form>
    </section>
</template>

<style lang="postcss" scoped>
.contact-section {
    @apply flex flex-col w-full h-fit px-0 md:px-24 py-16 bg-gray-300 content-center align-middle items-center text-slate-800
}

.form-container{
    @apply flex flex-col w-5/6 sm:w-3/4 md:w-1/2 align-middle
}
.form-container .input-field{
    @apply w-full px-4 py-2 my-2 border border-slate-700 bg-slate-100
}

.form-container .send-button{
    @apply w-full py-2 px-4 my-2 bg-slate-100 hover:bg-slate-700 border border-slate-700 hover:text-slate-50
}
</style>