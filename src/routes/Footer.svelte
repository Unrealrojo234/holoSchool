<script>
	let year = new Date().getFullYear();
</script>

<main class="contact-main container-fluid">
	<header class="contact-header">
		<h1><span>Get In Touch📬</span></h1>
		<p class="contact-subtitle text-secondary">We'd love to hear from you</p>
	</header>

	<div class="contact-container">
		<div class="contact-card card">
			<div class="contact-icon">
				<i class="fa-solid fa-phone fa-2x" aria-hidden="true"></i>
			</div>
			<div class="contact-info">
				<h3>Phone</h3>
				<a href="tel:254724454535" class="contact-link">+254 724 454 535</a>
			</div>
		</div>

		<div class="contact-card card">
			<div class="contact-icon">
				<i class="fa-solid fa-envelope fa-2x" aria-hidden="true"></i>
			</div>
			<div class="contact-info">
				<h3>Email</h3>
				<a href="mailto:peteromolloogutu@gmail.com" class="contact-link"
					>peteromolloogutu@gmail.com</a
				>
			</div>
		</div>

		<div class="contact-card card">
			<div class="contact-icon">
				<i class="fa-solid fa-location-dot fa-2x" aria-hidden="true"></i>
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
		margin: 2rem auto;
		padding: 0 1rem;
		font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
		box-sizing: border-box;
	}

	.contact-header {
		text-align: center;
		margin-bottom: 2rem;
	}

	.contact-header h1 {
		font-size: clamp(1.8rem, 5vw, 2.5rem);
		margin-bottom: 0.5rem;
		line-height: 1.2;
	}

	.contact-subtitle {
		font-size: clamp(0.9rem, 3vw, 1.1rem);
		font-style: italic;
		color: #6c757d;
	}

	.contact-container {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(min(100%, 300px), 1fr));
		gap: 1.5rem;
		margin: 2rem 0;
	}

	.contact-card {
		border-radius: 10px;
		padding: 1.25rem;
		box-shadow: 0 3px 10px rgba(250, 250, 250, 0.08);
		display: flex;
		align-items: center;
		gap: 1.25rem;
		transition: all 0.3s ease;
		background: none;
	}

	.contact-card:hover {
		transform: translateY(-5px);
		box-shadow: 0 10px 20px rgba(250, 250, 250, 0.1);
	}

	.contact-icon {
		background: #f8f9fa;
		width: 3.5rem;
		height: 3.5rem;
		min-width: 3.5rem;
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
		word-break: break-all;
	}

	.contact-link:hover {
		color: #4a3dc0;
		text-decoration: underline;
	}

	.contact-text {
		margin: 0;
		color: #6c757d;
	}

	.contact-footer {
		text-align: center;
		margin-top: 3rem;
		color: #6c757d;
		font-size: 0.9rem;
		padding-top: 1.5rem;
		border-top: 1px solid #e9ecef;
	}

	@media (max-width: 600px) {
		.contact-main {
			margin: 1.5rem auto;
			padding: 0 1rem;
		}

		.contact-card {
			flex-direction: column;
			text-align: center;
			gap: 1rem;
			padding: 1.5rem 1rem;
		}

		.contact-info h3 {
			font-size: 1.1rem;
		}
	}

	@media (max-width: 400px) {
		.contact-icon {
			width: 3rem;
			height: 3rem;
			min-width: 3rem;
		}

		.fa-2x {
			font-size: 1.25em;
		}
	}
</style>
