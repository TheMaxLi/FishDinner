<script lang="ts">
	import Drinks from './Drinks.svelte';
	import Pizza from './Pizza.svelte';
	import Sandwiches from './Sandwiches.svelte';

	let selectedMenuItem = $state<'pizza' | 'drinks' | 'sandwiches'>('pizza');
</script>

<div class="px-4 mb-8" id="menu">
	<div class="relative mb-12">
		<img src="/MenuHeader.svg" alt="Menu Header STAR" />
		<button
			onclick={() => (selectedMenuItem = 'pizza')}
			class="text-center text-cyan-900 text-xl font-normal cursor-pointer
			absolute top-50 left-10
			{selectedMenuItem === 'pizza' ? 'underline' : ''}"
		>
			pizza
		</button>
		<button
			onclick={() => (selectedMenuItem = 'drinks')}
			class="text-center text-cyan-900 text-xl font-normal cursor-pointer
			absolute right-12 top-[125px]
			{selectedMenuItem === 'drinks' ? 'underline' : ''}"
		>
			drinks
		</button>
		<button
			onclick={() => (selectedMenuItem = 'sandwiches')}
			class="text-center text-cyan-900 text-xl font-normal cursor-pointer
			absolute right-16 bottom-8
			{selectedMenuItem === 'sandwiches' ? 'underline' : ''}"
		>
			sandwiches
		</button>
	</div>

	{#if selectedMenuItem === 'pizza'}
		<Pizza />
	{:else if selectedMenuItem === 'drinks'}
		<Drinks />
	{:else if selectedMenuItem === 'sandwiches'}
		<Sandwiches />
	{/if}
</div>
