<template>
    <div class="rounded-lg lg:p-5 mx-auto bg-[radial-gradient(ellipse_at_bottom_right,_var(--tw-gradient-stops))] from-blue-100 via-blue-200 to-blue-300">
        <div class="text-center lg:mb-20">
            <h2 class="sm:text-3xl text-2xl font-bold text-center title-font text-gray-800 mb-4">Our Tour Packages</h2>

        </div>
        <div class="flex flex-col sm:grid sm:grid-cols-1 justify-center items-center  md:grid-cols-2   lg:grid-cols-4 gap-1 max-w-8-xl sm:mx-auto sm:mb-2 ">
            <div v-for="(item, index) in packages" :key="index"
                class="sm:p-2  mx-auto  w-screen p-1 sm:w-80 md:w-72    bg-white border border-1 rounded-lg hover:shadow-lg text-sm  ">


            
                
                <div class=" max-sm p-1">
                    <NuxtImg class=" mx-auto" :src="item.image" :alt="item.title"  format="webp"/>
                    <NuxtLink :href="item.link" :alt="item.title"><h3 class="text-lg mb-1 bg-sky-600 text-white px-1 font-bold hover:underline">{{ item.title }}</h3></NuxtLink>
                    <p :class="item.status">Sharing Boat : IDR {{ item.sharing }}K/person</p>
                    <p :class="item.status">Private Boat : IDR {{ item.private }}K/person</p>
                    <p>Include : {{ item.include }}</p>
                    <p>Duration : {{ item.duration }}</p>
                    <Booknow />
                </div>



            </div>

        </div>

    </div>
</template>
<script setup lang="ts">
const packages = ref([
    { id: 1, image:'dolphin-watching-tour.png',title: 'Sunrise dolphin watching tour', sharing: '100', private: '150', include: 'Life Jacket. Equipment.', duration: '2 hours',link:"/lovina-dolphin-watching-tour" },
    { id: 2, image:'dolphin-and-swimming.png',title: 'Dolphin watching and swimming with dolphins', sharing: '200', private: '250', include: 'Life Jacket. Equipment.', duration: '3 hours',link:"/lovina-dolphin-and-swimming-with-dolphin" },
    { id: 3, image:'dolphin-and-snorkeling.png',title: 'Dolphin watching and Snorkeling coral reef', sharing: '200', private: '250', include: 'Life Jacket. Equipment.', duration: '3 hours',link:"/lovina-dolphin-and-snorkeling" },
    { id: 4, image:'dolphin-swim-and-snorkeling.png',title: 'Dolphin watching, swim with dolphin and Snorkeling coral reef', sharing: '300', private: '350', include: 'Life Jacket. Equipment.', duration: '3 hours',link:"/lovina-dolphin-watching-snorkeling-and-swimming-with-dolphin" },
    { id: 5, image:'sunset-tour-with-plankton.png',title: 'Sunset tour and Swim with Plankton', sharing: '200', private: '250', include: 'Life Jacket. Equipment.', duration: '3 hours',link:"/sunset-plankton-tour" },
    { id: 6, image:'sunset-tour-fishing-fish.png',title: 'Sunset tour and fishing fish', sharing: '250', private: '300', include: 'Life Jacket. Equipment.', duration: '3 hours',link:"/fishing-tour-at-lovina" },
    { id: 8, image:'snorkeling-at-coral-reef.png',title: 'Snorkeling at Coral Reef', sharing: '100', private: '150', include: 'Life Jacket. Equipment.', duration: '2 hours',link:"/lovina-snorkeling-at-coral-reef" },
    { id: 7, image:'transfer-pick-up-area-bali.png',title: 'Transfer pick up at area Bali Fixed Price 600K/car/way', sharing: '600K', private: '', include: 'Car, Driver, Petrol', duration: 'Depend on Your Location',status:'hidden',link:"/transport-service" },
])
</script>