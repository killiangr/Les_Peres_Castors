<script>
	import Header from "../lib/Header.svelte"
</script>

<head>
	<title>LPC Forum</title>
</head>
<Header />

<div class="text-gray-600 body-font min-h-screen">
	<div class="container mx-auto">
		<div role="article" class="py-12 md:px-8">
			<div class="px-4 xl:px-0 py-10">
				<div class="flex flex-col lg:flex-row flex-wrap">
					<div class="mt-4 lg:mt-0 lg:w-3/5">
						<div>
							<h1 class="text-3xl ml-2 lg:ml-0 lg:text-4xl font-bold text-gray-900 tracking-normal lg:w-11/12">FAQ & Recherche d'aide en ligne</h1>
						</div>
					</div>
					<div class="lg:w-2/5 flex mt-10 ml-2 lg:ml-0 lg:mt-0 lg:justify-end">
						<div class="pt-2 relative text-gray-600">
							<input class="focus:ring-2 focus:ring-offset-2 focus:ring-gray-400 bg-white h-10 px-5 pr-16 rounded-lg text-sm focus:outline-none" type="search" name="search" placeholder="Rechercher..." />
							<button type="submit" class="focus:ring-2 focus:ring-offset-2 text-gray-600 focus:text-indigo-700 focus:rounded-full focus:bg-gray-100 focus:ring-indigo-700 bg-white focus:outline-none absolute right-0 top-0 mt-5 mr-4">
								<svg class="h-4 w-4 fill-current" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" id="Capa_1" x="0px" y="0px" viewBox="0 0 56.966 56.966" style="enable-background: new 0 0 56.966 56.966" xml:space="preserve" width="512px" height="512px">
                                            <path d="M55.146,51.887L41.588,37.786c3.486-4.144,5.396-9.358,5.396-14.786c0-12.682-10.318-23-23-23s-23,10.318-23,23  s10.318,23,23,23c4.761,0,9.298-1.436,13.177-4.162l13.661,14.208c0.571,0.593,1.339,0.92,2.162,0.92  c0.779,0,1.518-0.297,2.079-0.837C56.255,54.982,56.293,53.08,55.146,51.887z M23.984,6c9.374,0,17,7.626,17,17s-7.626,17-17,17  s-17-7.626-17-17S14.61,6,23.984,6z" />
                                        </svg>
							</button>
						</div>
					</div>
				</div>
			</div>
			<div class="px-6 xl:px-0">
				<div class="grid sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-3 pb-6 gap-8">
					<div role="cell" class="bg-gray-100">
						<div class="bg-white ring ring-purple-500 p-5 rounded-md relative h-full w-full">
							<!-- class="absolute inset-0 object-center object-cover h-full w-full"  -->
							<span><img class="bg-gray-200 p-2 mb-5 rounded-full" src="https://i.ibb.co/27R6nk5/home-1.png" alt="home-1" /></span>
							<h1 class="pb-4 text-2xl font-semibold">Rechercher de l'aide</h1>
							<div class="my-5">
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full space-x-3">
									<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
										<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
									</svg>
									<h4 class="text-md text-gray-900 dark:text-gray-100">Première fois sur ce site, comment ça marche?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full space-x-3">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100">Comment trouver quelque-un pour m'aider ?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Je n'ai reçu aucune réponse à mes questions, que dois-je faire ?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Puis-je demander à ce que quelque-un fasse un exercice pour moi ?</h4>
								</div>
							</div>
							<a class="hover:text-indigo-500 hover:underline absolute bottom-5 text-sm text-indigo-700 font-bold cursor-pointer flex items-center" href="javascript:void(0)">
								<p>Montrer tout</p>
								<div>
									<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-arrow-narrow-right" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="#4338CA" fill="none" stroke-linecap="round" stroke-linejoin="round">
										<path stroke="none" d="M0 0h24v24H0z" fill="none" />
										<line x1="5" y1="12" x2="19" y2="12" />
										<line x1="15" y1="16" x2="19" y2="12" />
										<line x1="15" y1="8" x2="19" y2="12" />
									</svg>
								</div>
							</a>
						</div>
					</div>
					<div role="cell" class="bg-gray-100">
						<div class="bg-white ring ring-purple-500 p-5 rounded-md relative h-full w-full">
							<!-- class="absolute inset-0 object-center object-cover h-full w-full"  -->
							<span><img class="bg-gray-200 p-2 mb-5 rounded-full" src="https://i.ibb.co/bdGyLYk/pricetags-1.png" alt="pricetags-1" /></span>
							<h1 class="pb-4 text-2xl font-semibold">Payez pour plus d'avantages</h1>
							<div class="my-5">
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Puis payer un professeur particulier?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Quelles sont les bonus obtenus à une prise en charge par un professeur aggréé?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Comment faire ma demande de tutorat rémunéré?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Où et comment payer la personne en charge?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Y a t-il une politique de remboursement?</h4>
								</div>
							</div>
							<a class="hover:text-indigo-500 hover:underline absolute bottom-5 text-sm text-indigo-700 font-bold cursor-pointer flex items-center" href="javascript:void(0)">
								<p>Montrer tout</p>
								<div>
									<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-arrow-narrow-right" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="#4338CA" fill="none" stroke-linecap="round" stroke-linejoin="round">
										<path stroke="none" d="M0 0h24v24H0z" fill="none" />
										<line x1="5" y1="12" x2="19" y2="12" />
										<line x1="15" y1="16" x2="19" y2="12" />
										<line x1="15" y1="8" x2="19" y2="12" />
									</svg>
								</div>
							</a>
						</div>
					</div>
					<div role="cell" class="bg-gray-100">
						<div class="bg-white ring ring-purple-500 p-5 rounded-md relative h-full w-full">
							<!-- class="absolute inset-0 object-center object-cover h-full w-full"  -->
							<span><img class="bg-gray-200 p-2 mb-5 rounded-full" src="https://i.ibb.co/GT4KHvJ/card-1.png" alt="home-1" /></span>
							<h1 class="pb-4 text-2xl font-semibold">Questions de cours</h1>
							<div class="my-5">
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Comment calculer la TL d'un polynome à racine complexe ?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Quelles sont mes chances au DE de Machine Learning ?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Comment obtenir un signal biphase antipolaire aléatoire sans avoir touché à MATLAB ?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Quelqu'un qui peut m'aider en HTML ?</h4>
								</div>
							</div>
							<a class="hover:text-indigo-500 hover:underline absolute bottom-5 text-sm text-indigo-700 font-bold cursor-pointer flex items-center" href="javascript:void(0)">
								<p>Montrer tout</p>
								<div>
									<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-arrow-narrow-right" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="#4338CA" fill="none" stroke-linecap="round" stroke-linejoin="round">
										<path stroke="none" d="M0 0h24v24H0z" fill="none" />
										<line x1="5" y1="12" x2="19" y2="12" />
										<line x1="15" y1="16" x2="19" y2="12" />
										<line x1="15" y1="8" x2="19" y2="12" />
									</svg>
								</div>
							</a>
						</div>
					</div>
					<div role="cell" class="bg-gray-100">
						<div class="bg-white ring ring-purple-500 p-5 rounded-md h-full relative w-full">
							<!-- class="absolute inset-0 object-center object-cover h-full w-full"  -->
							<span><img class="bg-gray-200 p-2 mb-5 rounded-full" src="https://i.ibb.co/rG4r6NJ/notifications-1.png" alt="home-1" /></span>
							<h1 class="pb-4 text-2xl font-semibold">Contacter un prof ou un élève</h1>
							<div class="my-5">
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Je suis nouveau sur le site, comment faire?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Comment envoyer un message à quelqu'un?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Que puis-je faire en accédant à leur profil?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Puis-je envoyer un message tout en restant anonyme?</h4>
								</div>
							</div>
							<a class="hover:text-indigo-500 hover:underline absolute bottom-5 text-sm text-indigo-700 font-bold cursor-pointer flex items-center" href="javascript:void(0)">
								<p>Montrer tout</p>
								<div>
									<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-arrow-narrow-right" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="#4338CA" fill="none" stroke-linecap="round" stroke-linejoin="round">
										<path stroke="none" d="M0 0h24v24H0z" fill="none" />
										<line x1="5" y1="12" x2="19" y2="12" />
										<line x1="15" y1="16" x2="19" y2="12" />
										<line x1="15" y1="8" x2="19" y2="12" />
									</svg>
								</div>
							</a>
						</div>
					</div>
					<div role="cell" class="bg-gray-100">
						<div class="relative bg-white ring ring-purple-500 p-5 rounded-md relative h-full w-full">
							<!-- class="absolute inset-0 object-center object-cover h-full w-full"  -->
							<span><img class="bg-gray-200 p-2 mb-5 rounded-full" src="https://i.ibb.co/HFC1hqn/people-1.png" alt="home-1" /></span>
							<h1 class="pb-4 text-2xl font-semibold">Blabla</h1>
							<div class="my-5">
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Sujets hors-sujets</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Conversation générale</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Les Saints Memes</h4>
								</div>
							</div>
							<a class="hover:text-indigo-500 hover:underline absolute bottom-5 text-sm text-indigo-700 font-bold cursor-pointer flex items-center" href="javascript:void(0)">
								<p>Montrer tout</p>
								<div>
									<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-arrow-narrow-right" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="#4338CA" fill="none" stroke-linecap="round" stroke-linejoin="round">
										<path stroke="none" d="M0 0h24v24H0z" fill="none" />
										<line x1="5" y1="12" x2="19" y2="12" />
										<line x1="15" y1="16" x2="19" y2="12" />
										<line x1="15" y1="8" x2="19" y2="12" />
									</svg>
								</div>
							</a>
						</div>
					</div>
					<div role="cell" class="bg-gray-100">
						<div class="relative bg-white ring ring-purple-500 p-5 rounded-md relative h-full w-full">
							<!-- class="absolute inset-0 object-center object-cover h-full w-full"  -->
							<span><img class="bg-gray-200 p-2 mb-5 rounded-full" src="https://i.ibb.co/QX80fYm/lock-closed-1.png" alt="home-1" /></span>
							<h1 class="pb-4 text-2xl font-semibold">Proposer des améliorations à l'équipe</h1>
							<div class="my-5">
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Première fois sur le site, comment contacter l'équipe?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Que puis-je proposer?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Mon point de vue est-il vraiment important?</h4>
								</div>
								<div class="flex items-center pb-4 dark:border-gray-700 cursor-pointer w-full">
									<div>
										<svg xmlns="http://www.w3.org/2000/svg" width="12.5" height="16" fill="none" viewBox="0 0 24 24" stroke="currentColor">
											<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
										</svg>
									</div>
									<h4 class="text-md text-gray-900 dark:text-gray-100 pl-4">Ne suis-je pas le produit de mes parents?</h4>
								</div>
							</div>
							<a class="hover:text-indigo-500 hover:underline absolute bottom-5 text-sm text-indigo-700 font-bold cursor-pointer flex items-center" href="javascript:void(0)">
								<p>Montrer tout</p>
								<div>
									<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-arrow-narrow-right" width="16" height="16" viewBox="0 0 24 24" stroke-width="1.5" stroke="#4338CA" fill="none" stroke-linecap="round" stroke-linejoin="round">
										<path stroke="none" d="M0 0h24v24H0z" fill="none" />
										<line x1="5" y1="12" x2="19" y2="12" />
										<line x1="15" y1="16" x2="19" y2="12" />
										<line x1="15" y1="8" x2="19" y2="12" />
									</svg>
								</div>
							</a>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>