<template>
  <v-card
    :loading="loading"
    class="mx-auto my-12"
    max-width="374"
  >
    <template v-slot:loader="{ isActive }">
      <v-progress-linear
        :active="isActive"
        color="deep-purple"
        height="4"
        indeterminate
      ></v-progress-linear>
    </template>

    <v-img
      height="250"
      src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
      cover
    ></v-img>

    <v-card-item>
      <v-card-title>Movie Title</v-card-title>

      <v-card-subtitle>
        <span class="me-1">1986</span>

        <v-icon
          color="error"
          icon="mdi-fire-circle"
          size="small"
        ></v-icon>
      </v-card-subtitle>
    </v-card-item>

    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
        <v-rating
          :model-value="4.5"
          color="amber"
          density="compact"
          size="small"
          half-increments
          readonly
        ></v-rating>

        <div class="text-grey ms-4">
          4.5 (413)
        </div>
      </v-row>

      <div class="my-4">Movie Description.</div>
    </v-card-text>

    <v-divider class="mx-4 mb-1"></v-divider>

    <v-card-title>Rate the movie</v-card-title>

    <div class="px-4">
      <div class="d-flex flex-column align-center justify-center">
        <v-rating v-model="rating" class="ma-2" density="default"></v-rating>
    </div>
    </div>
  </v-card>
</template>

<script setup>
  import { ref } from 'vue'

  const loading = ref (false)
  const rating = ref(3)
</script>