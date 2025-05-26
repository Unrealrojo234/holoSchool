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
		>
		</iframe>
	</div>
	<p class="map-directions">
		<i class="fa-solid fa-car"></i> 5km from Kisumu CBD along Kisumu-Kisii Highway
	</p>
</section>

<style>
	.map-section {
		margin: 3rem auto;
		max-width: 1000px;
		padding: 0 1rem;
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
		font-size: 0.9rem;
		margin-top: 1rem;
	}
</style>
