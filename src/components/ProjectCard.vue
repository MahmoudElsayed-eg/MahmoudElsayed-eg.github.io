<template>
    <div class="border border-gray-700 flex flex-col">
        <h3 class="font-medium text-xl p-5">{{ title }}</h3>
        <div class="flex gap-1 justify-around">
            <video class="w-full max-w-xs sm:max-w-sm md:max-w-md max-h-80" v-for="(item, index) in videos" :key="index" controls>
                <source :src="'/videos/'+item" type="video/mp4">
                Your browser does not support the video tag.
            </video>
        </div>
        <div class="p-5 space-y-3 text-gray-300">
            <p class="text-gray-400" v-html="desc">
            </p>
           
        </div>
    </div>
</template>
<script setup>
defineProps({
title:String,
desc:String,
videos:Array,
}
)
</script>