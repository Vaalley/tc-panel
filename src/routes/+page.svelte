<script>
	import { Input } from '$lib/components/ui/input';
	import { Textarea } from '$lib/components/ui/textarea';
</script>

<svelte:head>
	<title>🎬 Trap Cosmos Render Panel</title>
</svelte:head>

<main class="grid grid-cols-2 gap-12 p-12 font-montserrat">
	<!-- LEFT PANE -->
	<div class="space-y-4">
		<h4 class="scroll-m-20 text-xl font-semibold tracking-tight text-muted-foreground">
			New Upload
		</h4>
		<h1 class="scroll-m-20 text-4xl font-bold tracking-tight lg:text-5xl">
			Artist Name - Title Song (Someone Remix)
		</h1>

		<Input
			placeholder="https://soundcloud.com/iffoundmusic/die-4-u-w-noll-damnboy"
			labelText="SoundCloud URL"
		/>
		<Input
			placeholder="https://unsplash.com/photos/cars-on-road-between-high-rise-buildings-during-night-time-yVUQlyRlJSw"
			labelText="Unsplash URL"
		/>

		<h4 class="scroll-m-20 text-2xl font-semibold tracking-tight text-muted-foreground">
			YouTube Metadata
		</h4>
		<Input placeholder="if found, nøll, damnboy! - die 4 u" labelText="Title" />
		<Textarea placeholder="🔥 die 4 u 🔥" labelText="Description" />
	</div>

	<!-- RIGHT PANE -->
	<div>
		<p class="text-xs font-medium text-muted-foreground">Background Style</p>
	</div>
</main>
