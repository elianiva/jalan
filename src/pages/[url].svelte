<script>
  export let currentRoute;
</script>

<h1>
  Dynamic Path: <code>{decodeURIComponent(currentRoute.namedParams.url)}</code>
</h1>
