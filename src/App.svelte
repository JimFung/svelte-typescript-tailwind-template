<script lang="ts">
  let count = 0;

  function increment() {
    count += 1;
  }

  function decrement() {
    count -=1;
  }

  function reset() {
    count = 0;
  }
</script>

<main class='flex flex-col items-center'>
  <h1 class='text-3xl'>Your count is at {count}</h1>
  <section class='m-2'>
    <button class='border py-2 px-4 bg-green-50 m-1' on:click={increment}>increment</button>
    <button class='border py-2 px-4 bg-green-50 m-1' on:click={decrement}>decrement</button>
    <button class='border py-2 px-4 bg-green-50 m-1' on:click={reset}>reset</button>
  </section>
</main>
