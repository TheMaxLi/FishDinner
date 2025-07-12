<script lang="ts">
	import '../app.css';

	let { children } = $props();
</script>

<div class="flex w-full justify-center bg-gradient-to-b from-white to-blue-300">
	{@render children()}
</div>
