<main class="mission-main">
    <header class="mission-header">
        <h1><span>Our Guiding Principles ✨</span></h1>
        <p class="mission-subtitle">The foundation of our educational philosophy</p>
    </header>

    <div class="mission-grid">
        <article class="mission-card motto-card">
            <h2>Motto <span2 class="card-icon">🏆</span2>
            </h2>
            <div class="card-content">
                <p class="highlight-phrase">"Excellence is a virtue"</p>
            </div>
        </article>

        <article class="mission-card vision-card">
            <h2>Vision <span2 class="card-icon">👁️</span2></h2>
            <div class="card-content">
                <p>To be a school of choice for all-round excellence</p>
            </div>
        </article>

        <article class="mission-card mission-card">
            <h2>Mission <span2 class="card-icon">🎯</span2></h2>
            <div class="card-content">
                <p>To provide students with academic and life skills for the good of mankind</p>
            </div>
        </article>

        <article class="mission-card values-card">
            <h2>Core Values <span2 class="card-icon">❤️</span2></h2>
            <div class="card-content">
                <ul class="values-list">
                    <li><span2 class="value-icon">🙏</span2> Prayer</li>
                    <li><span2 class="value-icon">🌱</span2> Holistic Education</li>
                    <li><span2 class="value-icon">📈</span2> Continuous Improvement</li>
                    <li><span2 class="value-icon">👥</span2> Teamwork</li>
                    <li><span2 class="value-icon">💡</span2> Innovation</li>
                    <li><span2 class="value-icon">🛡️</span2> Integrity</li>
                </ul>
            </div>
        </article>
    </div>
</main>

<style>
    .mission-main {
        max-width: 1200px;
        margin: 4rem auto;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    .mission-header {
        text-align: center;
        margin-bottom: 3rem;
    }

    .mission-header h1 {
        font-size: 2.5rem;
        margin-bottom: 0.5rem;
    }


    .mission-subtitle {
        color: #7f8c8d;
        font-size: 1.1rem;
        font-style: italic;
    }

    .mission-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        gap: 2rem;
    }

    .mission-card {
        border-radius: 12px;
        padding: 2rem;
        box-shadow: 0 5px 15px rgba(250, 250, 250, 0.08);
        transition: all 0.3s ease;
        border-top: 4px solid;
    }

    .mission-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 25px rgba(250, 250, 250, 0.12);
    }

    .motto-card {
        border-color: #00b894;
    }

    .vision-card {
        border-color: #0984e3;
    }

    .mission-card.mission-card {
        border-color: #00C9A7;
    }

    .values-card {
        border-color: #e84393;
    }

    .card-icon {
        font-size: 2rem;
        margin-bottom: 1rem;
    }

    .mission-card h2 {
        margin-top: 0;
        margin-bottom: 1.5rem;
        font-size: 1.5rem;
    }

    .highlight-phrase {
        font-size: 1.3rem;
        font-weight: 600;
        color: #00b894;
        font-style: italic;
    }

    .values-list {
        list-style: none;
        padding: 0;
        margin: 0;
    }

    .values-list li {
        padding: 0.5rem 0;
        display: flex;
        align-items: center;
        gap: 0.8rem;
    }

    .value-icon {
        font-size: 1.2rem;
    }

    @media (max-width: 768px) {
        .mission-grid {
            grid-template-columns: 1fr;
        }
        
        .mission-header h1 {
            font-size: 2rem;
        }
    }
</style>