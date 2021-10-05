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
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: blue;
		text-transform: uppercase;
		font-size: 6em;
		font-weight: 150;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>