<script>
	import DayNightToggle from './DayNightToggle.svelte';
	import Hamburger from './Hamburger.svelte';
	import System9 from './System9.svelte';
	console.log('foo');
</script>

<nav class="flex border-2 border-black">
	<div class="border-2 border-black">
		<div class="block lg:hidden">
			<div>
				<!-- hamburger -->
				<Hamburger />
			</div>
			<div>
				<System9 />
			</div>
		</div>
		<div class="hidden lg:block">
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
	<div>
		<DayNightToggle />
	</div>
</nav>
