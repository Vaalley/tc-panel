<script>
	import { Input } from '$lib/components/ui/input';
</script>

<svelte:head>
	<title>🎬 Trap Cosmos Render Panel</title>
</svelte:head>

<main class="p-16 font-montserrat">
	<h2
		class="scroll-m-20 text-3xl font-medium tracking-tight text-muted-foreground transition-colors first:mt-0"
	>
		New Upload
	</h2>
	<h1 class="scroll-m-20 text-4xl font-bold tracking-tight lg:text-5xl">
		Artist Name - Title Song (Someone Remix)
	</h1>

	<Input
		value="https://soundcloud.com/tokzick/tupac-hit-em-up-tokzick-flip"
		labelText="SoundCloud URL"
	/>
	<Input
		value="https://unsplash.com/photos/a-boat-sitting-on-top-of-a-lake-next-to-a-mountain-3_PF89nVmuo"
		labelText="Unsplash URL"
	/>
	<Input value="I'm a title" labelText="Title" />
</main>
