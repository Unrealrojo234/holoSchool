<script>
	import emblaCarouselSvelte from 'embla-carousel-svelte';

	import Autoplay from 'embla-carousel-autoplay';

	const options = {
		loop: true,
		align: 'start',
		containScroll: 'trimSnaps'
	};

	const plugins = [Autoplay({ delay: 5000 })];
</script>

<main class="main">
	<header class="benefits-header">
		<h1><span>Why Choose Holo Secondary School?🌟</span></h1>
		<p class="benefits-subtitle">Discover the advantages that set us apart</p>
	</header>
	<div class="embla" use:emblaCarouselSvelte={{ options, plugins }}>
		<div class="embla__container">
			{#each Array(11) as _, i}
				<div class="embla__slide">
					<div class="benefit-card">
						<div class="benefit-number">{i + 1}</div>
						<div class="benefit-content">
							{#if i === 0}
								<h3>Prime Location</h3>
								<p>Conveniently situated along the Kisumu-Kisii Highway for easy accessibility</p>
							{:else if i === 1}
								<h3>Resource-Rich Library</h3>
								<p>Well-stocked library to support research and learning</p>
							{:else if i === 2}
								<h3>Clean Water Supply</h3>
								<p>Reliable access to treated, clean water for all students</p>
							{:else if i === 3}
								<h3>Digital Learning</h3>
								<p>Fully digitized education using modern audio-visual teaching methods</p>
							{:else if i === 4}
								<h3>Expert Educators</h3>
								<p>Highly qualified and approachable teaching staff</p>
							{:else if i === 5}
								<h3>Supportive Staff</h3>
								<p>Friendly non-teaching personnel to assist students</p>
							{:else if i === 6}
								<h3>Dedicated Leadership</h3>
								<p>Active and supportive Board of Management</p>
							{:else if i === 7}
								<h3>Spiritual Growth</h3>
								<p>Strong emphasis on moral and spiritual development</p>
							{:else if i === 8}
								<h3>Diverse Activities</h3>
								<p>Wide range of co-curricular programs for all-round development</p>
							{:else if i === 9}
								<h3>Academic Rewards</h3>
								<p>Scholarship opportunities for top-performing students</p>
							{:else if i === 10}
								<h3>High-Speed Connectivity</h3>
								<p>Reliable WiFi internet connection throughout the school</p>
							{/if}
						</div>
					</div>
				</div>
			{/each}
		</div>
	</div>
</main>

<style>
	.benefits-header {
		text-align: center;
		margin-bottom: 3rem;
	}

	.benefits-header h1 {
		font-size: 2.5rem;
		margin-bottom: 0.5rem;
	}

	.benefits-subtitle {
		color: #7f8c8d;
		font-size: 1.1rem;
		font-style: italic;
	}

	.main {
		margin: 4rem auto;
		max-width: 1200px;
		font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}
	.embla {
		overflow: hidden;
		padding: 2rem 0;
	}
	.embla__container {
		display: flex;
		gap: 1rem;
		align-items: stretch; /* Ensures equal height in row */
	}
	.embla__slide {
		flex: 0 0 85%;
		min-width: 0;
		height: auto;

		@media (min-width: 768px) {
			flex: 0 0 calc(33.33% - 1rem);
		}
	}

	.benefit-card {
		border-radius: 10px;
		padding: 1.5rem;
		box-shadow: 0 3px 10px rgba(250, 250, 250, 0.1);
		display: flex;
		flex-direction: column;
		gap: 1rem;
		height: 100%; /* Take full height of slide */
		border-left: 4px solid #00c9a7;
		box-sizing: border-box; /* Include padding in height */
	}

	.benefit-content {
		flex: 1; /* Take remaining space */
		display: flex;
		flex-direction: column;
	}

	.benefit-content h3 {
		margin: 0 0 0.5rem 0;
		color: #00c9a7;
		font-size: 1.2rem;
		line-height: 1.3;
	}

	.benefit-content p {
		margin: 0;
		line-height: 1.5;
		flex: 1; /* Push text to top */
	}

	.benefit-number {
		background: black;
		color: white;
		width: 30px;
		height: 30px;
		border-radius: 50%;
		display: flex;
		align-items: center;
		justify-content: center;
		font-weight: bold;
		flex-shrink: 0;
	}

	/* Responsive adjustments */
	@media (max-width: 767px) {
		.embla__slide {
			flex: 0 0 90%;
		}

		.benefit-card {
			padding: 1rem;
		}
	}
</style>
