<template>
  <div class="container mx-auto my-16 sm:px-6 lg:px-8">
    <form method="post" class="bg-nav rounded mx-auto px-6 py-6 w-1/2">
      <div class="flex flex-col">
        <label for="name" class="text-white text-xl">Nama</label>
        <input
          type="text"
          name="name"
          v-model="name"
          class="px-2 py-1 rounded"
          placeholder="name"
        />
        <!-- <span class="text-red-200 italic" v-if="errors.name">{{
          errors.name[0]
        }}</span> -->
      </div>

      <div class="flex flex-col mt-3">
        <label for="email" class="text-white text-xl">Email</label>
        <input
          type="email"
          name="email"
          v-model="email"
          class="px-2 py-1 rounded"
          placeholder="email"
        />
        <!-- <span class="text-red-200 italic" v-if="errors.email">{{
          errors.email[0]
        }}</span> -->
      </div>

      <div class="flex flex-col mt-3">
        <label for="no_telp" class="text-white text-xl">No Telp</label>
        <input
          type="number"
          name="no_telp"
          v-model="no_telp"
          class="px-2 py-1 rounded"
          placeholder="no telp"
        />
        <!-- <span class="text-red-200 italic" v-if="errors.no_telp">{{
          errors.no_telp[0]
        }}</span> -->
      </div>

      <div class="flex flex-col mt-3">
        <label for="password" class="text-white text-xl">Password</label>
        <input
          type="password"
          name="password"
          id="password"
          v-model="password"
          class="px-2 py-1 rounded"
          placeholder="password"
        />
        <!-- <span class="text-red-200 italic" v-if="errors.password">{{
          errors.password[0]
        }}</span> -->
      </div>
      <div class="flex flex-col mt-3">
        <label for="c_password" class="text-white text-xl"
          >Konfirmasi Password</label
        >
        <input
          type="password"
          name="c_password"
          id="c_password"
          v-model="c_password"
          class="px-2 py-1 rounded"
          placeholder="konfirmasi password"
        />
        <!-- <span class="text-red-200 italic" v-if="errors.c_password">{{ errors.c_password[0] }}</span> -->
      </div>

      <div class="flex flex-col mt-3">
        <label for="angkatan" class="text-white text-xl">Angkatan</label>
        <select
          class="form-select px-4 py-2 rounded-lg w-full"
          name="angkatan"
          id="angkatan"
          v-model="angkatan"
        >
          <option value="" disabled selected>-- pilih angkatan --</option>
          <option value="">2022</option>
          <option value="">2023</option>
        </select>
        <!-- <span class="text-red-200 italic" v-if="errors.angkatan">{{
          errors.angkatan[0]
        }}</span> -->
      </div>

      <div class="flex flex-col mt-3">
        <label for="alamat" class="text-white text-xl">Alamat</label>
        <input
          type="text"
          name="alamat"
          v-model="alamat"
          class="px-2 py-1 rounded"
          placeholder="alamat"
        />
        <!-- <span class="text-red-200 italic" v-if="errors.alamat">{{
          errors.alamat[0]
        }}</span> -->
      </div>

      <div class="mt-3">
        <label for="jenis_kelamin" class="text-white text-xl"
          >Jenis Kelamin</label
        >
        <br />
        <input
          type="radio"
          v-model="jenis_kelamin"
          id="lk"
          name="jenis_kelamin"
          value="laki_laki"
        />
        <label for="laki_laki" class="text-white text-base">Laki-Laki</label
        ><br />
        <input
          type="radio"
          v-model="jenis_kelamin"
          id="pr"
          name="jenis_kelamin"
          value="perempuan"
        />
        <label for="perempuan" class="text-white text-base">Perempuan</label
        ><br />
        <!-- <span class="text-red-200 italic" v-if="errors.jenis_kelamin">{{
          errors.jenis_kelamin[0]
        }}</span> -->
      </div>

      <div class="flex flex-col mt-3">
        <label for="jurusan" class="text-white text-xl">Jurusan</label>
        <select
          class="form-select px-4 py-2 rounded-lg w-full"
          name="jurusan"
          id="jurusan"
          v-model="jurusan"
        >
          <option value="" disabled selected>-- pilih jurusan --</option>
          <option value="">D3 Teknik Informatika</option>
          <option value="">D3 Manajemen Informatika</option>
          <option value="">S1 Akuntansi</option>
        </select>
        <!-- <span class="text-red-200 italic" v-if="errors.jurusan">{{
          errors.jurusan[0]
        }}</span> -->
      </div>

      <div class="flex flex-col mt-3">
        <label for="nim" class="text-white text-xl">NIM</label>
        <input
          type="number"
          name="nim"
          v-model="nim"
          class="px-2 py-1 rounded"
          placeholder="nim"
        />
        <!-- <span class="text-red-200 italic" v-if="errors.nim">{{
          errors.nim[0]
        }}</span> -->
      </div>

      <div class="flex flex-col mt-3">
        <label for="posisi" class="text-white text-xl">Posisi Pemain</label>
        <select
          class="form-select px-4 py-2 rounded-lg w-full"
          name="posisi"
          id="posisi"
          v-model="posisi"
        >
          <option value="" disabled selected>-- pilih posisi --</option>
          <option value="">Spiker</option>
          <option value="">Setter/Tosser</option>
          <option value="">Libero</option>
          <!-- <option value="">yang lain...</option> -->
        </select>
        <!-- <div>
          <label for="yl">isi posisi anda</label>
          <br />
          <input
            type="text"
            name="yl"
            id="yl"
            class="form-input px-4 py-2 rounded-lg w-full"
          />
        </div> -->
        <!-- <span class="text-red-200 italic" v-if="errors.posisi">{{
          errors.posisi[0]
        }}</span> -->
      </div>

      <!-- <div class="flex flex-col mt-3">
        <label for="prestasi" class="text-white text-xl">PRESTASI</label>
        <input type="text" class="px-2 py-1 rounded" placeholder="prestasi" />
        <span class="text-red-200 italic">PRESTASI</span>
      </div> -->

      <div class="text-center mt-3">
        <button @click="signUpHandler">DAFTAR</button>
      </div>
    </form>
    <div class="text-center">
      <p>
        sudah punya akun?
        <NuxtLink to="/auth/login">Login!</NuxtLink>
      </p>

      <NuxtLink to="/">Halaman Utama</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  name: "Signup",
  data() {
    return {
      name: null,
      email: null,
      no_telp: null,
      password: null,
      c_password: null,
      angkatan: null,
      alamat: null,
      jenis_kelamin: null,
      jurusan: null,
      nim: null,
      posisi: null,
    };
  },
  methods: {
    async signUpHandler() {
      const data = {
        'name': this.name,
        'email': this.email,
        'no_telp': this.no_telp,
        'password': this.password,
        'c_password': this.c_password,
        'angkatan': this.angkatan,
        'alamat': this.alamat,
        'jenis_kelamin': this.jenis_kelamin,
        'jurusan': this.jurusan,
        'nim': this.nim,
        'posisi': this.posisi,
      };
      console.log(data);
      try {
        const res = await this.$axios.post("/register", data);
        console.log(res);
      } catch (e) {
        console.log(e.message);
      }
    },
  },
};
</script>
