<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		credibilityStats = [],
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		credibilityStats?: Array<{ value: string; label: string }>;
		[key: string]: any;
	} = $props();
</script>

<header class="border-b border-gray-100 dark:border-gray-900" {...rest}>
	<div class="section-px section-py container mx-auto">
		<div class="grid gap-16 lg:grid-cols-2 lg:items-center">
			<!-- Content Column -->
			<div class="space-y-8">
				<div class="space-y-4">
					<h1 class="text-display">{title}</h1>
					<p class="text-title3 text-emphasis-dim">{subtitle}</p>
				</div>
				
				{#if credibilityStats.length > 0}
					<div class="grid grid-cols-3 gap-6">
						{#each credibilityStats as stat}
							<div class="text-center">
								<div class="text-title2 font-bold text-primary-600">{stat.value}</div>
								<div class="text-caption text-muted-foreground">{stat.label}</div>
							</div>
						{/each}
					</div>
				{/if}
			</div>

			<!-- Image Column -->
			<div class="aspect-video overflow-clip rounded-xl bg-gray-100 lg:aspect-[4/3]">
				<img
					class="h-full w-full object-cover"
					src={imageSrc}
					alt="Team collaboration and authentic moments"
				/>
			</div>
		</div>
	</div>
</header>
