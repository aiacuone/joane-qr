<script lang="ts">
	import QrCode from '$lib/components/QrCode.svelte';
	import '../app.css';
</script>

<div class="flex flex-col gap-20 h-screen justify-center">
	<QrCode qrCode="x39.com/" />
	<QrCode qrCode="lifewave.com/bodyrepair" />
</div>
