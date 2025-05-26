<script>
	let year = new Date().getFullYear();
</script>

<main class="contact-main">
	<header class="contact-header">
		<h1><span>Get In Touch📬</span></h1>
		<p class="contact-subtitle text-secondary">We'd love to hear from you</p>
	</header>

	<div class="contact-container">
		<div class="contact-card">
			<div class="contact-icon">
				<i class="fa-solid fa-phone fa-2x"></i>
			</div>
			<div class="contact-info">
				<h3>Phone</h3>
				<a href="tel:254724454535" class="contact-link">+254 724 454 535</a>
			</div>
		</div>

		<div class="contact-card">
			<div class="contact-icon">
				<i class="fa-solid fa-envelope fa-2x"></i>
			</div>
			<div class="contact-info">
				<h3>Email</h3>
				<a href="mailto:peteromolloogutu@gmail.com" class="contact-link"
					>peteromolloogutu@gmail.com</a
				>
			</div>
		</div>

		<div class="contact-card">
			<div class="contact-icon">
				<i class="fa-solid fa-location-dot fa-2x"></i>
			</div>
			<div class="contact-info">
				<h3>Address</h3>
				<p class="contact-text">Kisumu-Kisii Highway, Kenya</p>
			</div>
		</div>
	</div>

	<footer class="contact-footer">
		<p>&copy; 2024–{year} Holo Secondary School. All rights reserved.</p>
	</footer>
</main>

<style>
	.contact-main {
		max-width: 800px;
		margin: 4rem auto;
		padding: 0 2rem;
		font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}

	.contact-header {
		text-align: center;
		margin-bottom: 3rem;
	}

	.contact-header h1 {
		font-size: 2.5rem;
		margin-bottom: 0.5rem;
	}

	.contact-subtitle {
		font-size: 1.1rem;
		font-style: italic;
	}

	.contact-container {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
		gap: 2rem;
		margin: 3rem 0;
	}

	.contact-card {
		border-radius: 10px;
		padding: 1.5rem;
		box-shadow: 0 3px 10px rgba(250, 250, 250, 0.08);
		display: flex;
		align-items: center;
		gap: 1.5rem;
		transition: all 0.3s ease;
	}

	.contact-card:hover {
		transform: translateY(-5px);
		box-shadow: 0 10px 20px rgba(250, 250, 250, 0.1);
	}

	.contact-icon {
		background: #f0f0f0;

		width: 60px;
		height: 60px;
		border-radius: 50%;
		display: flex;
		align-items: center;
		justify-content: center;
		color: #6c5ce7;
	}

	.contact-info h3 {
		margin: 0 0 0.5rem 0;
		font-size: 1.2rem;
	}

	.contact-link {
		color: #6c5ce7;
		text-decoration: none;
		font-weight: 500;
		transition: color 0.2s ease;
	}

	.contact-link:hover {
		color: #4a3dc0;
		text-decoration: underline;
	}

	.contact-text {
		margin: 0;
		color: #636e72;
	}

	.contact-footer {
		text-align: center;
		margin-top: 4rem;
		color: #7f8c8d;
		font-size: 0.9rem;
		padding-top: 1.5rem;
		border-top: 1px solid #eee;
	}

	@media (max-width: 768px) {
		.contact-container {
			grid-template-columns: 1fr;
		}

		.contact-header h1 {
			font-size: 2rem;
		}
	}
</style>
