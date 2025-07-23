<script lang="ts">
	import './app.css';
	import svelteLogo from './assets/svelte.svg';
	import viteLogo from './assets/vite.svg';
</script>

<main>
	<div class="flex justify-center">
		<a href="https://vite.dev" target="_blank" rel="noreferrer">
			<img src={viteLogo} class="logo" alt="Vite Logo" />
		</a>
		<a href="https://svelte.dev" target="_blank" rel="noreferrer">
			<img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
		</a>
		<a href="/" target="_blank" rel="noreferrer">
			<img src="/images/icon-256.png" class="logo" alt="SE EcoStruxture Logo" />
		</a>
	</div>

	<h1 class="m-4">Vite + Svelte + EcoStruxture</h1>

	<p class="m-2 mt-10">
		{#await client.getUserSettings()}
			Welcome ____
		{:then userSetting}
			Welcome {userSetting.userName}
		{/await}
	</p>

	<p class="m-2">
		Version {client.Version}
	</p>

	<p class="m-2">
		{#await client.getObjectPath()}
			Server ____
		{:then path}
			Server {path.split('/')[1]}
		{/await}
	</p>
</main>

<style>
	.logo {
		height: 6em;
		padding: 1.5em;
		will-change: filter;
		transition: filter 300ms;
	}
	.logo:hover {
		filter: drop-shadow(0 0 2em #646cffaa);
	}
	.logo.svelte:hover {
		filter: drop-shadow(0 0 2em #ff3e00aa);
	}
</style>
