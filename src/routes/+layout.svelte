<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lora:400,700&display=swap">

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
        <p>created by <strong>Qick</strong></p> 
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		font-family: 'Lora', serif;

	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding-top: 10rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
