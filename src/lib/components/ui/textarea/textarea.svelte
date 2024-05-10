<script>
	import { Label } from '$lib/components/ui/label';
	import { cn } from '$lib/utils.js';
	let className = undefined;
	export let value = undefined;
	export { className as class };
	export let readonly = undefined;
	export let labelText = undefined;
</script>

<div>
	<Label
		class="relative left-4 top-3 bg-background p-1 text-sm font-medium text-muted-foreground"
		for={labelText}>{labelText}</Label
	>
	<textarea
		class={cn(
			'flex min-h-[80px] w-full rounded-md border-2 border-input bg-background px-3 py-2 text-sm ring-offset-background placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50',
			className
		)}
		bind:value
		{readonly}
		on:blur
		on:change
		on:click
		on:focus
		on:keydown
		on:keypress
		on:keyup
		on:mouseover
		on:mouseenter
		on:mouseleave
		on:paste
		on:input
		{...$$restProps}
	></textarea>
</div>
