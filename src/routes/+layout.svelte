<script>
  // import "@skeletonlabs/skeleton/themes/theme-skeleton.css";
  import "../qv_theme.postcss";
  import "@skeletonlabs/skeleton/styles/all.css";
  import "../app.postcss";
  import { AppShell, AppBar } from "@skeletonlabs/skeleton";
</script>

<!-- App Shell -->
<AppShell>
  <svelte:fragment slot="header">
    <!-- App Bar -->
    <AppBar background="bg-surface-100-800-token">
      <strong class="text-xl ">Whats Next?</strong>
    </AppBar>
  </svelte:fragment>
  <!-- Page Route Content -->
  <slot />
</AppShell>
