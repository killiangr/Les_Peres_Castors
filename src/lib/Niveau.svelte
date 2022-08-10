<script>
	export let src;
    export let id;
	export let href;
</script>

<div id={id} class="lg:w-1/5 sm:w-1/2 p-4">
	<div class="flex relative flex-col">
		<a href={href} class="relative w-full">
			<img alt="gallery" class="rounded-md relative inset-0 w-full h-full object-cover object-center" {src} />
		</a>
	</div>
</div>
