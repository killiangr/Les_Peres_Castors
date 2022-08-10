<script>
	import NavPanel from '../lib/NavPanel.svelte';
	let openMenu = false;
	import Inscription from '../lib/Inscription.svelte';
	let showModal = false;
	let toggleModal = () => {
		showModal = !showModal;
	};
</script>

<Inscription {showModal} on:click={toggleModal}/>
	

<div class="z-10 relative bg-white">
	<div class="max-w-full border-b-2 mx-auto p-5 sm:p-5">
		<div class="flex justify-between items-center md:justify-start md:space-x-10">
			<div class="flex-1 flex justify-center md:flex-initial">
				<a class="flex w-20 title-font font-medium items-center text-gray-900 md:mb-0" href=".">
					<img
						class="w-5/6 object-cover object-center rounded"
						alt="mascotte"
						src="https://team-rcv.xyz/lpc/castorhead.png"
					/>
					<span class="flex ml-3 text-xl">LPC</span>
				</a>
			</div>
			<div class="-mr-2 -my-2 md:hidden">
				<button
					type="button"
					class="bg-white rounded-md p-2 inline-flex items-center justify-center text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500"
					class:openMenu
					on:click={() => (openMenu = !openMenu)}
					aria-expanded="false"
				>
					<span class="sr-only">Open menu</span>
					<!-- Heroicon name: outline/menu -->
					<svg
						class="h-6 w-6"
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke="currentColor"
						aria-hidden="true"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M4 6h16M4 12h16M4 18h16"
						/>
					</svg>
				</button>
			</div>
			<nav class="hidden md:flex space-x-10 pl-5 border-gray-100 py-2 border-l-2 border-gray-400">
				<div class="relative space-x-3">
					<a href="quizz" class="text-base font-medium text-gray-500 hover:text-gray-900">
						Quizz
					</a>
					<a href="fiches" class="text-base font-medium text-gray-500 hover:text-gray-900">
						Fiches
					</a>
					<a href="annales" class="text-base font-medium text-gray-500 hover:text-gray-900">
						Annales
					</a>
					<a href="forum" class="text-base font-medium text-gray-500 hover:text-gray-900">
						Forum
					</a>
					<a href="contact" class="text-base font-medium text-gray-500 hover:text-gray-900">
						Contact
					</a>
				</div>
			</nav>
			<div class="hidden md:flex items-center justify-end md:flex-1 lg:w-0">
				<!--<button
					class="inline-flex items-center bg-gray-100 border-0 py-1 px-3 focus:outline-none hover:bg-gray-200 rounded text-base mt-4 md:mt-0 mr-1"
					on:click={toggleModal}
					>Inscription
					<svg
						fill="none"
						stroke="currentColor"
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						class="w-4 h-4 ml-1"
						viewBox="0 0 24 24"
					>
						<path d="M5 12h14M12 5l7 7-7 7" />
					</svg>
				</button>
				<button
					class="inline-flex items-center bg-gray-100 border-0 py-1 px-3 focus:outline-none hover:bg-gray-200 rounded text-base mt-4 md:mt-0"
					>Connexion
					<svg
						fill="none"
						stroke="currentColor"
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						class="w-4 h-4 ml-1"
						viewBox="0 0 24 24"
					>
						<path d="M5 12h14M12 5l7 7-7 7" />
					</svg>
				</button>-->
				<nav class="inline-flex items-center bg-gray-100 border-0 py-1 px-3 focus:outline-none hover:bg-gray-200 rounded text-base mt-4 md:mt-0 mr-1">
					<a href="profil" class="text-base font-medium text-gray-500 hover:text-gray-900">Profil</a>
				</nav>

			</div>
		</div>
	</div>
	{#if openMenu}
		<NavPanel bind:openMenu />
	{/if}

	<!--
Mobile menu, show/hide based on mobile menu state.

Entering: "duration-200 ease-out"
From: "opacity-0 scale-95"
To: "opacity-100 scale-100"
Leaving: "duration-100 ease-in"
From: "opacity-100 scale-100"
To: "opacity-0 scale-95"
-->
</div>