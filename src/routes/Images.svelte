<script>
	import emblaCarouselSvelte from 'embla-carousel-svelte';
	import Autoplay from 'embla-carousel-autoplay';

	let embla;
	let selectedIndex = 0;

	const onSelect = () => {
		if (embla) {
			selectedIndex = embla.selectedScrollSnap();
		}
	};

	let options = {
		loop: true,
		align: 'center',
		skipSnaps: false
	};

	let plugins = [Autoplay({ delay: 5000, stopOnInteraction: true })];

	const images = [
		{
			src: 'https://unrealrojo234.github.io/holomixedsecsecondaryschool/Holo%20Pics/image_05.jpg',
			alt: 'Holo Secondary School building exterior',
			caption: `Girls' Team`
		},
		{
			src: 'https://unrealrojo234.github.io/holomixedsecsecondaryschool/Images/image_10.jpg',
			alt: 'Students in classroom',
			caption: 'Engaged learning environment'
		},
		{
			src: 'https://unrealrojo234.github.io/holomixedsecsecondaryschool/Holo%20Pics/image_03.jpg',
			alt: 'School football team',
			caption: 'Champion sports teams'
		},
		{
			src: 'https://unrealrojo234.github.io/holomixedsecsecondaryschool/Holo%20Pics/image_09.jpg',
			alt: '',
			caption: 'Agriculture Students'
		},
		{
			src: 'https://unrealrojo234.github.io/holomixedsecsecondaryschool/Holo%20Pics/image_08.jpg',
			alt: '',
			caption: 'Candidates'
		},
		{
			src: 'https://unrealrojo234.github.io/holomixedsecsecondaryschool/Images/finals_01.jpg',
			alt: '',
			caption: 'Prize Giving Day'
		},
		{
			src: 'https://unrealrojo234.github.io/holomixedsecsecondaryschool/Holo%20Pics/image_14.jpg',
			alt: 'Chemistry Lesson',
			caption: 'Chemistry Session'
		}
	];
</script>

<div class="carousel-wrapper">
	<div
		class="embla"
		use:emblaCarouselSvelte={{ options, plugins }}
		bind:this={embla}
		on:select={onSelect}
	>
		<div class="embla__container">
			{#each images as image (image.src)}
				<div class="embla__slide">
					<div class="slide-content">
						<img src={image.src} alt={image.alt} loading="lazy" class="carousel-image" />
						<div class="slide-caption">
							<p>{image.caption}</p>
						</div>
					</div>
				</div>
			{/each}
		</div>
	</div>

	<!-- <div class="carousel-controls">
		<button class="carousel-button prev" on:click={() => embla.scrollPrev()}>
			<i class="fa-solid fa-chevron-left"></i>
			<span class="sr-only">Previous slide</span>
		</button>
		<button class="carousel-button next" on:click={() => embla.scrollNext()}>
			<i class="fa-solid fa-chevron-right"></i>
			<span class="sr-only">Next slide</span>
		</button>
	</div> -->
</div>

<style>
	.carousel-wrapper {
		position: relative;
		max-width: 1200px;
		margin: 2rem auto;
		border-radius: 12px;
		overflow: hidden;
		box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
	}

	.embla {
		overflow: hidden;
		border-radius: 12px;
	}

	.embla__container {
		display: flex;
		height: 500px;
	}

	.embla__slide {
		flex: 0 0 100%;
		min-width: 0;
		position: relative;
	}

	.slide-content {
		position: relative;
		width: 100%;
		height: 100%;
	}

	.carousel-image {
		width: 100%;
		height: 100%;
		object-fit: cover;
		object-position: center;
		display: block;
	}

	.slide-caption {
		position: absolute;
		bottom: 0;
		left: 0;
		right: 0;
		background: linear-gradient(to top, rgba(0, 0, 0, 0.7), transparent);
		color: white;
		padding: 2rem 1.5rem 1rem;
		text-align: center;
		font-size: 1.2rem;
		font-weight: 500;
	}

	@media (max-width: 768px) {
		.embla__container {
			height: 350px;
		}

		.slide-caption {
			font-size: 1rem;
			padding: 1.5rem 1rem 0.5rem;
		}
	}
</style>
