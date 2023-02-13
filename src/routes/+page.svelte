<script>
	import Aside from '$lib/aside/Aside.svelte';
	import Header from '../lib/header/Header.svelte';
	import Content from '../lib/Content.svelte';
</script>

<!-- <Aside />
<main>
	<Header />
	<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
</main> -->

<div class="flex">
	<Aside />
	<Content />
</div>
