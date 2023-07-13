<script lang="ts">
  import { page } from "$app/stores";
</script>

<nav>
  <ul>
    <a href="/" class:active={$page.url.pathname === "/"} title="Kurgon">
      <div class="pfp" />
    </a>
    <li>
      <a
        class:active={$page.url.pathname.startsWith("/Projects")}
        href="/Projects/">Projects</a
      >
    </li>
    <li>
      <a class:active={$page.url.pathname.startsWith("/Work")} href="/Work/"
        >Work</a
      >
    </li>
    <li>
      <a
        class:active={$page.url.pathname.startsWith("/Contact")}
        href="/Contact/">Contact</a
      >
    </li>
  </ul>
</nav>

<style scoped lang="scss">
  nav {
    display: flex;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 4rem;
    ul {
      display: flex;
      flex-direction: row;
      justify-content: flex-end;
      align-items: center;
      height: 100%;
      width: 100%;
      list-style-type: none;
      margin: 1rem;
      padding: 0;
      font-size: 1.25rem;
      a[title="Kurgon"] {
        margin-right: auto;
        background-image: url("../assets/Valknut.svg");
        background-size: 75%;
        background-position: center center;
        background-repeat: no-repeat;
        border-radius: 50%;
        height: 100%;
        aspect-ratio: 1/1;
      }
      a[title="Kurgon"].active {
        // outline: solid 2px #edeff4cc;
      }
      a {
        height: 100%;
      }

      li {
        display: flex;
        margin-inline: 1rem;
        a {
          padding: 0.8rem;
          padding-block: 0.5rem;
          border-radius: 3px;
          display: flex;
          align-items: center;
          justify-content: center;
          height: 100%;
          width: 100%;
          color: inherit;
          transition: background 0.3s;
        }
        a.active,
        a:hover {
          background-color: #d8dee950;
        }
        a.active {
          text-decoration: none;
        }
      }
    }
  }
</style>
