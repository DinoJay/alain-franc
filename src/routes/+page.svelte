<script>
	import { onMount } from 'svelte';
	import ImgFlip from '../lib/ImgFlip.svelte';

	let pr;
	onMount(() => {
		pr = Promise.all(
			Array.from(document.images)
				.filter((img) => !img.complete)
				.map(
					(img) =>
						new Promise((resolve) => {
							img.onload = img.onerror = resolve;
						})
				)
		).then(() => {
			console.log('images finished loading');
		});
	});
</script>

{#await pr}
	<div>...</div>
{:then _}
	<ImgFlip />
{/await}
