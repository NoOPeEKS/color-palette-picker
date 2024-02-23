<script setup lang="ts">
import AuthenticatedLayout from "@/Layouts/AuthenticatedLayout.vue";
import { Head } from "@inertiajs/vue3";
import { Button } from "@/Components/ui/button";
import {
    Accordion,
    AccordionContent,
    AccordionItem,
    AccordionTrigger,
} from "@/Components/ui/accordion";

const defaultValue = "item-1";

const accordionItems = [
    {
        value: "item-1",
        title: "Is it accessible?",
        content: "Yes. It adheres to the WAI-ARIA design pattern.",
    },
    {
        value: "item-2",
        title: "Is it unstyled?",
        content:
            "Yes. It's unstyled by default, giving you freedom over the look and feel.",
    },
    {
        value: "item-3",
        title: "Can it be animated?",
        content:
            "Yes! You can use the transition prop to configure the animation.",
    },
];
</script>

<template>
    <Head title="Dashboard" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Dashboard
            </h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                <div class="bg-white overflow-hidden shadow-sm sm:rounded-lg">
                    <div class="p-6 text-gray-900">You're logged in!</div>
                    <Button variant="destructive">Destructive</Button>
                    <Accordion
                        type="single"
                        class="w-full"
                        collapsible
                        :default-value="defaultValue"
                    >
                        <AccordionItem
                            v-for="item in accordionItems"
                            :key="item.value"
                            :value="item.value"
                        >
                            <AccordionTrigger>{{
                                item.title
                            }}</AccordionTrigger>
                            <AccordionContent>
                                {{ item.content }}
                            </AccordionContent>
                        </AccordionItem>
                    </Accordion>
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>
