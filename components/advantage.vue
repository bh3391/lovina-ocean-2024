<template>
    <section class="text-gray-600  body-font">
        <div class="container px-5 py-24 mx-auto ">
            <div class="text-center mb-20">
                <h2 class="sm:text-3xl text-2xl font-bold text-center title-font text-gray-800 mb-4">Why You Should book
                    with us ?</h2>

            </div>
            <div class="flex flex-wrap  lg:w-4/5 sm:mx-auto sm:mb-2 -mx-2">
                <div v-for="(item, index) in dataAdvatages" :key="index" class="p-2 sm:w-1/2 w-full hover:scale-105 transition ">
                    <div  class="bg-[radial-gradient(ellipse_at_right,_var(--tw-gradient-stops))] from-sky-400 to-indigo-900 rounded flex p-4 h-full items-center">
                        <svg fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                            stroke-width="3" class="text-slate-50 w-6 h-6 flex-shrink-0 mr-4" viewBox="0 0 24 24">
                            <path d="M22 11.08V12a10 10 0 11-5.93-9.14"></path>
                            <path d="M22 4L12 14.01l-3-3"></path>
                        </svg>
                        <span class="title-font font-medium text-white">
                            <h2 class="font-bold"> {{ item.h2 }}</h2>
                            <p class="text-xs text-justify">
                                {{ item.p }}</p>
                        </span>

                    </div>


                </div>

            </div>
            <Booknow />
        </div>
    </section>
</template>
<script setup lang="ts">
const dataAdvatages = ref([
    {
        h2: 'Piloted By Real Fisherman',
        p: 'Our excursions are guided by experienced and passionate fishermen who bring genuine expertise to your adventure.Benefit from their in-depth knowledge of local waters, ensuring an authentic and rewarding experience on every journey.Join us and navigate the seas with skilled hands that  know the ins and outs of fishing, making each trip memorable and full of real, hands- on expertise.'
    },
    {
        h2: 'No Time Limit',
        p: 'just endless opportunities for discovery. Our experiences are designed with the freedom to immerse yourself in the moment, whether its exploring the great outdoors, savoring the journey, or simply enjoying quality time with loved ones. Embrace the luxury of unlimited time as you create memories that last a lifetime. Your adventure, your pace—no constraints, only possibilities.'
    },
    {
        h2: 'We Have Large Parking Space',
        p: 'Enjoy the freedom of our large parking space, designed to accommodate your needs without the worry of limited availability. Whether youre visiting for an event, shopping, or a night out, rest assured that our expansive parking area is here to make your experience stress-free. '
    },
    {
        h2: 'Special Boat For Dolphin & Snorkling Tour',
        p: 'Dive into the magic of the ocean with our special boat designed exclusively for Dolphin & Snorkeling Tours! 🚤🐬 Immerse yourself in an unparalleled experience as you sail on a vessel crafted for comfort, safety, and optimal marine exploration. Join us for an unforgettable journey where every detail is tailored for your enjoyment.'
    },
    {
        h2: 'There Are Toilets , Restrooms & Coffe Shop on site.',
        p: 'Your comfort is our priority! Enjoy the convenience of on-site facilities with clean and accessible toilets, restrooms, and a cozy coffee shop. Whether youre here for an event, a day of exploration, or simply passing by, take a break with the assurance of well-maintained facilities. Enhance your experience with a refreshing cup of coffee, and rest easy knowing that all your needs are taken care of at our location. Your satisfaction is our commitment!'
    },
    {
        h2: 'Free Pick up by Boat or Motorbike for Hotel near Lovina Area.',
        p: 'Elevate your stay in Lovina with our complimentary pick-up service for hotels in the vicinity! Enjoy the convenience of a hassle-free journey as we ensure youre comfortably transported to your destination. Whether youre joining us for a dolphin tour, snorkeling adventure, or any other experience, our complimentary pick-up service by boat or motorbike adds an extra layer of convenience to your visit. Sit back, relax, and let us take care of the details.'
    },
    // Add more user objects as needed
]);
</script>