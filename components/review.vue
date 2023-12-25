<template>
    <div class="max-w-7xl mx-auto bg-slate-100 my-5 p-2 rounded-lg">
        <div class="flex flex-row">
            <h2 class="text-3xl w-4/5 ml-4 text-left my-4 font-bold "> What our customer say about us ?</h2><hr>
            <div class="text-center my-4 font-bold">Google Rating Score <br><span class="p-1 rounded-full text-2xl  text-orange-600">4,9<br>Excellent</span></div>
        </div>
       
        <div class="flex flex-wrap flex-col gap-2 md:grid md:grid-cols-2 lg:grid-cols-3">
            <div v-for="(item, index) in reviews" :key="index"
                class="p-2  w-full  bg-white border border-1 rounded-lg hover:shadow-lg text-xs hover:scale-105 transition ">
                <div class="p-1 mb-1">
                    <div class="flex flex-row">
                        <div class="w-9 text-center p-1 rounded bg-blue-500 text-white text-xl rounded-full font-bold">{{ item.photo }}</div>
                        <div class="text-md px-2 text-left font-bold">{{ item.name }}<br> {{ item.review }}. {{ item.date }}</div>
                    </div><hr>
                    <div class="text-justify text-xs p-1 ">
                        <p>{{ item.description }}</p>
                    </div><hr>
                    <a class="text-blue-600 hover:underline" target="blank" href="https://maps.app.goo.gl/HZFgwCf3ZKtD4ciTA" alt="Read Review At Google">Read Review at Google</a>
                </div>



            </div>

        </div>

    </div>
</template>
<script setup lang="ts">
const reviews = ref([
    {
        id: 1,
        photo: "S",
        name: "Simone Capone",
        review: "Local Guide ",
        description: "Esperienza fantastica, il ragazzo che ti porta è veramente disponibile e ti porta nel posto più adatto per vedere i delfini, è stata veramente unica non pensavo di potermi emozionare cosi. Ti fa anche foto e video mentre te sei in acqua. Grazie mille di tutto",
        rating: "5",
        date: 'Dec 2023',

    },
    {
        id: 2,
        photo: "I",
        name: "Ilja Huigen",
        review: "Local Guide ",
        description: "100% een aanrader!! Éen van de hoogtepunten van de vakantie. Alle tijd en kansen om veel dolfijnen te zien, ook van dichtbij. Prachtig! Erg leuke gids (Budi), liet ons ook helpen met de boot besturen.",
        rating: "5",
        date: 'Dec 2023',

    },
    {
        id: 5,
        photo: "M",
        name: "Maria Zammit",
        review: "Local Guide ",
        description: "This is one of the best experiences I have had so far in Bali! The captain was very friendly and took is to the best parts to see loads of dolphins and we had the chance to take amazing videos and photos! Support this man and book this activity because you will not only enjoy seeing the dolphins but the captain makes your day!",
        rating: "5",
        date: 'Jul 2023',

    },
    {
        id: 3,
        photo: "K",
        name: "Karim Ramaki",
        review: "Local Guide ",
        description: "Good communication about the options via Whatsapp and great tour guide on the boat, who was flexible and relaxed. Unfortunately the other people were sick and cancelled, so I was alone on the tour, but also had its benefits. Though, it would have been more sustainable considering fuel to mix with other groups and is an idea for them to consider. I went dolphin watching and snorkeling. I did a lot of reading beforehand about animal friendly dolphin tours, and ended up with this tour operator based on reviews and not swimming with the dolphins to disturb them as little as possible while still doing the tour. Even though the tour guide also went a little in the direction of the dolphins, but he turned his engine off before coming close and tried to stay on the outside of the group (not always), to make dolphins come to us andto prevent chasing the dolphins like crazy as some other boats did.",
        rating: "5",
        date: 'Jul 2023',

    },
   
    {
        id: 4,
        photo: "F",
        name: "Frank. S",
        review: "Local Guide ",
        description: "Wir sind in der Früh los ind eollte Delphine sehen. Nang Unser Reiseführer hat uns hingefahren und alles organisiert. Bor Sonnenaufgang waren wir auf dem Meer und es dauerte gar nicht lange da haben wir die ersten Flipper gesehen. Es war rin einzigartiges Erlebnis. Megaschön und sehr eindrucksvoll wie die Tiere sich durch das Wasser bewegten. Wir konnten uns auch am Boot festhalten und wurden durchs Wasser gezogen. Hierbei konnte man auch die Delphine unter Wasser betrachten. Sehr tolles Erlebnis.",
        rating: "5",
        date: 'Aug 2023',

    },
    {
        id: 6,
        photo: "A",
        name: "Amandine Constant",
        review: "Local Guide ",
        description: "Expérience inoubliable 😍🐬Nous avons pu passer presque 4h sur l’eau en compagnie des dauphins qui nous ont offert un spectacle incroyable !Puis nous avons nagé avec eux    réellement, masque & tuba fournis plus qu’à les admirer et les laisser vous approcher et nager dans les profondeurs pour ensuite réapparaître !Ouvrez grands les yeux ils peuvent être plus proches que ce que vous cherchez !Les équipes sont au top, chaleureuse, vous êtes de suite à l’aise et il font tout pour vous !",
        rating: "5",
        date: 'Aug 2023',

    },
])

</script>