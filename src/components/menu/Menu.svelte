<script lang="ts">
	import Drinks from './Drinks.svelte';
	import Pizza from './Pizza.svelte';
	import Sandwiches from './Sandwiches.svelte';

	let selectedMenuItem = $state<'pizza' | 'drinks' | 'sandwiches'>('pizza');
</script>

<div class="px-4 mb-8 flex items-center justify-center flex-col w-full" id="menu">
	<div class="relative mb-12 flex items-center justify-center max-w-[500px] w-full">
		<img src="/MenuHeader.svg" alt="Menu Header STAR" class="w-full" />
		<button
			onclick={() => (selectedMenuItem = 'pizza')}
			class="text-center text-cyan-900 text-xl font-normal cursor-pointer
			absolute top-[300px] left-14
			{selectedMenuItem === 'pizza' ? 'underline' : ''}"
		>
			pizza
		</button>
		<button
			onclick={() => (selectedMenuItem = 'drinks')}
			class="text-center text-cyan-900 text-xl font-normal cursor-pointer
			absolute right-12 top-[175px]
			{selectedMenuItem === 'drinks' ? 'underline' : ''}"
		>
			drinks
		</button>
		<button
			onclick={() => (selectedMenuItem = 'sandwiches')}
			class="text-center text-cyan-900 text-xl font-normal cursor-pointer
			absolute right-24 bottom-12
			{selectedMenuItem === 'sandwiches' ? 'underline' : ''}"
		>
			sandwiches
		</button>
	</div>
	<div class="w-full flex flex-col">
		{#if selectedMenuItem === 'pizza'}
			<Pizza />
		{:else if selectedMenuItem === 'drinks'}
			<Drinks />
		{:else if selectedMenuItem === 'sandwiches'}
			<Sandwiches />
		{/if}
	</div>
</div>
