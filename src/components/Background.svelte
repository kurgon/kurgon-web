<script lang="ts">
</script>

<div class="gradient" />

<style lang="scss" scoped>
  .gradient::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    z-index: -2;
    height: 100%;
    width: 100%;
    background-image: linear-gradient(to bottom left, #5b2a86, #000010 40%);
  }

  .gradient::after {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #000010;
    animation: bg-anim ease-in-out infinite 3s;
    z-index: -1;
  }

  @keyframes bg-anim {
    from,
    to {
      opacity: 0;
    }
    50% {
      opacity: 0.5;
    }
  }
</style>
