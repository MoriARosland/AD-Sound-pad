<script lang="ts">
	import type { PadData } from '$lib/PadData';
	import SoundCard from '$lib/SoundCard.svelte';

	let test_pad_data: PadData = {
		title: 'yaS',
		sound_source: '/placeholder'
	};

	let padDataArray: PadData[] = Array.from({ length: 12 }, () => test_pad_data);
</script>

<div class="flex flex-col items-center justify-center py-5">
	<h1 class="text-2xl">AD Sound-pad</h1>

	<p>
		Github <a href="https://github.com/NamePending99/AD-Sound-pad">repository</a>
	</p>
</div>

<div class="flex flex-col items-center mt-8">
	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
		{#each padDataArray as cardData}
			<SoundCard pad_data={cardData} />
		{/each}
	</div>
</div>
