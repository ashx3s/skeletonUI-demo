<script>
	import '../app.postcss';
	import { AppShell, AppBar, Avatar } from '@skeletonlabs/skeleton';
</script>

<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<AppBar>
			<svelte:fragment slot="lead">
				<strong class="text-xl uppercase">Skeleton</strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://discord.gg/EXqV7W8MtY"
					target="_blank"
					rel="noreferrer"
				>
					Discord
				</a>
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://twitter.com/SkeletonUI"
					target="_blank"
					rel="noreferrer"
				>
					Twitter
				</a>
				<a
					class="btn btn-sm variant-ghost-surface"
					href="https://github.com/skeletonlabs/skeleton"
					target="_blank"
					rel="noreferrer"
				>
					GitHub
				</a>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>

	<svelte:fragment slot="sidebarLeft">
		<div class="hidden lg:block lg:px-12 lg:mt-20">
			<ul>
				<li>List Items</li>
				<li>List Items</li>
				<li>List Items</li>
			</ul>
		</div>
	</svelte:fragment>
	<svelte:fragment slot="pageHeader">
		<Avatar
			src="https://images.unsplash.com/photo-1617296538902-887900d9b592?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzExMDB8&ixlib=rb-4.0.3&w=128&h=128&auto=format&fit=crop"
			width="w-32"
			rounded="rounded-full"
		/>
	</svelte:fragment>
	<!-- Router Slot -->
	<slot />
	<svelte:fragment slot="footer">&copy; Lilyx 2023</svelte:fragment>
</AppShell>
