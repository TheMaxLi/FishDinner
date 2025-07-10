<script lang="ts">
	import '../app.css';

	let { children } = $props();
</script>

<div class="flex w-full justify-center">
	{@render children()}
</div>
