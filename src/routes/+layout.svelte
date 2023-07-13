<script lang="ts">
  import "../app.scss";
  import Navbar from "../components/Navbar.svelte";
  import "nprogress/nprogress.css";
  import "../nprogress.scss";
  import NProgress from "nprogress";
  import { navigating } from "$app/stores";

  NProgress.configure({
    minimum: 0.16,
  });

  $: {
    if ($navigating) {
      NProgress.start();
    } else NProgress.done();
  }
</script>

<Navbar />
<slot />

<style lang="scss" scoped>
</style>
