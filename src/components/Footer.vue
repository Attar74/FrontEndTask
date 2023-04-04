<template>
    <footer class="md:mt-20 mb-10 text-center text-neutral-600 dark:bg-neutral-600 dark:text-neutral-200 lg:text-left">
        <div class="block md:flex items-center py-6 justify-between">
            <div>
                <span class="cursor-pointer text-gray-800 text-3xl md:text-4xl">Let's Connect</span>
            </div>
            <div class="my-5 md:my-0 flex items-center justify-center">
                <img v-for="(item, i) in socialItems" :key="i" class="mx-4 cursor-pointer" :src="item.src" :alt="item.alt">
            </div>
            <div class="flex cursor-pointer justify-center items-center" @click="backToTop">
                <span class="text-gray-800 text-2xl">Back to Top</span>
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="ml-2 w-6 h-6 text-gray-800">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M12 19.5v-15m0 0l-6.75 6.75M12 4.5l6.75 6.75" />
                </svg>
            </div>
        </div>
    </footer>
</template>

<script setup>
    import { reactive } from "vue";

    const socialItems = reactive([
        {
            src: 'src/assets/svg-icons/Instagram.svg',
            alt: 'Instagram'
        },
        {
            src: 'src/assets/svg-icons/YouTube.svg',
            alt: 'YouTube'
        },
        {
            src: 'src/assets/svg-icons/Vector.svg',
            alt: 'Vector'
        }
    ])
    const backToTop = ()=> {
        window.scrollTo({top: 0, behavior: "smooth"});
    }
</script>

<style lang="scss" scoped>

</style>