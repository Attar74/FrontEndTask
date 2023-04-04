<template>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-14">
        <div v-for="(project, i) in projects" :key="i" class="px-5 md:px-0">
            <img width="540" height="380" class="transition duration-300 ease-in-out hover:scale-110 max-w-full rounded-lg cursor-pointer" :src="project.imgSrc" alt="image description">
            <div class="mt-7">
                <p class="text-warmGray-900 text-2xl text-center md:text-left">{{ project.title }}</p>
                <div class="md:flex mt-3">
                    <span class="flex justify-center md:justify-between">
                        <img class="mr-2 cursor-pointer" src="src/assets/svg-icons/layers.svg" alt="layers">
                        <span class="text-trueGray-900 lg:text-xl">View Study Case</span>
                    </span>
                    <span class="md:ml-5 flex justify-center md:justify-between">
                        <img width="18" class="mr-2 cursor-pointer" src="src/assets/svg-icons/show.svg" alt="show">
                        <span class="text-trueGray-900 lg:text-xl">Live Preview</span>
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { reactive } from "vue";

    const projects = reactive([
        {
            title: "Minify - Web Design",
            imgSrc: "src/assets/images/image.svg",
        },
        {
            title: "Ant - Personal Portofolio",
            imgSrc: "src/assets/images/image1.svg",
        },
        {
            title: "Lumy - Dashboard UI Kit",
            imgSrc: "src/assets/images/image2.svg",
        },
        {
            title: "Keeper - Soccer Site",
            imgSrc: "src/assets/images/image3.svg",
        },
    ])
</script>
