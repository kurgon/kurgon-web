<script>
  import GithubIcon from "../components/GithubIcon.svelte";
</script>

<main>
  <header>
    Welcome to 
    <a class="repo" href="//github.com/kurgon/web" target="_blank">
      <GithubIcon />
      kurgon/web
    </a>
  </header>
  <hr />
  <h2>Programmer ∙ Cybersecurity enthusiast ∙ Open source</h2>
  <div class="Socials">
    <a href="//github.com/kurgon" target="_blank">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        width="24"
        height="24"
        class="main-grid-item-icon"
        fill="none"
        stroke="currentColor"
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
      >
        <path
          d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"
        />
      </svg>
    </a>
    <a href="#" style="color: #ef798a">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        width="24"
        height="24"
        class="main-grid-item-icon"
        fill="none"
        stroke="currentColor"
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
      >
        <path
          d="M22.54 6.42a2.78 2.78 0 0 0-1.94-2C18.88 4 12 4 12 4s-6.88 0-8.6.46a2.78 2.78 0 0 0-1.94 2A29 29 0 0 0 1 11.75a29 29 0 0 0 .46 5.33A2.78 2.78 0 0 0 3.4 19c1.72.46 8.6.46 8.6.46s6.88 0 8.6-.46a2.78 2.78 0 0 0 1.94-2 29 29 0 0 0 .46-5.25 29 29 0 0 0-.46-5.33z"
        />
        <polygon points="9.75 15.02 15.5 11.75 9.75 8.48 9.75 15.02" />
      </svg>
    </a>
  </div>
</main>

<style scoped lang="scss">
  main {
    display: flex;
    width: 70%;
    height: 70%;
    margin-top: auto;
    margin-right: auto;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-end;
    padding: 2rem;
    header {
      display: flex;
      flex-direction: row;
      font-size: 5.5rem;
      font-family: "Inter", sans-serif;
      font-weight: 800;
      width: 100%;
      a.repo {
        display: flex;
        flex-direction: row;
        text-decoration: inherit;
        color: inherit;
        margin: 0;
        border-radius: 15px;
        background-color: #ffffff20;
        transition: background 0.1s;
        gap: 1rem;
        padding-inline: 1rem;
        svg {
          height: 5rem;
          margin: auto;
          //background-image: url("../assets/github.svg");
          //background-size: 60%;
          // background-position: center center;
          //  background-repeat: no-repeat;
        }
      }
      a.repo:hover {
        background-color: #ffffff30;
      }
    }
    hr {
      width: 100%;
      margin-block: 1rem;
    }
    h2 {
      font-weight: 300;
    }
    .Socials {
      display: flex;
      flex-direction: row;
      gap: 1rem;
      width: 100%;
      height: 5rem;
      a {
        color: inherit;
      }
    }
  }
</style>
