<template>
    <SchemaOrgLocalBusiness
      name="Lovina Ocean Tours" 
      image="/1.webp"
      description="Lovina Ocean Tour is a popular tour operator located in Lovina Beach, Bali, known for its scenic boat tours and water activities. you can enjoy dolphin watching, snorkeling, and diving in the crystal clear waters of the Bali Sea while taking in the breathtaking views of the surrounding coastline. The tour provides a memorable experience for travelers seeking adventure and relaxation in a beautiful tropical setting."
      telephone="+62831-1530-0070"
      :address="{
        streetAddress: 'Spice beach club, jln, Kaliasem, Kec. Banjar, Kabupaten Buleleng, Bali',
        addressLocality: 'Kadek Suara',
        addressRegion: 'IDN',
        postalCode: '81152',
        addressCountry: 'Indonesia',
      }"
    />
    <SchemaOrgWebSite name="Lovina Ocean Tours" />
    <SchemaOrgWebPage :type="['CollectionPage', 'SearchResultsPage']" />
  </template>
  