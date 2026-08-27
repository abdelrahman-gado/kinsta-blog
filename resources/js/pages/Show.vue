<script setup>
import KinstaLayout from '../Layouts/KinstaLayout.vue';

defineProps({
    article: Object,
});
</script>

<template>
    <KinstaLayout>
        <article class="mx-auto mt-10 flex max-w-5xl justify-center border-b-2">
            <img
                src="/images/kinsta-logo.png"
                class="mx-auto h-80 w-80 rounded-xl py-5"
                alt=""
            />
            <div class="flex flex-col px-10 pt-5 pb-10 text-left">
                <h1 class="mb-10 text-xl font-semibold">{{ article.title }}</h1>
                <p>{{ article.body }}</p>
            </div>
        </article>
    </KinstaLayout>
</template>
