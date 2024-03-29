<template>
  <v-footer height="40" app>
    <div
      class="text-caption text-disabled"
      style="position: absolute; right: 16px;"
    >
      &copy; 2024 <span class="d-none d-sm-inline-block">Julio Loarte</span>
      —
      <a
        class="text-decoration-none on-surface"
        href="https://julioloarte.com"
        rel="noopener noreferrer"
        target="_blank"
      >
        www.julioloarte.com
      </a>
    </div>
  </v-footer>
</template>

<script setup>
  
</script>

<style scoped lang="sass">
  .social-link :deep(.v-icon)
    color: rgba(var(--v-theme-on-background), var(--v-disabled-opacity))
    text-decoration: none
    transition: .2s ease-in-out

    &:hover
      color: rgba(25, 118, 210, 1)
</style>
