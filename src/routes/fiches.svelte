<script>
	import Header from '../lib/Header.svelte';
	import { onMount } from 'svelte';
	function showDownload() {
		document.getElementById('upload').style.display = 'none';
		document.getElementById('download').style.display = 'block';
	}

	function showUpload() {
		document.getElementById('upload').style.display = 'block';
		document.getElementById('download').style.display = 'none';
	}
	onMount(() => {
		showDownload();
	});
	
</script>

<head>
	<title>LPC Fiches</title>
</head>

<Header />

<section class="text-gray-600 body-font min-h-screen">
	<div class="flex w-auto justify-center mt-5">
		<button
			class="flex inline-block font-semibold bg-blue-200 border-0 py-1 px-3 focus:outline-none hover:bg-gray-200 rounded text-base mt-4 md:mt-0 mr-1"
			id="buttonDown"
			on:click="{showDownload}"
			>Download
		</button>
		<button
			class="flex inline-block font-semibold bg-blue-200 border-0 py-1 px-3 focus:outline-none hover:bg-gray-200 rounded text-base mt-4 md:mt-0 mr-1"
			id="buttonUp"
			on:click="{showUpload}"
			>Upload
		</button>
	</div>
		
	<div class="z-10 relative bg-white mb-10" id="download">
		<div class="relative max-w-full mx-auto p-5 mt-8 -mb-5 sm:p-5">
			<div class="flex inline-block sm:flex-col justify-center">
				<div class="absolute w-full flex justify-center">
					<input
						class=" flex-shrink-0 relative flex w-1/3 items-center border-solid border-2 ring-offset-0 border-gray-500 placeholder-gray-500 rounded-sm focus:placeholder-gray-500"
						placeholder="Rechercher une fiche"
					/>
				</div>
				<div class="flex absolute inline-block justify-end w-1/6 right-0">
					<div class="flex w-auto">
						<button
							class="flex inline-flex font-semibold bg-gray-100 border-0 py-1 px-3 focus:outline-none hover:bg-gray-200 rounded text-base mt-4 md:mt-0 mr-1"
							>Info ?
						</button>
					</div>
				</div>
			</div>
		</div>
		<div class="max-w-full mx-auto p-5 sm:p-5">
			<div class="flex inline-block sm:flex-col justify-center">
				<nav class="md:flex relative space-x-5 px-5 py-2 w-2/5">
					<div
						class="flex inline-block space-x-5 justify-center w-2/5 border-gray-100 border-2 border-gray-400 py-2 px-2 rounded "
					>
						<a
							href="#"
							class="w-50 font-medium tracking-wide text-sm border-l-4 relative border-r-4 ring-offset-2 border-solid"
						>
							Nouveau
						</a>
						<a
							href="#"
							class="w-50 font-medium tracking-wide text-sm border-l-4 relative border-r-4 ring-offset-2 border-solid"
						>
							Vues
						</a>
						<a
							href="#"
							class="w-50 font-medium tracking-wide text-sm border-l-4 relative border-r-4 ring-offset-2 border-solid"
						>
							Populaire
						</a>
					</div>
					<div
						class="flex inline-block space-x-5 justify-center w-3/5 border-gray-100 border-2 border-gray-400 py-2 px-2 rounded "
					>
						<a
							href="#"
							class="w-50 font-medium tracking-wide text-sm relative border-l-4 border-r-4 ring-offset-2 border-solid"
						>
							Jour
						</a>
						<a
							href="#"
							class="w-50 font-medium tracking-wide text-sm relative border-l-4 border-r-4 ring-offset-2 border-solid"
						>
							Semaine
						</a>
						<a
							href="#"
							class="w-50 font-medium tracking-wide text-sm relative border-l-4 border-r-4 ring-offset-2 border-solid"
						>
							Mois
						</a>
						<a
							href="#"
							class="w-50 font-medium tracking-wide text-sm relative border-l-4 border-r-4 ring-offset-2 border-solid"
						>
							Toujours
						</a>
					</div>
				</nav>
				<nav class="md:flex absolute top-5 right-0 px-5 w-3/5">
					<div class="flex grid justify-center grid-cols-5 gap-2 auto-rows-auto w-auto py-5">
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							L1
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							L2
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							L3
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							M1
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							M2
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							Bio
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							Général
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							Info
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							Maths
						</a>
						<a
							href="#"
							class="w-50 rounded font-medium text-center tracking-wide text-sm relative border-2 ring-offset-2 border-solid border-black py-2"
						>
							Physique
						</a>
					</div>
				</nav>
			</div>
		</div>
		<div class="z-10 relative bg-white mt-10">
			<iframe
				class="relative min-h-screen"
				title="Gestionnaire Annales"
				width="100%"
				height="100%"
				src="https://team-rcv.xyz/lpc/fichiers/"
			/>
		</div>
	</div>
	<div class="z-10 relative bg-white min-h-screen mt-5" id="upload">
		<iframe
			class="relative min-h-screen"
			title="Drag and Drop"
			width="100%"
			height="100%"
			src="https://team-rcv.xyz/lpc/upload/"
		/>
	</div>
</section>
