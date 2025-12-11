<script lang="ts">
	import PlatformCard from './PlatformCard.svelte';
	import iphoneScreenshot from '$lib/assets/screenshots/iphone-dark-main-page.png';
</script>

<div class="mt-4 grid grid-cols-1 md:grid-cols-2 grid-rows-2 gap-4 min-h-128">
	<PlatformCard
		fullHeight={true}
		headingText="iOS app"
		descriptionText="Download from the App Store for bus notifications, lunch menus, and more."
		imageLink={iphoneScreenshot}
		imageAltText="Screenshot of the myBCA main page on an iPhone."
	/>
	<PlatformCard
		headingText="Web app"
		descriptionText="Access myBCA from your computer with our web app."
		targetLink="https://app.mybca.link"
	/>
	<PlatformCard headingText="Android app" descriptionText="Coming soon to the Google Play Store." />
</div>
