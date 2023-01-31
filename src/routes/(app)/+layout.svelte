<script>
	import '../../app.css';
	import { page } from '$app/stores';

	const navigation = [
		{
			title: 'Home',
			href: '/'
		},
		{
			title: 'Nutrientes',
			href: '/nutrients'
		},
		{
			title: 'Frutas',
			href: '/fruits'
		},
		{
			title: 'Sobre mim',
			href: '/about'
		}
	];
</script>

<div class="min-h-screen h-full w-screen">
	<header class="top-0 flex navbar bg-white shadow px-32">
		<div class="flex-1">
			<a href="/" class="btn btn-ghost normal-case text-xl">HealFruits</a>
		</div>
		<div class="flex-none">
			<ul class="menu menu-horizontal px-1">
				{#each navigation as navItem}
					<li>
						<a
							class="text-base btn-sm mx-1 {$page.url.pathname === navItem.href ? 'active' : ''} "
							href={navItem.href}>{navItem.title}</a
						>
					</li>
				{/each}
			</ul>
		</div>
	</header>
    <main class="h-96 flex-1">
        <slot />
    </main>
</div>
