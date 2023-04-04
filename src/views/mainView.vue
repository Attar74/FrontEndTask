<template>
    <div class="flex flex-col mt-3 md:mt-0">
        <span class="text-4xl md:text-5xl font-medium md:text-left text-center">
            Our Projects
        </span>
        <div class="md:mt-8 text-sm font-medium text-center">
            <ul class="md:flex md:flex-wrap -mb-px">
                <li class="text-3xl m-5 md:mr-13 lg:mr-16">
                    <a href="#" class="inline-block text-amber-400 border-b-4 border-amber-400 rounded-t-lg active dark:amber-300 dark:border-amber-300" >Web Design</a>
                </li>
                <li class="text-3xl m-5 md:mr-13 lg:mr-16">
                    <a href="#" class="text-gray-500 inline-block border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300" aria-current="page">Mobile App Design</a>
                </li>
                <li class="text-3xl m-5 md:mr-13 lg:mr-16">
                    <a href="#" class="text-gray-500 inline-block border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300">Freebies</a>
                </li>
            </ul>
        </div>
        <div class="my-8">
            <ItemsGroup />
        </div>
        <div class="mx-5 md:mx-0 md:mt-20 block md:flex bg-amber-400 rounded-3xl py-10 px-3 md:px-10 justify-between">
            <p class="text-white text-2xl md:text-5xl md:ml-0 mb-2 md:mb-0 text-center md:text-left">
                Interested working with me?
            </p>
            <div class="flex justify-center items-center">
                <button class="px-10 py-3 bg-white rounded-xl flex justify-center items-center">
                    <img class="mr-3 cursor-pointer" src="src/assets/svg-icons/mail.svg" alt="mail">
                    <span class="text-gray-800 text-xl md:text-3xl">
                        Email Me
                    </span>
                </button>
            </div>
        </div>
    </div>
</template>

<script setup>
    import ItemsGroup from '../components/ItemsGroup.vue'
</script>