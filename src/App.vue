<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <v-bottom-navigation :elevation="24" grow>
      <v-btn value="recent">
        <v-icon>mdi-history</v-icon>

        <span>Recent</span>
      </v-btn>

      <v-btn value="favorites">
        <v-icon>mdi-heart</v-icon>

        <span>Favorites</span>
      </v-btn>

      <v-btn value="nearby">
        <v-icon>mdi-map-marker</v-icon>

        <span>Nearby</span>
      </v-btn>
    </v-bottom-navigation>
    <div class="gap-5">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/catalog">Home</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
