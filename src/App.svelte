<script lang="ts">
	export let name: string;
</script>

<main>
	<h1>MOOON {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 260px;
		margin: 0 auto;
	}

	h1 {
		color:lightblue;
		text-transform: uppercase;
		font-size: 8em;
		font-weight: 150;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>