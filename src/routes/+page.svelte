<script lang="ts">
	import CardGrid from './PlatformCardGrid.svelte';
	import Hero from './Hero.svelte';
</script>

<svelte:head>
	<title>myBCA • the only BCA app you need</title>
	<meta
		name="description"
		content="myBCA is the all-in-one app for students of the Bergen County Academies, with bus notifications, lunch menus, events, and more."
	/>
</svelte:head>

<Hero />
<section>
	<CardGrid />
</section>
