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

<div class="relative w-full flex justify-end pt-32 pb-15">
	<img src="/NavigationStar.svg" alt="" class="w-fit" />
	<a
		href="#chefs"
		class="w-16 h-8 right-[110px] top-[265px] absolute text-right justify-start text-cyan-900 text-xl font-normal font-['New_Spirit']"
		onclick={smoothScroll}
	>
		chefs
	</a>
	<a
		href="#menu"
		class="w-16 h-8 right-[190px] top-[360px] absolute text-right justify-start text-cyan-900 text-xl font-normal font-['New_Spirit']"
		onclick={smoothScroll}
	>
		menu
	</a>
	<a
		href="#info"
		class="w-16 h-8 right-[190px] top-[490px] absolute text-right justify-start text-cyan-900 text-xl font-normal font-['New_Spirit']"
		onclick={smoothScroll}
	>
		info
	</a>
	<a
		href="#faq"
		class="w-16 h-8 right-[110px] top-[590px] absolute text-right justify-start text-cyan-900 text-xl font-normal font-['New_Spirit']"
		onclick={smoothScroll}
	>
		faq
	</a>
</div>
