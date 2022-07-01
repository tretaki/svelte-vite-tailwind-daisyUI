<script>
  let count = 0;
  const increment = () => {
    count += 1;
  };
</script>

<div class="flex space-x-2 justify-center m-4">
  <button on:click={increment} type="button" class="btn btn-primary"
    >Clicks: {count}
  </button>
</div>
