<script lang="ts">
  let currentNumber = 0;
  const getRandomNumber = () => {
    const newNumber = Math.floor(Math.random() * 75) + 1;
    currentNumber = newNumber;
  };
</script>

<div class="flex flex-col items-center justify-center text-white font-mono">
  <h2 class="text-9xl">{currentNumber}</h2>
  <button
    class="border-2 border-orange-500 p-2 text-2xl hover:bg-slate-800"
    on:click={getRandomNumber}>Rand Number</button
  >
</div>
