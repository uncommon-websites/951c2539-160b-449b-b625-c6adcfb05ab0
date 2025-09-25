<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
		}
	];
</script>

<SecondaryHero
	title="Gift-giving made effortless"
	subtitle="One wishlist. Every store. Shared instantly."
	imageSrc="/generated/image-a-diverse-group-of-young-adults-gathered.webp"
	credibilityStats={[
		{ value: "2M+", label: "Active users" },
		{ value: "4.9★", label: "App Store rating" },
		{ value: "#1", label: "Rated wishlist app" }
	]}
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"It started with a familiar problem—birthdays and holidays that came with stress instead of ease. Our founders, like many millennials and Gen Z shoppers, were juggling scattered screenshots, notes apps, and endless group chats just to figure out what to buy or ask for. Gift lists were last-minute and awkward, and people kept receiving the same presents because no one knew what had already been bought. It wasn't thoughtful—it was chaos.",
		"That's why we built Listful. We wanted a better way to keep track of the things we love across all our favorite stores and make sharing them simple. So we created a wishlist you can build from any retailer, prioritize your picks with drag and drop, and share with a single link that updates in real time—without forcing anyone to download an app or make an account. Whether for kids' birthdays or wedding showers, Listful turns gift-giving into something smooth, smart, and surprisingly fun.",
		"Today, over 2 million people use Listful to plan better gifts, skip the stress, and actually enjoy the moment. With a 4.9-star rating and thousands of glowing reviews, we're just getting started. Our goal? To become the go-to platform for the $500B global gift market—helping millions more skip the guesswork and give with confidence. After all, as one user put it, 'Listful made my birthday so much easier—every gift was exactly what I wanted.'"
	]}
/>

<!-- Our Culture Section -->
<Culture {values} generating />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	generating
	stakeholderType="team"
	title="Our team."
	subtitle="Your partners in innovation."
	stakeholders={[
		{
			name: "Alex Morgan",
			position: "Founder & CEO",
			bio: "Started the company with a vision to transform the industry through innovative solutions.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Jamie Chen",
			position: "Chief Design Officer",
			bio: "Award-winning designer with a passion for creating intuitive and beautiful experiences.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Taylor Wright",
			position: "Head of Engineering",
			bio: "Technology enthusiast focused on building scalable systems that make a difference.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	generating
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	generating
	title="Ready to collaborate?"
	subtitle="Let's create something amazing"
	description="Join the companies already leveraging our expertise to transform their digital presence and achieve their business goals."
/>
