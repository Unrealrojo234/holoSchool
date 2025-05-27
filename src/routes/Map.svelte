<section class="map-section">
	<h2>Our Location</h2>
	<div class="map-container">
		<!-- svelte-ignore a11y_missing_attribute -->
		<iframe
			src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d7979.4815197656835!2d35.00382!3d-0.357258!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x182aef9a2798cfd5%3A0xcd305e91745dcd43!2sHolo%20mixed%20s.s.!5e0!3m2!1sen!2ske!4v1748288323627!5m2!1sen!2ske"
			width="100%"
			height="450"
			style="border:0;"
			allowfullscreen=""
			loading="lazy"
			referrerpolicy="no-referrer-when-downgrade"
			aria-label="Google Maps location of Holo Secondary School"
		></iframe>
	</div>
	<p class="map-directions">
		<i class="fa-solid fa-car" aria-hidden="true"></i> 5km from Kisumu CBD along Kisumu-Kisii Highway
	</p>
</section>

<style>
	.map-section {
		max-width: 1000px;
		width: 100%;
		margin: 2rem auto;
		padding: 0 1rem;
		box-sizing: border-box;
	}

	.map-container {
		border-radius: 10px;
		overflow: hidden;
		box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
		margin: 1.5rem 0;
	}

	.map-directions {
		text-align: center;
		color: #666;
		font-size: clamp(0.85rem, 2vw, 0.9rem);
		margin-top: 1rem;
		display: flex;
		align-items: center;
		justify-content: center;
		gap: 0.5rem;
	}

	@media (max-width: 768px) {
		.map-section {
			width: 100%;
			margin: 0;
			padding: 0%;
		}

		.map-container iframe {
			height: 350px;
		}
	}

	@media (max-width: 480px) {
		.map-container iframe {
			height: 300px;
		}

		.map-directions {
			flex-direction: column;
			gap: 0.25rem;
		}
	}
</style>
