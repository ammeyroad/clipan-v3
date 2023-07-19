<template>
  <div
    class="bg-cover bg-blue-500"
    data-overlay="0.7"
    :style="{ backgroundImage: `url(${backgroundUrl})` }"
  >
    <div class="page-title">
      <div class="container">
        <h1 class="title">{{ title }}</h1>
      </div>
    </div>
    <div class="page-breadcrumb position-static">
      <div class="container">
        <ul class="flex text-center">
          <li class="breadcrumb-item">
            <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li class="breadcrumb-item">
            <span>{{ activePageName }}</span>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['activePageName', 'title', 'backgroundUrl'],
};
</script>
