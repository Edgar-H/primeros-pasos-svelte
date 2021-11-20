<script>
  export let algoD
</script>

<main>
  <p >Algo desde algo</p>
  <ul>
	{#each algoD as item}
		<li>{item.title}</li>
	{/each}
</ul>
</main>

<style>
  p{
    font-size:30px;
    font-weight:600
  }
  ul{
    list-style: none;
  }
</style>