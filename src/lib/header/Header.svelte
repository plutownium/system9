<script>
	import { text } from 'svelte/internal';
	import DayNightToggle from './DayNightToggle.svelte';
	import Hamburger from './Hamburger.svelte';
	import HeaderItem from './HeaderItem.svelte';
	import System9 from './System9.svelte';
	console.log('foo');
</script>

<div id="header-container" class="fixed w-full bg-red-500">
	<nav class="w-full flex border-4 border-black">
		<div id="left-box" class="w-12 h-12 flex items-center">
			<!-- left-box -->
			<div class="block lg:hidden ml-4 w-12">
				<!-- hamburger -->
				<Hamburger />
			</div>
		</div>
		<div id="middle-header" class="w-full border-2 border-green-400">
			<div
				id="mobile-header"
				class="w-full h-full flex lg:hidden justify-center items-center bg-red-800"
			>
				<System9 />
			</div>
			<div id="desktop-header" class="hidden lg:flex justify-between">
				<div>
					<System9 />
				</div>
				<div class="flex">
					<ul class="flex">
						<HeaderItem text="Products" anchor={'#products'} />
						<HeaderItem text="Company" anchor={'#company'} />
						<HeaderItem text="Partners" anchor={'#partners'} />
						<HeaderItem text="Company" anchor={'#company'} />
						<HeaderItem text="Jobs" anchor="jobs" />
					</ul>
				</div>
			</div>
		</div>
		<div
			id="theme-toggle"
			class="lg:border lg:border-l-midnight lg:dark:border-l-sand lg:border-t-0 lg:border-b-0 lg:border-r-0 w-20 h-20 "
		>
			<DayNightToggle />
		</div>
	</nav>
</div>
