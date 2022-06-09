<template>
  <div class="container mx-auto my-16 sm:px-6 lg:px-8">
    <form action="" class="bg-nav rounded mx-auto px-6 py-6 w-1/2">
      <div class="flex flex-col mt-3">
        <label for="email" class="text-white text-xl">Email</label>
        <input type="email" class="px-2 py-1 rounded" placeholder="email" />
        <span class="text-red-200 italic">EMAIL</span>
      </div>

      <div class="flex flex-col mt-3">
        <label for="password" class="text-white text-xl">Password</label>
        <input
          type="password"
          class="px-2 py-1 rounded"
          placeholder="password"
        />
        <span class="text-red-200 italic">PASSWORD</span>
      </div>

      <div class="text-center mt-3">
        <lr-button type="submit"> LOGIN </lr-button>
      </div>
    </form>
    <div class="text-center">
      <p>
        belum punya akun?
        <NuxtLink to="/auth/register">Daftar!</NuxtLink>
      </p>

      <NuxtLink to="/">Halaman Utama</NuxtLink>
    </div>
  </div>
</template>
