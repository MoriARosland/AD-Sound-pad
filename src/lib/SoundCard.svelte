<script lang="ts">
	import type { PadData } from '$lib/PadData';

	export let pad_data: PadData;
</script>

<div class="border rounded border-blue-500 p-4 w-48 h-28">
	<p>{pad_data.title}</p>
</div>
