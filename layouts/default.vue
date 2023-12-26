<template>
    <SeoKit />
    <Schema />
    <NuxtLoadingIndicator />
    <Header />
    <div style="font-family: 'Poppins';" class="container text-gray-800 max-w-7xl bg-white mx-auto">
        <slot />
    </div>
    <Footer />
</template>
<style>


;
/* Define the initial state of the element */
</style>
<script setup>
useHead({
    script: [
        {
            hid: 'gtm-script',
            src: 'https://www.googletagmanager.com/gtm.js?id=GTM-PGGDNB8D',
            async: true,
            defer: true,
        },
    ],
}),


useSeoMeta({
    title: 'Best Price Guaranteed: #1 Lovina Dolphin Tours',
    ogTitle: 'Lovina Dolphin Tour  Services | Best Price Guaranteed',
    description: 'Discover Lovina Ocean Tour: Exciting boat tours, dolphin watching, snorkeling, and diving in Bali crystal-clear waters. Memorable adventures and relaxation in a tropical paradise.',
    ogDescription: 'Discover Lovina Ocean Tour: Exciting boat tours, dolphin watching, snorkeling, and diving in Balis crystal-clear waters. Memorable adventures and relaxation in a tropical paradise.',
    ogImage: 'https://lovinaoceantours/1.webp',
    twitterCard: 'summary_large_image',
})
</script>