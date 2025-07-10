<script lang="ts">
	function smoothScroll(event: MouseEvent) {
		event.preventDefault();
		const targetId = (event.currentTarget as HTMLAnchorElement).getAttribute('href')?.slice(1);
		const target = document.getElementById(targetId!);
		if (target) {
			target.scrollIntoView({ behavior: 'smooth' });
		}
	}
</script>

<div class="relative w-full">
	<img src="/NavigationStar.svg" alt="" />

	<a
		href="#menu"
		class="w-16 h-8 left-[220px] top-[275px] absolute text-right justify-start text-cyan-900 text-xl font-normal font-['New_Spirit']"
		onclick={smoothScroll}
	>
		menu
	</a>
	<a
		href="#info"
		class="w-16 h-8 left-[150px] top-[370px] absolute text-right justify-start text-cyan-900 text-xl font-normal font-['New_Spirit']"
		onclick={smoothScroll}
	>
		info
	</a>
	<a
		href="#faq"
		class="w-16 h-8 left-[150px] top-[480px] absolute text-right justify-start text-cyan-900 text-xl font-normal font-['New_Spirit']"
		onclick={smoothScroll}
	>
		faq
	</a>
</div>
