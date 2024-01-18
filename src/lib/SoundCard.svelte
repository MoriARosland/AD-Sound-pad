<script lang="ts">
	import type { PadData } from '$lib/PadData';

	export let pad_data: PadData;

	// let audio: HTMLAudioElement;

	function playAudio() {
		const audio = new Audio('src/lib/assets/jas.m4a');
		audio.currentTime = 0.68;
		audio.play();
	}
</script>

<audio src="src/lib/assets/jas.m4a"></audio>
<div
	on:click={playAudio}
	class="border rounded border-blue-500 p-4 w-48 h-28 hover:scale-105 transition-transform"
>
	<p>{pad_data.title}</p>
</div>
