<template>
  <div class="p-2">
    <div
      class="
        group
        relative
        flex
        h-72
        sm:h-[400px]
        items-center
        px-12
        overflow-hidden
        rounded-lg
        bg-gray-100 bg-gradient-to-tr
        from-blue-400
        to-blue-600
      "
    >
      <img
        src="https://images.unsplash.com/photo-1618556450991-2f1af64e8191?auto=format&q=75&fit=crop&w=1000"
        loading="lazy"
        class="
          absolute
          inset-0
          h-full
          w-full
          object-cover object-center
          opacity-25
          transition
          duration-200
        "
      />
      <div class="relative text-white mt-24">
        <ol class="flex h-8 space-x-2">
          <li class="flex items-center">
            <a
              rel="noopener noreferrer"
              href="#"
              title="Back to homepage"
              class="hover:underline"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20"
                fill="currentColor"
                class="w-5 h-5 pr-1 dark:text-gray-400"
              >
                <path
                  d="M10.707 2.293a1 1 0 00-1.414 0l-7 7a1 1 0 001.414 1.414L4 10.414V17a1 1 0 001 1h2a1 1 0 001-1v-2a1 1 0 011-1h2a1 1 0 011 1v2a1 1 0 001 1h2a1 1 0 001-1v-6.586l.293.293a1 1 0 001.414-1.414l-7-7z"
                />
              </svg>
            </a>
          </li>
          <li class="flex items-center space-x-2">
            /
            <a
              rel="noopener noreferrer"
              href="#"
              class="flex items-center px-1 capitalize hover:underline ml-2"
              >Profile</a
            >
          </li>
          <li class="flex items-center space-x-2">/</li>
        </ol>
        <h3 class="text-black-800 text-2xl font-bold sm:text-3xl md:text-4xl">
          Tata Kelola Perusahaan
        </h3>
      </div>
    </div>
  </div>
  <ul
    class="
      w-full
      md:mx-auto md:max-w-screen-xl
      flex
      justify-between
      items-start
      mb-8
      space-x-3
      overflow-x-auto
      p-2
    "
  >
    <li class="flex w-full">
      <button class="btn-garbir py-2">sejarah</button>
      <button class="btn-garbir py-2">sejarah</button
      ><button class="btn-garbir py-2">sejarah</button>
      <button class="btn-garbir py-2">sejarah</button
      ><button class="btn-garbir py-2">sejarah</button>
      <button class="btn-garbir py-2">sejarah</button>
    </li>
  </ul>

  <section>
    <div class="text-left max-w-screen-xl mx-auto">
      <p class="font-semibold text-yellow-500 text-sm xl:text-xl">
        Profil Perusahaan
      </p>

      <h3 class="text-black-800 text-4xl font-bold md:text-4xl">
        Profile Perusahaan
      </h3>
      <garis />
    </div>
  </section>
</template>

<script lang="ts" setup>
useHead({
  title: 'aksii',
  titleTemplate: '%s - Clipan Finance Indonesia',
  meta: [{ name: 'description', content: 'Clipan Finance Indonesia' }],
});
</script>
