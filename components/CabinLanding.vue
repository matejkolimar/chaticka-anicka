<template>
  <!-- Cabin landing image with logo, and slogan. -->
  <section
    id="app"
    class="hero min-h-screen"
    style="background-image: url('assets/images/wide-house.jpeg')">
    <div class="hero-overlay bg-opacity-40"></div>
    <div class="hero-content text-center text-neutral-content">
      <div class="max-w-md">
        <h1 class="mb-5 text-5xl font-bold">Chaticka Anicka</h1>
        <p class="mb-5">
          To je oaza kludu a pokoja na krasnom a tichom mieste...
        </p>
        <button class="btn btn-primary" @click.prevent="btnPress">
          Kontakt
        </button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection',
  setup() {
    onMounted(() => {
      themeChange(false)
    })
  },
  methods: {
    btnPress() {
      return console.log('Press button')
    },
  },
}
</script>

<style scoped></style>
