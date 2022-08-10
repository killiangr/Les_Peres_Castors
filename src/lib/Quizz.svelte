<script>
	export let title = 'Titre';
	export let title_quizz;
	export let description;
</script>

<a href="quizzquestions">
	<div class="lg:w-1/3 sm:w-1/2 p-4">
		<div class="flex relative">
			<h1 class="absolute inset-0 w-full h-full object-cover object-center title-font visible font-medium text-3xl text-gray-1000">{title}</h1>
			<div
				class="px-8 py-10 relative z-1 w-full border-4 border-gray-200 bg-white opacity-0 hover:opacity-100"
			>
				<h1 class="title-font text-lg font-medium text-gray-900 mb-3">
					{title_quizz}
				</h1>
				<p class="leading-relaxed">
					{description}
				</p>
			</div>
		</div>
	</div>
</a>