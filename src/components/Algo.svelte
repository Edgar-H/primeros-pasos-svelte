<script>
  export let algoD
  let level = 'low'
  const url = "https://www.youtube.com/watch?v=OTfUE2dY5JU"
  const cambiarLevel = () => {
    level = 'strong'
  }
</script>

<main>
  <p >Algo desde algo</p>
  <ul>
	{#each algoD as item}
		<li>{item.title}</li>
	{/each}
</ul>
{#if level === 'strong'}
  <p>Esto fue el resultado <a href={url}><span>click</span></a></p>
{/if}
<button on:click={cambiarLevel}>Cambiar</button>
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