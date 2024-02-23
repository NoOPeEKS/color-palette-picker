<script setup lang="ts"></script>
<template>
    <div
        class="grid w-full min-h-screen grid-cols-1 md:grid-cols-3 items-start justify-start py-12 gap-4 md:gap-8 px-4 md:px-6"
    >
        <div class="container grid max-w-5xl items-start justify-start gap-4">
            <h1 class="text-3xl font-bold tracking-tighter">
                Color Palette Picker
            </h1>
            <p class="text-gray-500">
                Select a color to copy to your clipboard.
            </p>
            <div
                class="grid w-full grid-cols-1 md:grid-cols-3 items-start justify-start gap-4 md:gap-6"
            >
                <div
                    class="relative flex items-center justify-center rounded-md border border-gray-200 bg-white shadow-sm w-full aspect-square border-gray-200 dark:border-gray-800 dark:bg-gray-950 dark:border-gray-800"
                >
                    <span
                        class="absolute inset-0 bg-red-500 opacity-30 rounded-md dark:bg-red-500"
                    ></span>
                    <div
                        class="absolute inset-0 flex items-end justify-center space-x-2 text-sm dark:text-gray-50"
                    >
                        <span>#ff4d4f</span>
                    </div>
                </div>
                <div
                    class="relative flex items-center justify-center rounded-md border border-gray-200 bg-white shadow-sm w-full aspect-square border-gray-200 dark:border-gray-800 dark:bg-gray-950 dark:border-gray-800"
                >
                    <span
                        class="absolute inset-0 bg-orange-500 opacity-30 rounded-md dark:bg-orange-500"
                    ></span>
                    <div
                        class="absolute inset-0 flex items-end justify-center space-x-2 text-sm dark:text-gray-50"
                    >
                        <span>#ff7a45</span>
                    </div>
                </div>
                <div
                    class="relative flex items-center justify-center rounded-md border border-gray-200 bg-white shadow-sm w-full aspect-square border-gray-200 dark:border-gray-800 dark:bg-gray-950 dark:border-gray-800"
                >
                    <span
                        class="absolute inset-0 bg-yellow-500 opacity-30 rounded-md dark:bg-yellow-500"
                    ></span>
                    <div
                        class="absolute inset-0 flex items-end justify-center space-x-2 text-sm dark:text-gray-50"
                    >
                        <span>#ffd666</span>
                    </div>
                </div>
                <div
                    class="relative flex items-center justify-center rounded-md border border-gray-200 bg-white shadow-sm w-full aspect-square border-gray-200 dark:border-gray-800 dark:bg-gray-950 dark:border-gray-800"
                >
                    <span
                        class="absolute inset-0 bg-lime-500 opacity-30 rounded-md dark:bg-lime-500"
                    ></span>
                    <div
                        class="absolute inset-0 flex items-end justify-center space-x-2 text-sm dark:text-gray-50"
                    >
                        <span>#aaf0d1</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
