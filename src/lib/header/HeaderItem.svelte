<script>
	export let text = '';
	export let anchor = '';
</script>

<li>
	<a class="hover-underline" href="/{anchor}">{text}</a>
	<div
		class="line absolute hover:before:h-3 h-5 mt-2 border border-r-0 border-b-0 border-t-0 w-12"
	/>
</li>
