<template>
  <section id="formLogin" class="formLogin">
    <div
      class="
        columns-1
        sm:columns-1
        md:columns-1
        lg:columns-2
        xl:columns-2
        bg-slate-50
      "
    >
      <div class="flex justify-center items-center h-screen w-full">
        <div class="flex items-center">
          <div class="h-96 w-[400px] bg-white rounded-lg shadow-xl px-6">
            <div class="justify-center items-center h-full w-full">
              <img src="~/static/logo.png" alt="avbc" width="60" height="60" />
              <h1>Lorem ipsum dolor sit amet.</h1>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Inventore, dolor?
              </p>

              <form action="">
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
                  <label for="password">Password</label>
                  <br />
                  <input
                    type="password"
                    name="password"
                    id="paassword"
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
                      belum punya akun?
                      <NuxtLink to="/register">Daftar!</NuxtLink>
                    </p>

                    <NuxtLink to="/login">Halaman Utama</NuxtLink>
                  </div>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>

      <div class="w-screen h-screen">
        <img
          src="~/static/avbc/6.jpg"
          alt="avbc"
          class="w-full h-full overflow-hidden"
        />
      </div>
    </div>
  </section>
</template>
