<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">

	<main>
		<slot />
	</main>
	
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
