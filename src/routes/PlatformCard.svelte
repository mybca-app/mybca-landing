<script lang="ts">
	const {
		fullHeight = false,
		headingText,
		descriptionText = "",
		imageLink,
		imageAltText = "",
	}: {
		fullHeight?: boolean,
		headingText: string,
		descriptionText?: string,
		imageLink?: string,
		imageAltText?: string,
	} = $props();
</script>

<div
	class={`bg-mybca-light-bg-surface dark:bg-mybca-dark-bg-surface hover:bg-mybca-light-bg-surface-200 hover:dark:bg-mybca-dark-bg-surface-200 transition
    rounded-xl pt-4 px-4 ${imageLink ? '' : 'pb-4'} ${fullHeight ? 'row-span-2' : 'row-span-1'} flex flex-col`}
>
	<div>
		<div class="p-3">
			<h2 class="font-semibold font-serif text-2xl">{headingText}</h2>
			<p>{descriptionText}</p>
		</div>
		{#if imageLink}
		<div class="flex grow items-end overflow-hidden">
			<img src={imageLink} alt={imageAltText} class="object-cover w-full h-full">
		</div>
		{/if}
	</div>
</div>
