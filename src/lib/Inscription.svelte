<script>
	export let showModal = false;
	export let isPromo = false;
	/* import supabase from '../lib/db.js';
	import { session } from '$app/stores'; */

	let email, password, nom, prenom, niveau;

	/* async function signUp() {
		const { user, session: sesh, error } = await supabase.auth.signUp({
			email,
			password
		});
		if (error) alert(error, message);
		console.log(user, session, error);
		$session = sesh;
	} */
</script>

<!-- {#if showModal}
	<div class="backdrop" class:promo={isPromo} on:click|self>
		<div class="modal">
			<div class="title">
				<slot name="title">
					<h3>Default Title</h3>
				</slot>
			</div>
			<slot />
		</div>
	</div>
{/if} -->

{#if showModal}
	<div class="backdrop" class:promo={isPromo} on:click|self>
		<div class="modal">
			<head>
				<title>Inscription</title>
			</head>
			<form class="overflow-auto">
				<div class="title">
					<h2 class="text-gray-900 text-lg font-medium title-font mb-5">Inscription</h2>
				</div>
				<div class="flex flex-wrap">
					<div class="relative mb-4 p-4 md:w-1/2">
						<label for="nom" class="ml-3 leading-7 text-sm text-gray-400" tablindex="0">Nom</label>
						<input
							type="text"
							id="nom"
							name="Nom"
							class="ml-1 mt-1 w-full bg-gray-600 bg-opacity-20 focus:bg-transparent focus:ring-2 focus:ring-indigo-900 rounded border border-gray-600 focus:border-indigo-500 text-base outline-none text-gray-500 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
							bind:value={nom}
						/>
					</div>
					<div class="relative mb-4 p-4 md:w-1/2">
						<label for="prénom" class="ml-3 leading-7 text-sm text-gray-400">Prénom</label>
						<input
							type="text"
							id="prénom"
							name="Prénom"
							class="ml-1 mt-1 w-full bg-gray-600 bg-opacity-20 focus:bg-transparent focus:ring-2 focus:ring-indigo-900 rounded border border-gray-600 focus:border-indigo-500 text-base outline-none text-gray-500 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
							bind:value={prenom}
						/>
					</div>
				</div>
				<div class="flex flex-wrap">
					<div class="relative mb-4 justify-center">
						<label for="niveau" class="ml-7 leading-7 text-sm text-gray-400">Niveau d'étude</label>
						<select
							id="niveau"
							class="rounded border appearance-none border-gray-300 py-2 focus:outline-none focus:ring-2 focus:ring-indigo-200 focus:border-indigo-500 text-base pl-3 pr-10"
							bind:value={niveau}
						>
							<option>L1</option>
							<option>L2</option>
							<option>L3</option>
							<option>M1</option>
							<option>M2</option>
						</select>
						<span
							class="absolute right-0 top-0 h-full w-10 text-center text-gray-600 pointer-events-none flex items-center justify-center"
						>
							<svg
								fill="none"
								stroke="currentColor"
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								class="w-4 h-4"
								viewBox="0 0 24 24"
							>
								<path d="M6 9l6 6 6-6" />
							</svg>
						</span>
					</div>
				</div>
				<div class="flex flex-wrap px-4">
					<div class="relative w-full mb-4 mt-3">
						<label for="email" class="ml-3 leading-7 text-sm text-gray-400">Email</label>
						<input
							type="email"
							id="email"
							name="email"
							autocomplete="email"
							class="ml-1 mt-1 w-full bg-gray-600 bg-opacity-20 focus:bg-transparent focus:ring-2 focus:ring-indigo-900 rounded border border-gray-600 focus:border-indigo-500 text-base outline-none text-gray-500 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
							placeholder="exemple@domaine.com"
							bind:value={email}
						/>
					</div>
				</div>
				<div class="flex flex-wrap">
					<div class="relative mb-4 p-4 md:w-1/2">
						<label for="password" class="ml-3 leading-7 text-sm text-gray-400">Mot de passe</label>
						<input
							id="password"
							name="password"
							type="password"
							autocomplete="current-password"
							required
							class="appearance-none rounded-none relative block ml-1 mt-1 w-full bg-gray-600 bg-opacity-20 focus:bg-transparent focus:ring-2 focus:ring-indigo-900 rounded border border-gray-600 focus:border-indigo-500 text-base outline-none text-gray-500 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
							placeholder="Password"
							bind:value={password}
						/>
					</div>
					<div class="relative mb-4 p-4 md:w-1/2">
						<label for="password" class="ml-3 leading-7 text-sm text-gray-400">Confirmation</label>
						<input
							id="password"
							name="password"
							type="password"
							required
							class="appearance-none rounded-none relative block ml-1 mt-1 w-full bg-gray-600 bg-opacity-20 focus:bg-transparent focus:ring-2 focus:ring-indigo-900 rounded border border-gray-600 focus:border-indigo-500 text-base outline-none text-gray-500 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
							bind:value={password}
							placeholder="Password"
						/>
					</div>
				</div>
				<div class="flex justify-center mb-3">
					<button
						class="text-white bg-indigo-500 border-0 py-2 px-8 focus:outline-none hover:bg-indigo-600 rounded text-lg"
						>Valider</button
					>
				</div>
			</form>
			<div class="flex justify-center">
				<p class="text-gray-900 text-base font-light mb-2">
					----------- ou bien se connecter avec -----------
				</p>
			</div>
			<div class="flex justify-center items-center space-x-2 mb-2">
				<a href="https://github.com" class="github w-8" target="_blank" rel="noopener noreferrer"
					><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"
						><path
							fill="currentColor"
							d="M12 .5C5.37.5 0 5.78 0 12.292c0 5.211 3.438 9.63 8.205 11.188.6.111.82-.254.82-.567 0-.28-.01-1.022-.015-2.005-3.338.711-4.042-1.582-4.042-1.582-.546-1.361-1.335-1.725-1.335-1.725-1.087-.731.084-.716.084-.716 1.205.082 1.838 1.215 1.838 1.215 1.07 1.803 2.809 1.282 3.495.981.108-.763.417-1.282.76-1.577-2.665-.295-5.466-1.309-5.466-5.827 0-1.287.465-2.339 1.235-3.164-.135-.298-.54-1.497.105-3.121 0 0 1.005-.316 3.3 1.209.96-.262 1.98-.392 3-.398 1.02.006 2.04.136 3 .398 2.28-1.525 3.285-1.209 3.285-1.209.645 1.624.24 2.823.12 3.121.765.825 1.23 1.877 1.23 3.164 0 4.53-2.805 5.527-5.475 5.817.42.354.81 1.077.81 2.182 0 1.578-.015 2.846-.015 3.229 0 .309.21.678.825.56C20.565 21.917 24 17.495 24 12.292 24 5.78 18.627.5 12 .5z"
						/></svg
					></a
				>
				<a
					href="https://facebook.com"
					class="facebook w-10"
					target="_blank"
					rel="noopener noreferrer"
					><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 30 30">
						<path
							d="M15,3C8.373,3,3,8.373,3,15c0,6.016,4.432,10.984,10.206,11.852V18.18h-2.969v-3.154h2.969v-2.099c0-3.475,1.693-5,4.581-5 c1.383,0,2.115,0.103,2.461,0.149v2.753h-1.97c-1.226,0-1.654,1.163-1.654,2.473v1.724h3.593L19.73,18.18h-3.106v8.697 C22.481,26.083,27,21.075,27,15C27,8.373,21.627,3,15,3z"
						/></svg
					>
				</a>
				<a
					href="https://www.google.com"
					class="google w-9"
					target="_blank"
					rel="noopener noreferrer"
					><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 50 50"
						><path
							d="M 25.996094 48 C 13.3125 48 2.992188 37.683594 2.992188 25 C 2.992188 12.316406 13.3125 2 25.996094 2 C 31.742188 2 37.242188 4.128906 41.488281 7.996094 L 42.261719 8.703125 L 34.675781 16.289063 L 33.972656 15.6875 C 31.746094 13.78125 28.914063 12.730469 25.996094 12.730469 C 19.230469 12.730469 13.722656 18.234375 13.722656 25 C 13.722656 31.765625 19.230469 37.269531 25.996094 37.269531 C 30.875 37.269531 34.730469 34.777344 36.546875 30.53125 L 24.996094 30.53125 L 24.996094 20.175781 L 47.546875 20.207031 L 47.714844 21 C 48.890625 26.582031 47.949219 34.792969 43.183594 40.667969 C 39.238281 45.53125 33.457031 48 25.996094 48 Z"
						/></svg
					>
				</a>
			</div>
			<div class="flex justify-center">
				<p class="text-gray-900 text-base font-light mb-5">
					Déjà membre ? <a href="Connexion">Connecte-toi !</a>
				</p>
			</div>
		</div>
	</div>
{/if}

<style>
	* {
		z-index: 100;
	}
	.backdrop {
		width: 100%;
		height: 100%;
		position: fixed;
		background: rgba(0, 0, 0, 0.8);
	}
	.modal {
		padding: 10px;
		border-radius: 10px;
		max-width: 600px;
		margin: 5% auto;
		text-align: left;
		background: white;
	}
	.title {
		text-align: center;
	}
	.promo .modal {
		background: crimson;
		color: white;
	}
</style>
