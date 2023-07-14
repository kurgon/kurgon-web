<script lang="ts">
  import "../app.scss";
  import Navbar from "../components/Navbar.svelte";
  import "nprogress/nprogress.css";
  import "../nprogress.scss";
  import NProgress from "nprogress";
  import { navigating } from "$app/stores";
  import Background from "../components/Background.svelte";

  NProgress.configure({
    minimum: 0.16,
    trickle: true,
  });

  $: {
    if ($navigating) {
      NProgress.start();
    } else NProgress.done();
  }
</script>

<Background />
<Navbar />
<slot />

<style lang="scss" scoped>
</style>
