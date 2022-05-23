<template>
  <!-- Navbar Start -->

  <header
    class="bg-transparent absolute top-0 left-0 w-full flex items-center z-10"
  >
    <img
      src="~/static/logo.png"
      alt="avbc"
      width="50"
      height="50"
      class="ml-12"
    />

    <div class="container">
      <div class="flex items-center justify-between relative">
        <div class="px-4">
          <a
            href="#home"
            class="font-bold text-2xl text-white block py-6 hover:text-primary"
            >AVBC</a
          >
        </div>

        <div class="flex items-center px-4">
          <button
            id="hamburger"
            name="hamburger"
            class="absolute block right-4 lg:hidden"
            type="button"
          >
            <span
              class="
                hamburger-line
                transition
                duration-500
                ease-in-out
                origin-top-left
              "
            ></span>
            <span
              class="
                w-5
                h-0.5
                my-2
                block
                bg-white
                transition
                duration-500
                ease-in-out
              "
            ></span>
            <span
              class="
                hamburger-line
                transition
                duration-500
                ease-in-out
                origin-bottom-left
              "
            ></span>
          </button>

          <nav
            id="nav-menu"
            class="
              hidden
              absolute
              py-5
              bg-nav
              max-w-[250px]
              w-full
              rounded-lg
              shadow-lg
              right-4
              top-full
              lg:block
              lg:static
              lg:bg-transparent
              lg:max-w-full
              lg:rounded-none
              lg:shadow-none
              lg:font-bold
              dark:bg-dark dark:shadow-slate-500
              lg:dark:bg-transparent
            "
          >
            <ul class="block lg:flex">
              <li class="flex items-center pl-8 mt-3 lg:mt-0">
                <div class="flex">
                  <label
                    for=""
                    class="w-6 h-6 mx-2 flex justify-center items-center"
                  >
                    <svg
                      role="img"
                      viewBox="0 0 24 24"
                      xmlns="http://www.w3.org/2000/svg"
                      aria-labelledby="color-scheme-light"
                    >
                      <path
                        d="M12 18c-3.309 0-6-2.691-6-6s2.691-6 6-6 6 2.691 6 6-2.691 6-6 6zm0-10c-2.206 0-4 1.794-4 4s1.794 4 4 4 4-1.794 4-4-1.794-4-4-4zm0-4a1 1 0 0 1-1-1V1a1 1 0 0 1 2 0v2a1 1 0 0 1-1 1zm0 20a1 1 0 0 1-1-1v-2a1 1 0 1 1 2 0v2a1 1 0 0 1-1 1zM5.64 6.64a.997.997 0 0 1-.707-.293l-1.42-1.42a.999.999 0 1 1 1.414-1.414l1.42 1.42A.999.999 0 0 1 5.64 6.64zm14.139 14.139a.997.997 0 0 1-.707-.293l-1.42-1.42a.999.999 0 1 1 1.414-1.414l1.42 1.42a.999.999 0 0 1-.707 1.707zM3 13H1a1 1 0 1 1 0-2h2a1 1 0 0 1 0 2zm20 0h-2a1 1 0 1 1 0-2h2a1 1 0 1 1 0 2zM4.22 20.779a.999.999 0 0 1-.707-1.707l1.42-1.42a.999.999 0 1 1 1.414 1.414l-1.42 1.42a.993.993 0 0 1-.707.293zM18.359 6.64a.999.999 0 0 1-.707-1.707l1.42-1.42a.999.999 0 1 1 1.414 1.414l-1.42 1.42a.997.997 0 0 1-.707.293z"
                        class="fill-white"
                      ></path>
                    </svg>
                  </label>
                  <input type="checkbox" class="hidden" id="dark-toggle" />
                  <label for="dark-toggle">
                    <div
                      class="
                        flex
                        h-5
                        w-9
                        cursor-pointer
                        items-center
                        rounded-full
                        bg-slate-500
                        p-1
                      "
                    >
                      <div
                        class="
                          toggle-circle
                          h-4
                          w-4
                          rounded-full
                          bg-white
                          transition
                          duration-300
                          ease-in-out
                        "
                      ></div>
                    </div>
                  </label>
                  <label
                    for=""
                    class="w-6 h-6 mx-2 flex justify-center items-center"
                  >
                    <svg
                      role="img"
                      viewBox="0 0 24 24"
                      xmlns="http://www.w3.org/2000/svg"
                      aria-labelledby="color-scheme-dark"
                    >
                      <path
                        d="M12.048 21.963c-.308 0-.618-.015-.93-.043-2.66-.246-5.064-1.513-6.771-3.567s-2.512-4.651-2.266-7.311a10.004 10.004 0 0 1 9.038-9.038 1 1 0 0 1 .896 1.589 6.008 6.008 0 0 0 1.258 8.392c2.078 1.536 5.055 1.536 7.133 0a1 1 0 0 1 1.591.896 9.951 9.951 0 0 1-9.949 9.082zM9.315 4.438a8.006 8.006 0 0 0-5.244 6.787 7.954 7.954 0 0 0 1.813 5.849 7.95 7.95 0 0 0 5.417 2.854 7.95 7.95 0 0 0 8.266-5.243 8.01 8.01 0 0 1-2.729.476 7.946 7.946 0 0 1-4.755-1.565C9.174 11.443 8.145 7.68 9.315 4.438z"
                        class="fill-white"
                      ></path>
                    </svg>
                  </label>
                </div>
              </li>
              <li class="group">
                <a
                  href="#home"
                  class="
                    text-base text-white
                    py-2
                    mx-8
                    flex
                    group-hover:text-primary
                    dark:text-white
                  "
                  >FAQS</a
                >
              </li>
              <li class="group">
                <NuxtLink
                  to="/login"
                  class="
                    text-base text-white
                    py-2
                    mx-8
                    flex
                    group-hover:scale-110 group-hover:shadow-primary
                    transition
                    duration-300
                    dark:text-white
                    bg-primary
                    btnLogin
                    tracking-wide
                  "
                  >LOGIN</NuxtLink
                >
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
  </header>

  <!-- Navbar End -->
</template>

<script>
</script>

<style>
.hamburger-line {
  @apply w-[30px] h-[2px] my-2 block bg-white dark:bg-white;
}

.hamburger-active > span:nth-child(1) {
  @apply rotate-45 translate-x-1;
}
.hamburger-active > span:nth-child(2) {
  @apply scale-0 translate-x-1;
}
.hamburger-active > span:nth-child(3) {
  @apply -rotate-45 translate-x-1;
}
</style>
