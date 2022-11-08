<script>
  let count = 0;
  $: doubled = count * 2;

  function incrementCount() {
    count += 1;
  }
</script>

<button on:click={incrementCount}>
  Clicked {count}
  {count === 1 ? "time" : "times"}
</button>

<p>{count} doubled is {doubled}</p>
