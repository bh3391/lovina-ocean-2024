<template>
    <section class="body-font">
        <div class="container px-5 py-24 mx-auto flex flex-col">
            <div class="lg:w-4/6 mx-auto">


                <div class=" flex  flex-col text-center justify-center sm:pr-8 sm:py-8">
                    <h2 class="text-xl font-bold "> About Us!</h2><br>
                    <div class="w-full inline-flex items-center  text-gray-400">
                        <div class="mx-auto">
                            <nuxt-img class="rounded hidden sm:block" loading="lazy" width="425" height="275" format="webp"
                                src="/kadek.jpeg" alt="Foto Pak Kadek" />
                            <nuxt-img class="rounded sm:hidden" loading="lazy" width="425" height="275" format="webp"
                                src="/kadek.jpeg" alt="Foto Pak Kadek" />
                            <h2 class="text-lg  text-gray-800 mt-4 ">Kadek Suara</h2>
                            
                        </div>
                    </div>
                    <div class="flex flex-col p-2 md:p-4 items-center text-justify justify-center">

                       
                        <p class="text-sm md:text-md  ">Introducing Captain Kadek!!<br>

                            Lovina Ocean Tour is a Professional Dolphin Tour Package Service Provider @ Lovina Beach,
                            Singaraja-Bali,
                            Captain Kadek has experience providing Dolphin Tour services since 1988.
                            <br>We are committed to provide the best service to our customers. Apart from being a Dolphin
                            tour service provider, we also provide Snorkeling and Diving services at Lovina Beach
                        </p>
                        <Booknow />
                    </div>
                </div>


            </div>
        </div>
</section></template>