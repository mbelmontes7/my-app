<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<p>By- <a href="https://magalybelmontes77.notion.site/Magaly-s-creativity-home-8a88ba5e947f44ffb5d35acebf64f678">Magaly Belmontes 🖤</a>
		
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		color: rgb(13, 1, 25);
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
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

	footer a {
		font-weight: bold;
		color: rgb(43, 8, 104);
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
