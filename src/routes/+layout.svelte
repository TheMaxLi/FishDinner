<script lang="ts">
	import '../app.css';

	let { children } = $props();
</script>

<div class="flex w-full justify-center bg-gradient-to-b from-white to-sky-400">
	{@render children()}
</div>
