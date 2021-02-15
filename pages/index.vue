<template>
  <div>
    <Menu />
    <Hero />
    <BannerCreateAccount />
    <Features />
    <Carrousel />
    <BannerCreateAccountSecond />
    <Footer />
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>
