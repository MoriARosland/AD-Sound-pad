<script lang="ts">
	import type { PadData } from '$lib/PadData';
	import SoundCard from '$lib/SoundCard.svelte';

	let test_pad_data: PadData = {
		title: 'this is text from a component.',
		sound_source: '/placeholder'
	};
</script>

<div class="flex flex-col items-center justify-center py-5">
	<h1 class="text-2xl">AD Sound-pad</h1>
	<p>
		Github <a href="https://github.com/NamePending99/AD-Sound-pad">repository</a>
	</p>
</div>

<div class="flex flex-col items-center mt-8">
	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
		<SoundCard pad_data={test_pad_data}></SoundCard>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<SoundCard pad_data={test_pad_data}></SoundCard>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
		<div class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform">
			<p>Place holder</p>
		</div>
	</div>
</div>
