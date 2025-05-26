<main class="board-main">
    <header class="board-header">
        <h1 style="color: aliceblue;"> <span>School Leadership 📋</span></h1>
        <p class="subtitle">Honoring those who have guided our institution</p>
    </header>

    <div class="board-container">
        <section class="board-section">
            <div class="section-header">
                <div class="icon-box">👨‍🏫</div>
                <h2>Principals</h2>
            </div>
            <ul class="timeline-list">
                <li><span2 class="year">1980-1986</span2> Mr. Charles Anang'a Okolo</li>
                <li><span2 class="year">1987-1989</span2> Mr. Patric Adu</li>
                <li><span2 class="year">1990</span2> Mr. Alaro Nyaranga</li>
                <li><span2 class="year">1990-1991</span2> Mr. Ogara Amoko</li>
                <li><span2 class="year">1992-1993</span2> Mr. Simidi John</li>
                <li><span2 class="year">1994-1995</span2> Mr. Otieno Gogo</li>
                <li><span2 class="year">1996-2001</span2> Mr. Leonard Odera</li>
                <li><span2 class="year">2001</span2> Mr. Douglas Otieno</li>
                <li><span2 class="year">2001-2007</span2> Mr. Paul Mbara</li>
                <li><span2 class="year">2007-2011</span2> Mr. Jared Ochieng Obong'o</li>
                <li><span2 class="year">2012-2019</span2> Mr. Amos Awiti</li>
                <li><span2 class="year">2019-2023</span2> Mr. Kenneth Y.A</li>
                <li><span2 class="year">2023-present</span2> Mr. Peter Ogutu</li>
            </ul>
        </section>

        <section class="board-section">
            <div class="section-header">
                <div class="icon-box">👨‍💼</div>
                <h2>B.O.M Chairs</h2>
            </div>
            <ul class="timeline-list">
                <li><span2 class="year">1981-1985</span2> Mr. Steven Oketch Tambo</li>
                <li><span2 class="year">1981-1985</span2> Mr. Ishmael N. Nyagowa Tambo</li>
                <li><span2 class="year">1985-1990</span2> Mr. Steven Oketch Tambo</li>
                <li><span2 class="year">1991</span2> Mr. Simeon Gori Tambo</li>
                <li><span2 class="year">1991-2005</span2> Eng. Haggai Oketch Tambo</li>
                <li><span2 class="year">2005-2007</span2> Rev. Moses T.A Oketch</li>
                <li><span2 class="year">2011-2019</span2> Eng. Tobias Edwin Juma Ojwang</li>
                <li><span2 class="year">2019-present</span2> Eng. Bishop Jackton Okumu</li>
            </ul>
        </section>
    </div>
</main>

<style>
    .board-main {
        margin: 4rem auto;
        max-width: 1200px;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        /* color: #333; */
    }

    .board-header {
        text-align: center;
        margin-bottom: 3rem;
    }

    .board-header h1 {
        font-size: 2.5rem;
        margin-bottom: 0.5rem;
    }


    .subtitle {
        color: #7f8c8d;
        font-size: 1.1rem;
        font-style: italic;
    }

    .board-container {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        gap: 2rem;
    }

    .board-section {
        flex: 1;
        min-width: 300px;
        /* background: white; */
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(250, 250, 250, 0.1);
        padding: 1.5rem;
        transition: transform 0.3s ease;
    }

    .board-section:hover {
        transform: translateY(-5px);
    }

    .section-header {
        display: flex;
        align-items: center;
        gap: 1rem;
        margin-bottom: 1.5rem;
        padding-bottom: 0.5rem;
        border-bottom: 2px solid #00C9A7;
    }

    .icon-box {
        background: #00C9A7;
        color: white;
        width: 40px;
        height: 40px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 1.2rem;
    }

    .board-section h2 {
        margin: 0;
    }

    .timeline-list {
        list-style: none;
        padding: 0;
        margin: 0;
        padding-left: 1.5rem;
    }

    .timeline-list li {
        padding: 0.7rem 0;
        position: relative;
        line-height: 1.4;
    }

    .timeline-list li:before {
        content: '';
        position: absolute;
        left: -1.7rem;
        top: 1.2rem;
        width: 10px;
        height: 10px;
        background: #00C9A7;
        border-radius: 50%;
    }

    .year {
        display: inline-block;
        width: 80px;
        color: #00C9A7;
        font-weight: 600;
    }

    @media (max-width: 768px) {
        .board-container {
            flex-direction: column;
        }
        
        .board-section {
            min-width: 100%;
        }
    }
</style>