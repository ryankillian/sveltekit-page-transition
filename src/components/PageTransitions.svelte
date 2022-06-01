<script>
	import { fly } from 'svelte/transition';
	export let refresh = '';
</script>

{#key refresh}
	<div in:fly={{ y: -50, duration: 1250, delay: 1300 }} out:fly={{ y: -50, duration: 1250 }}>
		<slot />
	</div>
{/key}
