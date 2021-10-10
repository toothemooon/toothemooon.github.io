<script lang="ts">
	import { text } from "svelte/internal";
	
		let firstName = 'Jimi';
		let lastName = 'Hendr';
		let beltColour = 'black';
	
		const handleClick = () => {
			beltColour = 'orange';
		}
		
		const handleInput = (e) => {
			beltColour = e.target.value;
		}
	</script>
	
	<main>
		<p>{beltColour} belt</p>
		<input type="text" bind:value={firstName}>
		<input type="text" bind:value={lastName}>
		<input type='color' bind:value={beltColour}>
	</main>
	
	<style>
		main {
			text-align: center;
			padding: 1em;
			max-width: 240px;
			margin: 0 auto;
		}
	
		h1 {
			color: lightblue;
			text-transform: uppercase;
			font-size: 4em;
			font-weight: 100;
		}
	
		@media (min-width: 640px) {
			main {
				max-width: none;
			}
		}
	</style>