<!--
@component AboutTeaser
A minimalist founder story teaser that builds personal connection and company credibility.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Alex Morgan",
		role: "Founder & CEO",
		image: "https://images.unsplash.com/photo-1519085360753-af0119f7cbe7?w=400&h=400&fit=crop&crop=faces"
	};

	const founderQuote = "After watching dozens of e-commerce teams struggle with fragmented systems and disconnected customer experiences, I realized the problem wasn't technology—it was the lack of holistic thinking. We started this company to prove that seamless operations and exceptional UX aren't separate goals, they're two sides of the same transformation.";
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-3xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"${founderQuote}"`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="grid items-center gap-8">
				<div class="flex items-center justify-center gap-4">
					<img
						src={teamMember.image}
						alt={teamMember.name}
						class="size-16 rounded-full object-cover ring-1 ring-black/5"
					/>
					<div>
						<div class="text-callout">{teamMember.name}</div>
						<div class="text-caption text-emphasis-low">{teamMember.role}</div>
					</div>
					<Button href="/about" variant="secondary" size="sm" class="ml-6">Read our story</Button>
				</div>
			</div>
		</div>
	</div>
</section>
