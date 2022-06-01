<script>
	export let segment;
</script>

<div>
	<a href="/" class={segment === '/' ? 'current' : ''}>Home</a>
	<a href="/about" class={segment === '/about' ? 'current' : ''}>About</a>
</div>

<style>
	a {
		text-decoration: none;
	}
	.current {
		text-decoration: underline;
	}
</style>
