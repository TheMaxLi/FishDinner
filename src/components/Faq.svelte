<script>
	const faqItems = [
		{
			question: 'will there be fish?',
			answer: 'no.\n\nseb can come in smelling like fish upon request'
		},
		{
			question: 'how do i get there?',
			answer:
				'drive there idk\n\nparking @\nEasyPark - Lot 7\nother parking options\n\ncould also transit\nskytrain to main street science world then walk or bus over!'
		},
		{
			question: "what if i don't like the food?",
			answer: 'then this might be a deeply confusing experience for you.'
		},
		{
			question: 'can i sit next to seb?',
			answer: "we'll see how much fish he smells like first."
		},
		{
			question: 'what if i want more food?',
			answer: 'look at tina directly in the eyes and whisper "round two."'
		},
		{
			question: 'how much does it cost?',
			answer:
				'whatever feels good. even vibes are accepted. but donations keep the magic going and tina and seb mildly fed.'
		}
	];
</script>

<div class="px-4 mb-8 pt-40">
	<div class="text-center text-cyan-900 text-5xl font-normal mb-8">#faq</div>

	<div class="space-y-0">
		{#each faqItems as item}
			<div class="border-t border-b border-cyan-900 py-1.5">
				<div class="text-cyan-900 text-xl font-semibold lowercase">
					➬ {item.question}
				</div>
				<div class="text-cyan-900 text-lg font-medium lowercase whitespace-pre-line">
					{item.answer}
				</div>
			</div>
		{/each}
	</div>
</div>
