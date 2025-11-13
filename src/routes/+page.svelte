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
	centered={false}
	title="Transform e-commerce into seamless customer experiences"
	subtitle="Holistic UX design and operational refinement that turns fragmented operations into cohesive, conversion-driven journeys."
	imageSrc="https://www.unc.mn/image-placeholder.svg"
/>
<LogoScroller
	label="Trusted by leading commerce brands"
	logoUrls={[
		'https://cdn.brandfetch.io/warbyparker.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/glossier.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/everlane.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/allbirds.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we do"
	text="We partner with e-commerce brands to transform fragmented operations into cohesive customer experiences. Through holistic UX design and operational refinement, we turn disconnected touchpoints into seamless journeys that drive conversion and retention. Our phased approach eliminates implementation fears while delivering measurable results across the $5.5T commerce market."
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Krishnan",
			position: "Director of E-commerce",
			company: "Luxe Home Living",
			quote:
				"The holistic transformation cut our checkout abandonment by 42% in just three months. Their phased approach meant zero disruption to daily operations while we saw immediate improvements in conversion rates.",
			image: "https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?w=400&h=400&fit=crop&crop=faces"
		},
		{
			name: "Marcus Thompson",
			position: "VP of Digital Experience",
			company: "Heritage Fashion Co.",
			quote:
				"We recovered six months of development time by partnering with their team. What would have cost us $300K in hiring and trial-and-error was delivered seamlessly with measurable ROI from week one.",
			image: "https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?w=400&h=400&fit=crop&crop=faces"
		},
		{
			name: "Mei Chen",
			position: "Head of Customer Experience",
			company: "Botanica Beauty",
			quote:
				"Their operational refinement eliminated 68% of our customer support tickets. The integrated UX changes transformed our fragmented touchpoints into a cohesive journey that customers actually enjoy.",
			image: "https://images.unsplash.com/photo-1580489944761-15a19d654956?w=400&h=400&fit=crop&crop=faces"
		}
	]}
/>

<Features
	title="Our approach"
	subtitle="We transform fragmented e-commerce operations into cohesive experiences that drive measurable growth through strategic design and operational excellence."
	features={[
		{
			title: "Holistic UX transformation",
			description:
				"We redesign every customer touchpoint with a unified design language that eliminates friction and creates intuitive paths to purchase."
		},
		{
			title: "Operational refinement",
			description:
				"Your backend systems become as seamless as your frontend. We streamline workflows, integrate platforms, and eliminate operational bottlenecks that slow growth."
		},
		{
			title: "Phased transformation roadmaps",
			description:
				"Change without disruption through carefully sequenced rollouts that minimize risk while delivering incremental value at every stage."
		},
		{
			title: "Retention-focused metrics",
			description:
				"We measure what matters by tracking customer lifetime value, repeat purchase rates, and engagement depth rather than vanity metrics."
		},
		{
			title: "Seamless platform integration",
			description:
				"Your commerce stack works as one cohesive system, connecting inventory, fulfillment, marketing, and analytics into unified customer experiences."
		},
		{
			title: "Conversion architecture",
			description:
				"Strategic design decisions backed by behavioral psychology and conversion research that turn browsers into buyers and buyers into advocates."
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Ready to transform your e-commerce experience?"
	subtitle="Start your journey today"
	description="Join leading commerce brands who've eliminated operational friction and increased conversions through our phased transformation approach. No disruption, no guesswork—just measurable results from week one."
	imageSrc="https://images.unsplash.com/photo-1556761175-b413da4baf72?w=800&h=1000&fit=crop&crop=faces"
	callsToAction={[
		{
			href: "/contact",
			label: "Schedule a consultation",
			variant: "primary"
		},
		{
			href: "/about",
			label: "Learn our approach",
			variant: "secondary"
		}
	]}
/>
