<script lang="ts">
  // import "@skeletonlabs/skeleton/themes/theme-skeleton.css";
  import "../qv_theme.postcss";
  import "@skeletonlabs/skeleton/styles/all.css";
  import "../app.postcss";
  import { AppShell, AppBar } from "@skeletonlabs/skeleton";
  import Nav_actions from "$lib/Nav_actions.svelte";
</script>

<!-- App Shell -->
<AppShell>
  <svelte:fragment slot="header">
    <!-- App Bar -->
    <AppBar background="bg-surface-400-500-token" border="border-token">
      <svelte:fragment slot="lead">Whats Next?</svelte:fragment>
      <svelte:fragment slot="trail">
        <a href="/about">About</a>
      </svelte:fragment>
    </AppBar>
  </svelte:fragment>

  <!-- Page Route Content -->
  <slot />

  <svelte:fragment slot="footer">Footer</svelte:fragment>
</AppShell>
