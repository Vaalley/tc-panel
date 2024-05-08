<script>
	import { cn } from '$lib/utils.js';
	let className = undefined;
	export let value = undefined;
	export { className as class };
	export let readonly = undefined;
	export let labelText = undefined;
</script>

<div>
	<label
		class="relative left-4 top-3 bg-background p-1 text-sm font-medium text-muted-foreground"
		for={labelText}>{labelText}</label
	>
	<input
		id={labelText}
		class={cn(
			'flex h-10 w-full rounded-md border-2 border-input bg-background px-4 py-6 text-base ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50',
			className
		)}
		bind:value
		{readonly}
		on:blur
		on:change
		on:click
		on:focus
		on:focusin
		on:focusout
		on:keydown
		on:keypress
		on:keyup
		on:mouseover
		on:mouseenter
		on:mouseleave
		on:paste
		on:input
		on:wheel|passive
		{...$$restProps}
	/>
</div>
