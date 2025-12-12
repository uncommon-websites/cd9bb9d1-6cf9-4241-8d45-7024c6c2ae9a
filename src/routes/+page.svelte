<script lang="ts">
	import { onMount } from 'svelte';

	let scrollY = 0;
</script>

<svelte:window bind:scrollY />

<div class="font-sans text-gray-900 antialiased selection:bg-primary-200 selection:text-primary-900">

	<!-- Hero Section -->
	<section class="relative min-h-screen w-full bg-gradient-to-b from-gray-900 via-gray-800 to-white text-white px-6 md:px-12 lg:px-24 pt-32 pb-24 flex flex-col justify-between">
		<div class="max-w-5xl">
			<h1 class="font-serif text-5xl md:text-7xl lg:text-8xl leading-[1.1] md:leading-[1.1] tracking-tight">
				We transform creative visions into polished brand identities through collaborative iteration.
			</h1>
		</div>

		<div class="mt-24">
			<a href="#work" class="inline-flex items-center justify-center px-6 py-3 border border-white/30 rounded-full text-sm font-medium hover:bg-primary-500 hover:text-white hover:border-primary-500 transition-colors duration-300 backdrop-blur-sm">
				View our work
			</a>
		</div>
	</section>

	<!-- Trusted Partners -->
	<section class="bg-white px-6 md:px-12 lg:px-24 py-16 md:py-24">
		<p class="text-lg md:text-xl text-gray-600 mb-12">Trusted by ambitious startups and established brands</p>
		
		<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-4 md:gap-8">
			<!-- Logos placeholders -->
			{#each ['Notion', 'Stripe', 'Figma', 'Linear', 'Vercel', 'Framer'] as partner}
				<div class="h-20 bg-gray-50 rounded-lg flex items-center justify-center grayscale opacity-70 hover:opacity-100 hover:grayscale-0 transition-all duration-300">
					<span class="font-semibold text-gray-800">{partner}</span>
				</div>
			{/each}
		</div>
	</section>

    <!-- Work Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24" id="work">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 md:mb-24">
            <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900">Selected work</h2>
            <a href="/work" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                See all <span class="ml-2">→</span>
            </a>
        </div>

        <div class="space-y-24 md:space-y-32">
            <!-- Project 1: Verdant Fashion -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Verdant Fashion</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        A complete brand identity for a sustainable fashion startup, from logo design to brand guidelines, creating a cohesive visual language that reflects their eco-conscious values.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Brand Identity</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Visual Design</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-designer-working-on-brand-identity-sketc-1765515649413-0.webp" alt="Brand identity design process" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 2: Nexus Workspace -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Nexus Workspace</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Workspace branding for a tech startup, including environmental graphics, signage, and interior design elements that inspire creativity and collaboration.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Environmental Design</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Brand Identity</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-modern-minimalist-office-interior-with-n-1765515652666-1.webp" alt="Modern workspace interior" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 3: Pure Botanics -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Pure Botanics</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Packaging design for an organic skincare line that balances elegance with sustainability, featuring custom illustrations and a refined color palette.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Packaging Design</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Brand Identity</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Illustration</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-elegant-product-packaging-design-mockups-1765515655706-2.webp" alt="Product packaging design" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 4: Ember Kitchen -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Ember Kitchen</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Complete restaurant branding including logo, menu design, signage, and digital presence for a farm-to-table dining experience.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Brand Identity</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Print Design</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-creative-team-collaborating-around-a-tab-1765515658538-3.webp" alt="Design collaboration" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>
        </div>
        
        <div class="mt-12 md:hidden">
            <a href="/work" class="flex items-center text-gray-500 hover:text-gray-900 transition-colors">
                See all <span class="ml-2">→</span>
            </a>
        </div>
    </section>

    <!-- Process Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-16 max-w-3xl">Our collaborative process</h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Discover -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Discover</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We start by understanding your vision, audience, and goals through collaborative workshops and research, laying the foundation for authentic brand expression.
                </p>
                <div class="mt-8 flex justify-center h-48 items-center">
                    <div class="w-24 h-24 rounded-full border-4 border-primary-500 flex items-center justify-center">
                        <span class="text-3xl">1</span>
                    </div>
                </div>
            </div>

            <!-- Design -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Design</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    Through iterative design cycles, we craft visual identities that resonate with your audience while staying true to your brand values and vision.
                </p>
                <div class="mt-8 flex justify-center h-48 items-center">
                    <div class="w-24 h-24 rounded-full border-4 border-primary-500 flex items-center justify-center">
                        <span class="text-3xl">2</span>
                    </div>
                </div>
            </div>

            <!-- Deliver -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Deliver</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We provide polished, production-ready assets and comprehensive brand guidelines, ensuring consistent implementation across all touchpoints.
                </p>
                <div class="mt-8 flex justify-center h-48 items-center">
                    <div class="w-24 h-24 rounded-full border-4 border-primary-500 flex items-center justify-center">
                        <span class="text-3xl">3</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Thoughts Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <div class="flex flex-col md:flex-row justify-between items-end mb-12">
            <h2 class="font-serif text-3xl md:text-4xl text-gray-900">Insights & inspiration</h2>
            <a href="/thoughts" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                Read all <span class="ml-2">→</span>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Blog Post 1 -->
            <div class="group cursor-pointer">
                <div class="aspect-square bg-primary-600 rounded-lg overflow-hidden mb-4 relative">
                     <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-2xl text-center p-8">The Power of Iteration in Brand Design</div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Why the best brands are built through collaborative refinement</h3>
            </div>

             <!-- Blog Post 2 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-900 rounded-lg overflow-hidden mb-4 relative">
                    <div class="absolute inset-0 flex items-center justify-center text-white text-center p-8 flex-col">
                        <span class="text-sm uppercase tracking-widest mb-2">Typography</span>
                        <span class="text-3xl font-serif">Matters</span>
                    </div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Choosing the right typeface for your brand identity</h3>
            </div>

             <!-- Blog Post 3 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-100 rounded-lg overflow-hidden mb-4 relative">
                     <img src="https://images.unsplash.com/photo-1634128221889-82ed6efebfc3?q=80&w=1000&auto=format&fit=crop" alt="Color swatches" class="w-full h-full object-cover" />
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Color psychology in brand design: What your palette says about you</h3>
            </div>

             <!-- Blog Post 4 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-800 rounded-lg overflow-hidden mb-4 relative">
                    <img src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?q=80&w=1000&auto=format&fit=crop" alt="Team collaboration" class="w-full h-full object-cover opacity-60" />
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Building brands that scale: Lessons from 500+ client projects</h3>
            </div>

             <!-- Blog Post 5 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-primary-500 rounded-lg overflow-hidden mb-4 relative flex items-center justify-center">
                    <div class="text-white text-center p-8">
                        <div class="text-6xl mb-4">✦</div>
                        <div class="text-xl font-serif">Craft</div>
                    </div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">The importance of craft in an AI-driven design world</h3>
            </div>

             <!-- Blog Post 6 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-900 rounded-lg overflow-hidden mb-4 relative">
                     <img src="https://images.unsplash.com/photo-1558655146-d09347e92766?q=80&w=1000&auto=format&fit=crop" alt="Design tools" class="w-full h-full object-cover opacity-40" />
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">From concept to launch: Our design process demystified</h3>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="px-6 md:px-12 lg:px-24 py-12">
        <div class="bg-gradient-to-r from-gray-100 to-gray-50 rounded-2xl p-8 md:p-16 lg:p-20">
            <h3 class="font-serif text-2xl md:text-3xl text-gray-900 mb-4">Stay inspired</h3>
            <p class="text-gray-600 mb-8 max-w-md">Get design insights, case studies, and inspiration delivered to your inbox monthly.</p>
            
            <form class="flex flex-col sm:flex-row gap-4 max-w-lg">
                <input type="email" placeholder="your@email.com" class="flex-1 bg-white border border-gray-200 rounded-lg px-4 py-3 text-sm placeholder:text-gray-400 focus:ring-2 focus:ring-primary-500 focus:border-transparent outline-none" />
                <button type="submit" class="bg-gray-900 hover:bg-primary-600 transition-colors text-white px-6 py-3 rounded-lg text-sm font-medium">
                    Subscribe
                </button>
            </form>
            <p class="text-[10px] text-gray-500 mt-4">We respect your privacy. Unsubscribe at any time.</p>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="relative bg-gradient-to-b from-gray-800 via-gray-900 to-gray-950 pt-32 pb-48 px-6 md:px-12 lg:px-24 overflow-hidden">
        <div class="max-w-5xl relative z-10">
            <h2 class="font-serif text-4xl md:text-6xl lg:text-7xl text-white leading-tight mb-8">
                Ready to transform your brand? <br />
                <span class="text-white/70">Let's collaborate to create a visual identity that resonates with your audience and stands the test of time.</span>
            </h2>
            
            <div class="mt-16">
                 <a href="/contact" class="inline-flex items-center justify-center px-6 py-3 bg-primary-500 hover:bg-primary-600 rounded-full text-sm font-medium text-white transition-colors duration-300">
                    Start a project
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-950 text-gray-300 px-6 md:px-12 lg:px-24 pt-24 pb-12 relative overflow-hidden">
        <div class="relative z-10">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-24">
                <div class="col-span-1 md:col-span-2">
                    <a href="/contact" class="text-2xl font-medium hover:text-primary-400 transition-colors inline-flex items-center">
                        Start a project <span class="ml-2">→</span>
                    </a>
                </div>
                
                <div class="space-y-4">
                    <h4 class="font-medium text-white">Contact</h4>
                    <div class="pt-4 text-sm space-y-1">
                        <p>hello@company.design</p>
                        <p>+1 (555) 123-4567</p>
                    </div>
                </div>

                <div class="space-y-4">
                    <h4 class="font-medium text-white">Follow</h4>
                    <div class="pt-4 text-sm space-y-1">
                        <p><a href="#" class="hover:text-primary-400 transition-colors">Instagram</a></p>
                        <p><a href="#" class="hover:text-primary-400 transition-colors">LinkedIn</a></p>
                        <p><a href="#" class="hover:text-primary-400 transition-colors">Dribbble</a></p>
                    </div>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between items-end border-t border-white/10 pt-8">
                <div class="mb-4 md:mb-0">
                    <!-- Logo Icon -->
                    <svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-white">
                        <rect x="4" y="4" width="11" height="11" rx="2" fill="currentColor" />
                        <rect x="9" y="9.5" width="10" height="10" rx="2" fill="currentColor" fill-opacity="0.24" />
                    </svg>
                </div>
                
                <div class="flex gap-6 text-xs font-medium">
                    <a href="#" class="hover:text-primary-400 transition-colors">Work</a>
                    <a href="#" class="hover:text-primary-400 transition-colors">About</a>
                    <a href="#" class="hover:text-primary-400 transition-colors">Contact</a>
                    <a href="#" class="hover:text-primary-400 transition-colors">Privacy</a>
                </div>
            </div>

            <div class="flex justify-between text-[10px] opacity-50 mt-12">
                <p>© 2025 Company Design Studio</p>
                <p>All rights reserved</p>
            </div>
        </div>
    </footer>
</div>

<style>
    /* Custom utility for vertical writing mode */
    .writing-vertical-rl {
        writing-mode: vertical-rl;
    }
</style>

