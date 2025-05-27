<main class="results-main">
	<header class="results-header">
		<h1><span>K.C.S.E Performance 📊</span></h1>
		<p class="results-subtitle">Holo Secondary School's Historical Examination Results</p>
	</header>

	<div class="results-container">
		<div class="results-card">
			<div class="results-icon">
				<i class="fa-solid fa-trophy"></i>
			</div>
			<div class="results-content">
				<h2>Past Examination Results</h2>
				<p>
					Access our complete K.C.S.E performance records dating back several years. These documents
					showcase our consistent academic excellence.
				</p>

				<div class="download-section">
					<a href="/kcse_results.pdf" class="download-btn" target="_blank" download>
						<i class="fa-solid fa-file-arrow-down"></i> Download Results
					</a>
					<span class="file-info">PDF, 1.2MB</span>
				</div>
			</div>
		</div>
	</div>
</main>

<style>
	p {
		font-style: italic;
	}
	.results-main {
		max-width: 800px;
		margin-bottom: 4rem;
		display: block;
		margin: auto;
		padding: 0 0.5rem;
		font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
	}

	.results-header {
		text-align: center;
		margin-bottom: 3rem;
	}

	.results-header h1 {
		font-size: 2.5rem;
		margin-bottom: 0.5rem;
	}

	.results-subtitle {
		color: #7f8c8d;
		font-size: 1.1rem;
	}

	.results-container {
		background: white;
		border-radius: 10px;
		box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
		overflow: hidden;
	}

	.results-card {
		display: flex;
		padding: 0.5rem;
		gap: 2rem;
		align-items: center;
		background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%);
	}

	.results-icon {
		background: #e67e22;
		color: white;
		width: 70px;
		height: 70px;
		border-radius: 50%;
		display: flex;
		align-items: center;
		justify-content: center;
		font-size: 1.8rem;
		flex-shrink: 0;
	}

	.results-content h2 {
		color: #2c3e50;
		margin-top: 0;
	}

	.results-content p {
		color: #636e72;
		line-height: 1.6;
		font-style: italic;
	}

	.download-section {
		margin-top: 1.5rem;
		display: flex;
		align-items: center;
		gap: 1rem;
	}

	.download-btn {
		background: #e67e22;
		color: white;
		padding: 0.8rem 1.5rem;
		border-radius: 5px;
		text-decoration: none;
		font-weight: 600;
		transition: all 0.3s ease;
		display: inline-flex;
		align-items: center;
		gap: 0.5rem;
	}

	.download-btn:hover {
		background: #d35400;
		transform: translateY(-2px);
	}

	.file-info {
		color: #7f8c8d;
		font-size: 0.9rem;
	}

	@media (max-width: 768px) {
		.results-card {
			flex-direction: column;
			text-align: center;
		}

		.download-section {
			justify-content: center;
		}
	}
</style>
