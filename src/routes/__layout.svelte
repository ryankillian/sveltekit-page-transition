<script context="module">
	export const load = async ({ url }) => {
		return {
			props: {
				key: url.pathname
			}
		};
	};
</script>

<script>
	import Nav from '../components/Nav.svelte';
	import PageTransitions from '../components/PageTransitions.svelte';
	export let key;
</script>

<Nav segment={key} />

<PageTransitions refresh={key}>
	<slot />
</PageTransitions>
