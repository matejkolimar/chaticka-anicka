<template>
  <!-- Best cabin amenities like view, terrace, grill,... -->
  <section
    class="flex flex-col md:flex-row bg-white py-10 md:py-16 px-2 md:px-20 gap-2">
    <!-- Exterior amenities -->
    <div class="flex md:w-1/3 md:justify-center">
      <ul class="w-full md:max-w-md">
        <p class="p-4 mb-3 text-center font-bold text-xl">Exteriér</p>
        <li
          v-for="amenity in exterior"
          :key="amenity.id"
          class="p-4 mb-3 flex justify-between bg-white shadow rounded-lg">
          <div class="flex items-center">
            <img class="w-10 h-10" :src="amenity.img" :alt="amenity.name" />
            <p class="ml-2 text-gray-700 font-semibold font-sans tracking-wide">
              {{ amenity.name }}
            </p>
          </div>
        </li>
      </ul>
    </div>

    <!-- Interior amenities -->
    <div class="flex md:w-1/3 md:justify-center">
      <ul class="w-full md:max-w-md">
        <p class="p-4 mb-3 text-center font-bold text-xl">Interiér</p>
        <li
          v-for="amenity in interior"
          :key="amenity.id"
          class="p-4 mb-3 flex justify-between bg-white shadow rounded-lg">
          <div class="flex items-center">
            <img class="w-10 h-10" :src="amenity.img" :alt="amenity.name" />
            <p class="ml-2 text-gray-700 font-semibold font-sans tracking-wide">
              {{ amenity.name }}
            </p>
          </div>
        </li>
      </ul>
    </div>

    <!-- Kitchen amenities -->
    <div class="flex md:w-1/3 md:justify-center">
      <ul class="w-full md:max-w-md">
        <p class="p-4 mb-3 text-center font-bold text-xl">Kuchyňa</p>
        <li
          v-for="amenity in kitchen"
          :key="amenity.id"
          class="p-4 mb-3 flex justify-between bg-white shadow rounded-lg">
          <div class="flex items-center">
            <img class="w-10 h-10" :src="amenity.img" :alt="amenity.name" />
            <p class="ml-2 text-gray-700 font-semibold font-sans tracking-wide">
              {{ amenity.name }}
            </p>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      exterior: [
        {
          id: 1,
          name: 'Výhľad na jazero',
          img: '../assets/images/svg/view.svg',
        },
        {
          id: 1,
          name: 'Krb a ohnisko',
          img: '../assets/images/svg/grill.svg',
        },
        {
          id: 1,
          name: 'Parkovanie v objekte',
          img: '../assets/images/svg/parking.svg',
        },
        {
          id: 1,
          name: 'Terasa',
          img: '../assets/images/svg/terrace.svg',
        },
        {
          id: 1,
          name: 'Vonkajšie stolovanie',
          img: '../assets/images/svg/outside-place.svg',
        },
      ],
      interior: [
        {
          id: 1,
          name: '3 kúpeľne s wc a sprchovým kútom',
          img: '../assets/images/svg/shower.svg',
        },
        {
          id: 1,
          name: '3 Spálne s možnosťou voľby postelí. ',
          img: '../assets/images/svg/single-bed.svg',
        },
        {
          id: 1,
          name: 'Manželská posteľ alebo jednolôžkova posteľ',
          img: '../assets/images/svg/master-bed.svg',
        },
        {
          id: 1,
          name: 'Posteľná bielizeň',
          img: '../assets/images/svg/bed-sheets.svg',
        },
        {
          id: 1,
          name: 'Úložný priestor na oblečenie',
          img: '../assets/images/svg/storage.svg',
        },
      ],
      kitchen: [
        {
          id: 1,
          name: 'Chladnička',
          img: '../assets/images/svg/freezer.svg',
        },
        {
          id: 2,
          name: 'Riad, hrnce a príbory',
          img: '../assets/images/svg/kitchen-stuff.svg',
        },
        {
          id: 3,
          name: 'Elektrický sporák',
          img: '../assets/images/svg/electric-oven.svg',
        },
        {
          id: 4,
          name: 'Rýchlovarná kanvica',
          img: '../assets/images/svg/electric-kettle.svg',
        },
        {
          id: 5,
          name: 'Mikrovlnná rúra',
          img: '../assets/images/svg/microwave.svg',
        },
      ],
    }
  },
}
</script>

<style scoped></style>
