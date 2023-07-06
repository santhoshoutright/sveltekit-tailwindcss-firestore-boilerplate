<script>
	import Accordion from '$lib/Accordion.svelte';
	const accordions = [1, 2, 3, 4, 5];
</script>

<div class="p-10 mx-auto max-w-7xl">
	<h1 class="bg-primary text-white p-8 rounded-xl text-3xl font-bold mb-4 text-center">
		Welcome to TSOC development
	</h1>
	<p class="mb-4">
		Visit <a class="bg-primary text-white hover:underline p-1" href="https://kit.svelte.dev"
			>kit.svelte.dev</a
		> to learn about Svelte and SvelteKit
	</p>
	<p class="mb-4">
		Visit <a  class="bg-primary text-white hover:underline p-1" href="https://tailwindcss.com">tailwindcss.com</a> to learn about TailwindCSS
	</p>
	<p class="mb-12">
		Yes, you can remove <span  class="bg-primary text-white p-1"> +page.svelte </span> file and you can start making your awesome website.
	</p>

	<div class="mb-4">
		<h1 class="text-white font-semibold">Extras</h1>
		<h2 class="mb-4">
			Below collapsible accordion is just a Daisy UI pre made utility classes on top of TailwindCSS
			utility classes
		</h2>
		<p>
			This one is optional: There are different combination of components availble in Daisy UI you
			can started using it on your next stunning website. Why don't give a try and you won't regret
			it. Visit <a class="bg-primary text-white hover:underline p-1" href="https://daisyui.com/">daisyui.com</a> to learn about Daisy UI
		</p>
	</div>
	<div class="space-y-2">
		{#each accordions as accordion}
			<Accordion number={accordion} />
		{/each}
	</div>
</div>
