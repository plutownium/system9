<script>
	import DayNightToggle from './DayNightToggle.svelte';
	import Hamburger from './Hamburger.svelte';
	import System9 from './System9.svelte';
	console.log('foo');
</script>

<div id="header-container" class="fixed w-full bg-red-500">
	<nav class="w-full flex justify-between border-4 border-black">
		<div id="header-left" class="w-full border-2 border-green-400">
			<div id="mobile-header" class="w-full flex lg:hidden bg-red-400">
				<div class="lg:hidden ml-4">
					<!-- hamburger -->
					<Hamburger />
				</div>
				<div class="w-full border-2 border-blue-500">
					<System9 />
				</div>
			</div>
			<div id="desktop-header" class="hidden lg:block">
				<div>
					<System9 />
				</div>
				<div>
					<div>
						<ul>
							<li>Products</li>
							<li>Company</li>
							<li>Partners</li>
							<li>Contact</li>
							<li>Jobs</li>
						</ul>
					</div>
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
