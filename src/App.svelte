<script>
  import { Router } from "svelte-router-spa";
  import routes from "virtual:generated-pages-svelte";

  let url = "";

  console.log(routes);
</script>

<nav>
  <a href="/one">Pertama</a>
  <a href="/two">Second</a>
  <a href="/three">三つ目</a>
  <a href="/four">Kepapat</a>
</nav>
<form on:submit|preventDefault={() => (window.location.href = url)}>
  <input type="text" placeholder="Type anything" bind:value={url} />
  <button>Go!</button>
</form>

<Router {routes} />

<a id="smol" href="https://github.com/aldy505/vite-plugin-pages-svelte">
  aldy505/vite-plugin-pages-svelte
</a>
