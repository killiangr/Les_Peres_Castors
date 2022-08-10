<script>
	import Header from '../lib/Header.svelte';
	import Niveau from '../lib/Niveau.svelte';
	import Formation from '../lib/Formation.svelte';
	let visible = true
	function onVisible(){
		visible=!visible;
		console.log(visible);
	}
</script>

<head>
	<title>LPC Quizz</title>
</head>

<Header />
<section class="text-gray-600 body-font">
	<div class="container px-5 pt-20 pb-10 mx-auto">
		<div class="flex flex-col text-center w-full mb-10">
			<h1 class="uppercase sm:text-3xl text-2xl font-medium title-font mb-4 text-gray-900">
				Quizzs en pagailles !
			</h1>
			<p class="lg:w-2/3 mx-auto leading-relaxed text-base">
				Selectionnez un quizz pour avoir accès à son contenu. Regardez, téléchargez, likez !
			</p>
		</div>
		<div class="flex justify-center elative mb-10">
			<input
				class="w-1/4 border-solid border-2 ring-offset-0 border-gray-500 placeholder-gray-500 rounded-md focus:placeholder-gray-500"
				placeholder="Rechercher un quizz"
			/>
		</div>
		<div class="flex flex-col text-center w-full mb-5">
			<h3 class="text-xl text-base font-semibold tracking-wide no-underline mb-5">
				Veuillez saisir un niveau d'étude
			</h3>
			<div class="flex flex-wrap -m-4" >
				<Niveau href="#L1" id="l1" src="https://1fichier.com/?fd04rvgyd610hwzwlvnm"/>
				<Niveau href="#L2" id="l2" src="https://1fichier.com/?fewgwxa6nb9v8rz10o8r"/>
				<Niveau href="#L3" id="l3" src="https://1fichier.com/?okkolyzfsi8a1slavxhh"/>
				<Niveau href="#M1" id="m1" src="https://1fichier.com/?ya6g1b6s791eyk4z9ow4"/>
				<Niveau href="#M2" id="m2" src="https://1fichier.com/?yl87lxbnsaal9oe2wnjf"/>
			</div>
		</div>
	</div>
	{#if visible}
		<div class="container px-5 pt-5 pb-10 mx-auto" >
			<div class="flex flex-col text-center w-full mb-20">
				<h3 class="text-xl text-base font-semibold tracking-wide no-underline mb-5">
					Veuillez saisir un module
				</h3>
				<div class="flex flex-wrap -m-4">
					<Formation id="biologie" src="https://1fichier.com/?uq3cqu6js481g2rzxbbn" href="biologie"/>
					<Formation id="general" src="https://1fichier.com/?742iwwj2b4lkkplqk4k3" href="formationgen"/>
					<Formation id="informatique" src="https://1fichier.com/?z7uqpa516rzhyuvee8gw" href="informatique"/>
					<Formation id="maths" src="https://1fichier.com/?qppjwfejucgylpe4x5xm" href="maths"/>
					<Formation id="physique" src="https://1fichier.com/?p2zfs6psb1rwhjdygqzl" href="physique"/>
				</div>
			</div>
		</div>
	{/if}
</section>
