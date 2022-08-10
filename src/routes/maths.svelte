<script>
	import Header from '../lib/Header.svelte';
	import Quizz from '../lib/Quizz.svelte';
	import supabase from '../lib/db.js';
	import { onMount } from 'svelte';
	let matieres = [];
	let quizzs = [];

	onMount(() => {
		getquizzmatieres();
		getquizzs();
	});

	async function getquizzmatieres() {
		/*let { data: quizzs, error } = */ await supabase
			.from('quizzs')
			.select('matières (*)')
			.then((res) => {
				matieres = res.data;
			});
		console.log(matieres);
	}
	async function getquizzs() {
		/*let { data: quizzs, error } = */ await supabase
			.from('quizzs')
			.select()
			.then((res) => {
				quizzs = res.data;
			});
		console.log(quizzs);
	}
</script>

<head>
	<title>LPC Quizz Maths</title>
</head>

<Header />
<div class="container px-5 pt-10 mx-auto">
	<div class="flex flex-col text-center w-full mb-20">
		<h3 class="text-xl text-base font-semibold tracking-wide no-underline mb-5">
			Les quizzs de maths
		</h3>
	</div>
	<div class="flex flex-wrap">
		{#each quizzs as q,matieres}
			<Quizz titletitle_quizz={q.nom} description={q.description}/>
		{/each}
	</div>
</div>
