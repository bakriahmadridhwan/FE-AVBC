<template>
  <section id="formRegister" class="formRegister">
    <div class="flex justify-center items-center w-full">
      <div class="flex items-center">
        <div class="w-[800px] bg-white rounded-lg shadow-xl px-6">
          <div class="justify-center items-center w-full">
            <img src="~/static/logo.png" alt="avbc" width="60" height="60" />
            <h1>Lorem ipsum dolor sit amet.</h1>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Inventore, dolor?
            </p>

            <form action="">
              <div>
                <label for="name">Nama</label>
                <br />
                <input
                  type="text"
                  name="name"
                  id="name"
                  class="form-input px-4 py-2 rounded-lg w-full"
                />
              </div>

              <div>
                <label for="email">Email</label>
                <br />
                <input
                  type="email"
                  name="email"
                  id="email"
                  class="form-input px-4 py-2 rounded-lg w-full"
                />
              </div>

              <div>
                <label for="no_telp">Nomor Telfon</label>
                <br />
                <input
                  type="number"
                  name="no_telp"
                  id="no_telp"
                  class="form-input px-4 py-2 rounded-lg w-full"
                />
              </div>

              <div>
                <label for="password"
                  >Password (digunakan untuk login akun)</label
                >
                <br />
                <input
                  type="password"
                  name="password"
                  id="paassword"
                  class="form-input px-4 py-2 rounded-lg w-full"
                />
              </div>

              <div>
                <label for="password">Konfirmasi Password</label>
                <br />
                <input
                  type="password"
                  name="password"
                  id="paassword"
                  class="form-input px-4 py-2 rounded-lg w-full"
                />
              </div>

              <div>
                <label for="angkatan">Angkatan</label>
                <br />
                <select
                  class="form-select px-4 py-2 rounded-lg w-full"
                  name="angkatan"
                  id="angkatan"
                >
                  <option value="" disabled selected>
                    -- pilih angkatan --
                  </option>
                  <option value="">2022</option>
                  <option value="">2023</option>
                </select>
              </div>

              <div>
                <label for="alamat">Alamat</label>
                <br />
                <input
                  type="text"
                  name="alamat"
                  id="alamat"
                  class="form-input px-4 py-2 rounded-lg w-full"
                />
              </div>

              <div>
                <label for="jk">Jenis Kelamin</label>
                <br />
                <input type="radio" id="lk" name="fav_language" value="lk" />
                <label for="lk">Laki-Laki</label><br />
                <input type="radio" id="pr" name="fav_language" value="pr" />
                <label for="pr">Perempuan</label><br />
              </div>

              <div>
                <label for="jurusan">Jurusan</label>
                <br />
                <select
                  class="form-select px-4 py-2 rounded-lg w-full"
                  name="jurusan"
                  id="jurusan"
                >
                  <option value="" disabled selected>
                    -- pilih jurusan --
                  </option>
                  <option value="">D3 Teknik Informatika</option>
                  <option value="">D3 Manajemen Informatika</option>
                </select>
              </div>

              <div>
                <label for="nim">NIM</label>
                <br />
                <input
                  type="number"
                  name="nim"
                  id="nim"
                  class="form-input px-4 py-2 rounded-lg w-full"
                />
              </div>

              <div>
                <label for="posisi">Posisi Pemain</label>
                <br />
                <select
                  class="form-select px-4 py-2 rounded-lg w-full"
                  name="posisi"
                  id="posisi"
                >
                  <option value="" disabled selected>-- pilih posisi --</option>
                  <option value="">Spiker</option>
                  <option value="">Setter/Tosser</option>
                  <option value="">Libero</option>
                  <option value="">yang lain...</option>
                </select>
                <div>
                  <label for="yl">isi posisi anda</label>
                  <br />
                  <input
                    type="text"
                    name="yl"
                    id="yl"
                    class="form-input px-4 py-2 rounded-lg w-full"
                  />
                </div>
              </div>

              <div>
                <label for="prestasi">Prestasi</label>
                <br />
                <input
                  type="text"
                  name="prestasi"
                  id="prestasi"
                  class="form-input px-4 py-2 rounded-lg w-full"
                />
              </div>

              <div>
                <button
                  class="
                    py-2
                    px-4
                    bg-primary
                    text-white
                    font-bold
                    w-full
                    mx-auto
                    rounded-xl
                    my-4
                  "
                >
                  Login
                </button>
                <div class="text-center">
                  <p>
                    sudah punya akun?
                    <NuxtLink to="/login">Daftar!</NuxtLink>
                  </p>

                  <NuxtLink to="/">Halaman Utama</NuxtLink>
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style></style>
<script></script>
  ``
