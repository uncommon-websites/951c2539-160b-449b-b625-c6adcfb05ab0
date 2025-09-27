<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="All your gift ideas. In one place."
	subtitle="Simplify giving and sharing with smart wishlists."
	imageSrc="/generated/image-a-candid-documentary-style-medium-shot-o.webp"
	centered={false}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/pinterest.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/target.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/etsy.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/shopify.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Mehta",
			position: "Marketing Manager",
			company: "Bay Area Parent",
			quote:
				"Listful saved me hours planning my daughter's birthday party. Instead of juggling bookmarks across five different stores, I organized everything in one place and shared the link with family. No more duplicate gifts!",
			image: "/generated/image-candid-environmental-portrait-of-priya-m.webp"
		},
		{
			name: "Marcus Thompson",
			position: "UX Designer",
			company: "Remote Dad",
			quote:
				"Creating Christmas lists used to be such a headache. With Listful's price comparison, I found the best deals across retailers and saved over $200 last season. My wife and I can coordinate gifts without ruining surprises.",
			image: "/generated/image-candid-environmental-portrait-of-marcus-.webp"
		},
		{
			name: "Elena Rodriguez",
			position: "Graduate Student",
			company: "UCLA",
			quote:
				"Wedding registry chaos became organized bliss. Listful let me add items from Etsy, Target, and local boutiques all in one list. Guests loved how easy it was to browse and buy without creating accounts.",
			image: "/generated/image-candid-environmental-portrait-of-elena-r.webp"
		}
	]}
/>

<Features
	title="Everything you need for gifting"
	subtitle="Transform scattered gift ideas into organized, shareable wishlists that make giving effortless"
	features={[
		{
			title: "Add from any store",
			description: "Copy and paste any product link from Amazon, Target, Etsy, or anywhere online to build your perfect wishlist.",
			imageSrc: "/generated/image-a-young-adult-smiling-arranges-a-colorfu.webp"
		},
		{
			title: "Never duplicate gifts",
			description: "Real-time purchase tracking shows what's been bought, eliminating awkward duplicate gifts and gift-giving anxiety.",
			imageSrc: "/generated/image-a-group-of-friends-gathered-around-a-kit.webp"
		},
		{
			title: "Share without friction",
			description: "Send your wishlist link to anyone and they can view and buy gifts without creating an account.",
			imageSrc: "/generated/image-family-members-of-different-ages-sit-tog.webp"
		},
		{
			title: "Compare prices automatically",
			description: "See the best prices across retailers and save money on every gift with automatic price comparison.",
			imageSrc: "/generated/image-two-people-compare-gift-items-by-holding.webp"
		},
		{
			title: "Drag to prioritize",
			description: "Easily reorder your wishlist by importance so gift-givers know exactly what you want most.",
			imageSrc: "/generated/image-a-person-sits-cross-legged-on-a-cozy-rug.webp"
		},
		{
			title: "Works everywhere",
			description: "From Nike to local boutiques, add products from any website to create unified wishlists across all your favorite stores.",
			imageSrc: "/generated/image-a-group-of-friends-and-family-gather-aro.webp"
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
