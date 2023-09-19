<script lang="ts">
	import { onMount } from 'svelte';
	import qrcode from 'qrcode';

	export let qrCode: string | number;

	let qrCodeCanvas: HTMLCanvasElement;

	onMount(() => {
		qrcode.toCanvas(qrCodeCanvas, qrCode);
	});
</script>

<div class="flex flex-col">
	<p class="text-center">{qrCode}</p>
	<div class="flex justify-center">
		<canvas bind:this={qrCodeCanvas} width="300" height="300" />
	</div>
</div>
