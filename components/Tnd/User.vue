<template>
  <div>
    <section>
      <div
        class="
          bg-blue-600
          h-52
          sm:h-[400px]
          bg-[url('/background-slider.jpg')] bg-cover bg-no-repeat bg-center
        "
      ></div>
    </section>
    <section class="-mt-20 px-6">
      <div class="max-w-screen-lg mx-auto">
        <img
          src="/background-slider.jpg"
          class="w-[150px] h-[150px] rounded-2xl border-4 mx-auto"
          alt=""
        />
        <div class="text-center">
          <h3 class="text-blue-600 text-2xl pt-2 font-extrabold md:text-4xl">
            Nama Peserta
          </h3>

          <p class="">jabatan karyawan</p>
          <div
            class="
              inline-flex
              justify-between
              items-center
              py-1
              px-1
              text-sm text-gray-700
              bg-white
              rounded-full
            "
            role="alert"
          >
            <span class="text-sm font-medium px-2">0021321</span>
          </div>
          <garis />
        </div>
        <div
          class="
            mb-8
            flex
            items-center
            rounded-xl
            bg-white
            text-center
            mx-auto
            max-w-screen-sm
          "
        >
          <a
            href="#"
            class="
              w-full
              rounded-l-xl
              py-4
              hover:shadow-md
              dark:border-jacarta-600
            "
          >
            <div class="mb-1 font-bold text-2xl">7.2K</div>
            <div class="text-2xs font-medium tracking-tight -mt-2">Items</div>
          </a>
          <a
            href="#"
            class="
              w-full
              py-4
              hover:shadow-md
              dark:border-jacarta-600
              border-r border-l
            "
          >
            <div class="mb-1 font-bold text-2xl">5.3K</div>
            <div class="text-2xs font-medium tracking-tight -mt-2">Owners</div>
          </a>
          <a
            href="#"
            class="w-full bo py-4 hover:shadow-md dark:border-jacarta-600"
          >
            <div
              class="
                mb-1
                flex
                items-center
                justify-center
                text-base
                font-medium
              "
            >
              <span class="mb-1 font-bold text-2xl">2.55</span>
            </div>
            <div class="text-2xs font-medium tracking-tight -mt-2">
              Floor Price
            </div>
          </a>
        </div>
        <div class="flex mt-5 w-full overflow-x-auto">
          <div class="flex py-12">
            <div
              class="
                w-72
               
                snap-center
                block
                rounded-2xl
                border border-jacarta-100
                bg-white
                p-2
                text-gray-600
                hover:text-blue-600
                transition-shadow
                hover:shadow-lg
              "
            >
              <figure class="relative">
                <a href="item.html">
                  <img
                    src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
                    alt="item 5"
                    class="h-64 rounded-[0.625rem]"
                    loading="lazy"
                  />
                </a>
                <div
                  class="
                    absolute
                    top-3
                    right-3
                    flex
                    items-center
                    space-x-1
                    rounded-md
                    bg-white
                    p-2
                  "
                >
                  <span class="text-sm ">Operation</span>
                </div>
                <div class="absolute left-3  -bottom-3 ">
                  <div class="flex items-center px-3 py-1 rounded-full bg-blue-600 text-white ">
                     <Icon name="solar:call-chat-rounded-bold-duotone" class="w-4 h-4 mr-2 text-white" /> 120 
                  </div>
                </div>
              </figure>
              <div class="p-2">
                <div class="mt-4 flex items-center justify-between">
                  <h4 href="item.html">
                    <span class="font-bold capitalize"
                      >sosialisai cara pembayaran cabang</span
                    >
                  </h4>
                </div>
                <div
                  class="
                    mt-2
                    flex flex-wrap
                   space-y-1
                    w-full
                   
                    text-xs text-gray-900
                  "
                >
                  <div
                    class="
                      flex mr-1
                      items-center
                      bg-gray-100
                      w-max
                      p-2
                      rounded
                      opacity-50
                      hover:opacity-100 hover:fill-blue-600 hover:text-blue-600
                    "
                  >
                   <Icon name="solar:call-chat-rounded-bold-duotone" class="w-4 h-4" />
                    <span class="ml-1">14 Jan</span>
                  </div>
                  <div
                    class="
                      flex mr-1
                      items-center
                      bg-gray-100
                      w-max
                      p-2
                      rounded
                      opacity-50
                      hover:opacity-100 hover:fill-blue-600 hover:text-blue-600
                    "
                  >
                    <Icon name="solar:call-chat-rounded-bold-duotone" class="w-4 h-4" />
                    <span class="ml-1">Zoom</span>
                  </div>
                  <div
                    class="
                      flex mr-1
                      items-center
                      bg-gray-100
                      w-max
                      p-2
                      rounded
                      opacity-50
                      hover:opacity-100 hover:fill-blue-600 hover:text-blue-600
                    "
                  >
                    <Icon name="solar:call-chat-rounded-bold-duotone" class="w-4 h-4" />
                    <span class="ml-1">Wajib</span>
                  </div>
                   <div
                    class="
                      flex
                      items-center
                      bg-gray-100
                      w-max
                      p-2
                      rounded
                      opacity-50
                      hover:opacity-100 hover:fill-blue-600 hover:text-blue-600
                    "
                  >
                    <Icon name="solar:call-chat-rounded-bold-duotone" class="w-4 h-4" />
                    <span class="ml-1">Wajib</span>
                  </div>
                </div>

                <div class="mt-8 flex items-bottom justify-between">
                  <p>
                    <sub>Mulai dari </sub><br />
                    <span class="text-lg font-bold text-blue-600"
                      >Rp. 20.000.000</span
                    >
                    <span class="text-xs"> /bulan</span>
                  </p>
                  <p>
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="24"
                      height="24"
                      class="mt-6"
                      viewBox="0 0 24 24"
                    >
                      <path
                        fill="#888888"
                        d="M20.16 5A6.29 6.29 0 0 0 12 4.36a6.27 6.27 0 0 0-8.16 9.48l6.21 6.22a2.78 2.78 0 0 0 3.9 0l6.21-6.22a6.27 6.27 0 0 0 0-8.84Zm-1.41 7.46l-6.21 6.21a.76.76 0 0 1-1.08 0l-6.21-6.24a4.29 4.29 0 0 1 0-6a4.27 4.27 0 0 1 6 0a1 1 0 0 0 1.42 0a4.27 4.27 0 0 1 6 0a4.29 4.29 0 0 1 .08 6Z"
                      />
                    </svg>
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <TabGroup>
          <TabList class="flex space-x-1 rounded-xl p-1">
            <Tab
              v-for="category in Object.keys(categories)"
              as="template"
              :key="category"
              v-slot="{ selected }"
            >
              <button
                :class="[
                  'w-full rounded-lg py-2.5 text-sm font-medium leading-5 text-gray-600',
                  'ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
                  selected
                    ? 'bg-blue-600 shadow text-white'
                    : 'text-blue-100 hover:bg-white/[0.12] hover:text-blue-600',
                ]"
              >
                {{ category }}
              </button>
            </Tab>
          </TabList>

          <TabPanels class="mt-2">
            <TabPanel
              v-for="(posts, idx) in Object.values(categories)"
              :key="idx"
              :class="[
                'rounded-xl bg-white p-3',
                'ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
              ]"
            >
              <ul>
                <li
                  v-for="post in posts"
                  :key="post.id"
                  class="relative rounded-md p-3 hover:bg-gray-100"
                >
                  <h3 class="text-sm font-medium leading-5">
                    {{ post.title }}
                  </h3>

                  <ul
                    class="
                      mt-1
                      flex
                      space-x-1
                      text-xs
                      font-normal
                      leading-4
                      text-gray-500
                    "
                  >
                    <li>{{ post.date }}</li>
                    <li>&middot;</li>
                    <li>{{ post.commentCount }} comments</li>
                    <li>&middot;</li>
                    <li>{{ post.shareCount }} shares</li>
                  </ul>

                  <a
                    href="#"
                    :class="[
                      'absolute inset-0 rounded-md',
                      'ring-blue-400 focus:z-10 focus:outline-none focus:ring-2',
                    ]"
                  />
                </li>
              </ul>
            </TabPanel>
          </TabPanels>
        </TabGroup>
      </div>
    </section>
  </div>
</template>
<script setup>
import { ref } from 'vue';
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue';

const categories = ref({
  Training: [
    {
      id: 1,
      title: 'Does drinking coffee make you smarter?',
      date: '5h ago',
      commentCount: 5,
      shareCount: 2,
    },
  ],
  Progress: [
    {
      id: 1,
      title: 'Is tech making coffee better or worse?',
      date: 'Jan 7',
      commentCount: 29,
      shareCount: 16,
    },
    {
      id: 2,
      title: 'Ask Me Anything: 10 answers to your questions about coffee',
      date: '2d ago',
      commentCount: 9,
      shareCount: 5,
    },
    {
      id: 1,
      title: 'Ask Me Anything: 10 answers to your questions about coffee',
      date: '2d ago',
      commentCount: 9,
      shareCount: 5,
    },
  ],
  Selesai: [
    {
      id: 1,
      title: 'Ask Me Anything: 10 answers to your questions about coffee',
      date: '2d ago',
      commentCount: 9,
      shareCount: 5,
    },
  ],
});
</script>
