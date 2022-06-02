<template>
  <!-- Hero Section Start -->

  <section id="home" class="pt-36 bg-nav dark:bg-slate-800">
    <div class="container">
      <div class="flex flex-wrap">
        <div class="w-full self-center px-4 lg:w-1/2">
          <h1 class="text-base font-semibold text-primary md:text-xl">
            Halo Semua 👋
            <span
              class="
                block
                font-bold
                text-white text-4xl
                mt-1
                lg:text-5xl
                dark:text-white
              "
              >AMIKOM VOLLEYBALL CLUB</span
            >
          </h1>
          <h2 class="font-medium text-tri text-lg mb-5 lg:text-2xl">
            Komunitas Olahraga
            <span class="text-dark dark:text-white font-bold">Bola Voli</span>
          </h2>
          <p
            class="font-medium text-gray-300 mb-10 leading-relaxed text-justify"
          >
            Amikom Volleyball Club (AVBC) adalah salah satu komunitas kegiatan
            olahraga di Universitas Amikom Yogyakarta yang diperuntukkan bagi
            mahasiswa yang mau mendalami atau menyalurkan bakat dan minat di
            bidang olahraga bola voli.
            <span class="text-dark font-bold tracking-wide dark:text-white"
              >Pelaksanaan kegiatan ini dilaksanakan dibawah bimbingan komunitas
              voli di AMIKOM yaitu AVBC.</span
            >
          </p>

          <div class="flex">
            <NuxtLink
              to="/register"
              class="
                text-base
                font-semibold
                text-white
                bg-primary
                py-3
                px-8
                rounded-full
                hover:shadow-lg hover:shadow-primary
                transition
                duration-300
                ease-in-out
                shadow-white shadow-sm
                font-bold
              "
              >
              <span class="animate-pulse">{{ !buttonRegister.open ? buttonRegister.msg : 'Daftar Sekarang!' }}</span>
              </NuxtLink
            >
            <NuxtLink
              to="#contact"
              class="
                text-base
                font-semibold
                text-white
                shadow-white shadow-sm
                py-3
                px-8
                mx-2
                rounded-full
                hover:shadow-md hover:shadow-white
                transition
                duration-300
                ease-in-out
              "
              >Hubungi Kami</NuxtLink
            >
          </div>
        </div>

        <div class="w-full self-end px-4 lg:w-1/2">
          <div class="mt-10 relative lg:mt-0 lg:right-0">
            <img
              src="~/static/logo.png"
              alt="AVBC"
              class="max-w-full mx-auto scale-90 relative z-10"
            />
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Hero Section End -->
</template>

<script>
export default {
  data() {
    return {
      buttonRegister: {
        open: false,
        msg: null
      },
    };
  },
  mounted() {
    this.cekHariPendaftaran();
  },
  methods: {
    cekHariPendaftaran() {
      const that = this;
      this.$axios
        .get("public/hari-pendaftaran")
        .then(({ data }) => {
          this.buttonRegister.open = data.data.open;
          this.buttonRegister.msg = data.message
        })
        .catch((err) => {
          console.log(err);
        });
    },
  },
};
</script>