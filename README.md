# Alusine-Fofanah-905005535
#WebDesign Assignment 1 Repository 

##Home Page - Sketch and Wireframe
![Home Page Hand Sketch](https://github.com/user-attachments/assets/07f013d7-25f7-4568-8884-f118d1c25f2a)
<img width="1125" height="1286" alt="Home Page Wireframe" src="https://github.com/user-attachments/assets/5c163920-57a2-4548-90c5-31a8e8c55b3d" />
##Players Page - Sketch and Wireframe
![Players Page Hand Sketch](https://github.com/user-attachments/assets/4da971fd-aff1-4984-994d-e3feb1a03597)
<img width="1125" height="1286" alt="Players Page Wireframe" src="https://github.com/user-attachments/assets/293867c3-b94a-4893-856d-f78c6472957c" />
##Matces Page - Sketch and Wireframe
![Matches Page Hand Sketch](https://github.com/user-attachments/assets/17fe7d33-aa9b-4d9c-96a6-68be76db42c7)
<img width="1135" height="1636" alt="Matches Page Wireframe" src="https://github.com/user-attachments/assets/2593dd6f-50ed-401b-9a77-521af39cb17e" />
##About Us Page - Sketch and Wireframe
![About Us Page Hand Sketch](https://github.com/user-attachments/assets/e02e686b-5f97-4902-85c1-e3a9baee858e)
<img width="1125" height="1388" alt="About Us Page Wireframe" src="https://github.com/user-attachments/assets/72e11d2e-9ffb-414a-a3a2-c48a998ff3d2" />
##Contact Page -Sketch and Wireframe
![Contact Page Hand Sketch](https://github.com/user-attachments/assets/f3f85893-d28f-49a8-9fc4-381f7a00bd20)
<img width="1125" height="1449" alt="Contact Page Wireframe" src="https://github.com/user-attachments/assets/486aeef3-322a-43b3-a481-7cd27d27b111" />

#FOOTBALL AGENCY SIERRA LEONE - HTML AND CSS CODE
##style.css - cod/* styles.css - Football Agency Sierra Leone */

/* Reset and Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
    background: #f4f4f4;
}

/* Sierra Leone Colors */
:root {
    --sl-green: #1EB53A;
    --sl-white: #FFFFFF;
    --sl-blue: #0072C6;
    --dark-green: #158230;
    --light-green: #e8f5e9;
    --text-dark: #2c3e50;
}

/* Header Styles */
.header {
    background: linear-gradient(135deg, var(--sl-green) 0%, var(--dark-green) 100%);
    color: var(--sl-white);
    padding: 0;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.header-top {
    background: var(--dark-green);
    padding: 10px 0;
    font-size: 14px;
}

.header-top .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.contact-info span {
    margin-right: 20px;
}

.header-main {
    padding: 20px 0;
}

.header-main .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    display: flex;
    align-items: center;
    gap: 15px;
}

.logo-img {
    width: 60px;
    height: 60px;
    background: var(--sl-white);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    border: 3px solid var(--sl-blue);
}

.logo-img img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.logo-text h1 {
    font-size: 24px;
    font-weight: 700;
}

.logo-text p {
    font-size: 12px;
    opacity: 0.9;
}

/* Navigation */
.nav-menu {
    display: flex;
    list-style: none;
    gap: 5px;
}

.nav-menu li a {
    color: var(--sl-white);
    text-decoration: none;
    padding: 12px 25px;
    display: block;
    font-weight: 600;
    border-radius: 5px;
    transition: all 0.3s ease;
}

.nav-menu li a:hover,
.nav-menu li a.active {
    background: var(--sl-blue);
    transform: translateY(-2px);
}

/* Container */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, var(--sl-blue) 0%, var(--sl-green) 100%);
    color: var(--sl-white);
    padding: 80px 20px;
    text-align: center;
    position: relative;
    overflow: hidden;
}

.hero::before {
    content: '';
    position: absolute;
    width: 2000px;
    height: 500px;
    background-image: url('../IMAGES/team-background.jpg.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    opacity: 0.15;
    top: -50px;
    right: -50px;
    border-radius: 10px;
}

.hero h1 {
    font-size: 48px;
    margin-bottom: 20px;
    animation: fadeInDown 1s;
}

.hero p {
    font-size: 20px;
    max-width: 800px;
    margin: 0 auto;
    line-height: 1.8;
    animation: fadeInUp 1s;
}

/* Stats Bar */
.stats-bar {
    background: var(--sl-white);
    padding: 40px 20px;
    margin: -30px auto 40px;
    max-width: 1100px;
    border-radius: 10px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.1);
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 30px;
    position: relative;
    z-index: 10;
}

.stat-item {
    text-align: center;
    padding: 20px;
    border-right: 2px solid var(--light-green);
}

.stat-item:last-child {
    border-right: none;
}

.stat-number {
    font-size: 48px;
    font-weight: 700;
    color: var(--sl-green);
    display: block;
    margin-bottom: 10px;
}

.stat-label {
    font-size: 16px;
    color: var(--text-dark);
    font-weight: 600;
}

/* Section Styles */
.section {
    padding: 60px 20px;
}

.section-title {
    font-size: 36px;
    text-align: center;
    margin-bottom: 40px;
    color: var(--sl-green);
    position: relative;
    padding-bottom: 15px;
}

.section-title::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 80px;
    height: 4px;
    background: var(--sl-blue);
    border-radius: 2px;
}

/* Search Box */
.search-container {
    max-width: 600px;
    margin: 0 auto 40px;
}

.search-box {
    display: flex;
    gap: 10px;
    background: var(--sl-white);
    padding: 10px;
    border-radius: 10px;
    box-shadow: 0 3px 15px rgba(0,0,0,0.1);
}

.search-box input {
    flex: 1;
    padding: 12px 20px;
    border: 2px solid #ddd;
    border-radius: 5px;
    font-size: 16px;
}

.search-box input:focus {
    outline: none;
    border-color: var(--sl-green);
}

.search-box select {
    padding: 12px 20px;
    border: 2px solid #ddd;
    border-radius: 5px;
    font-size: 16px;
    min-width: 150px;
}

.search-box button {
    padding: 12px 30px;
    background: var(--sl-green);
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-weight: 600;
}

.search-box button:hover {
    background: var(--dark-green);
}

/* Card Grid */
.card-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
    margin-top: 40px;
}

.card {
    background: var(--sl-white);
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
}

.card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.2);
}

.card-img {
    width: 100%;
    height: 250px;
    overflow: hidden;
    background: #f0f0f0;
    display: flex;
    align-items: center;
    justify-content: center;
}

.card-img img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.card-content {
    padding: 25px;
}

.card-content h3 {
    font-size: 22px;
    color: var(--sl-green);
    margin-bottom: 10px;
}

.card-content .position {
    color: var(--sl-blue);
    font-weight: 600;
    font-size: 16px;
    margin-bottom: 15px;
}

.card-content p {
    color: #666;
    line-height: 1.6;
    margin: 8px 0;
}

.card-content strong {
    color: var(--text-dark);
}

/* Player Cards */
.player-card {
    background: var(--sl-white);
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
}

.player-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(30, 181, 58, 0.3);
}

.player-img {
    width: 100%;
    height: 300px;
    overflow: hidden;
    background: #f0f0f0;
    display: flex;
    align-items: center;
    justify-content: center;
}

.player-img img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.player-info {
    padding: 20px;
}

.player-info h3 {
    font-size: 24px;
    color: var(--sl-green);
    margin-bottom: 5px;
}

.player-info .position {
    color: var(--sl-blue);
    font-weight: 600;
    font-size: 18px;
    margin-bottom: 15px;
    display: block;
}

.player-details {
    background: var(--light-green);
    padding: 15px;
    border-radius: 5px;
    margin-top: 15px;
}

.player-details p {
    margin: 8px 0;
    font-size: 14px;
}

/* Match Cards */
.match-card {
    background: var(--sl-white);
    border-radius: 10px;
    padding: 30px;
    margin-bottom: 30px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    border-left: 5px solid var(--sl-green);
}

.match-card.upcoming {
    border-left-color: var(--sl-blue);
    background: linear-gradient(135deg, #e3f2fd 0%, var(--sl-white) 100%);
}

.match-badge {
    display: inline-block;
    padding: 8px 20px;
    border-radius: 20px;
    font-weight: 600;
    font-size: 14px;
    margin-bottom: 15px;
}

.match-badge.victory {
    background: var(--sl-green);
    color: var(--sl-white);
}

.match-badge.defeat {
    background: #f44336;
    color: var(--sl-white);
}

.match-badge.draw {
    background: #ff9800;
    color: var(--sl-white);
}

.match-badge.upcoming {
    background: var(--sl-blue);
    color: var(--sl-white);
}

.match-info {
    display: flex;
    justify-content: space-between;
    margin-bottom: 20px;
    font-size: 14px;
    color: #666;
}

.match-score {
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin: 30px 0;
}

.team {
    text-align: center;
    flex: 1;
}

.team-name {
    font-size: 20px;
    font-weight: 700;
    color: var(--text-dark);
    margin-bottom: 10px;
}

.score {
    font-size: 56px;
    font-weight: 700;
    color: var(--sl-green);
}

.match-score .vs {
    font-size: 24px;
    font-weight: 700;
    color: #999;
    padding: 0 30px;
}

.match-details {
    background: var(--light-green);
    padding: 15px;
    border-radius: 5px;
}

.match-details p {
    margin: 5px 0;
}

/* Timeline */
.timeline {
    position: relative;
    max-width: 900px;
    margin: 40px auto;
    padding-left: 50px;
}

.timeline::before {
    content: '';
    position: absolute;
    left: 20px;
    top: 0;
    bottom: 0;
    width: 4px;
    background: var(--sl-green);
}

.timeline-item {
    position: relative;
    margin-bottom: 40px;
    background: var(--sl-white);
    padding: 25px;
    border-radius: 10px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
}

.timeline-item::before {
    content: '';
    position: absolute;
    left: -38px;
    top: 30px;
    width: 20px;
    height: 20px;
    background: var(--sl-blue);
    border: 4px solid var(--sl-white);
    border-radius: 50%;
    box-shadow: 0 0 0 4px var(--light-green);
}

.timeline-item h3 {
    color: var(--sl-green);
    font-size: 20px;
    margin-bottom: 10px;
}

/* Mission/Vision Boxes */
.two-col-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
    gap: 30px;
    margin: 40px 0;
}

.info-box {
    background: var(--sl-white);
    padding: 35px;
    border-radius: 10px;
    border-top: 4px solid var(--sl-green);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.info-box h3 {
    color: var(--sl-green);
    font-size: 24px;
    margin-bottom: 15px;
}

/* Contact Form */
.contact-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 50px;
    margin-top: 40px;
}

.contact-info-section {
    background: var(--sl-white);
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    margin-bottom: 30px;
}

.contact-info-section h3 {
    color: var(--sl-green);
    font-size: 20px;
    margin-bottom: 15px;
}

.contact-form {
    background: var(--sl-white);
    padding: 40px;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.form-group {
    margin-bottom: 25px;
}

.form-group label {
    display: block;
    margin-bottom: 8px;
    color: var(--text-dark);
    font-weight: 600;
}

.form-group input,
.form-group select,
.form-group textarea {
    width: 100%;
    padding: 12px 15px;
    border: 2px solid #ddd;
    border-radius: 5px;
    font-size: 16px;
    transition: all 0.3s ease;
}

.form-group input:focus,
.form-group select:focus,
.form-group textarea:focus {
    outline: none;
    border-color: var(--sl-green);
}

.form-group textarea {
    min-height: 150px;
    resize: vertical;
}

/* Buttons */
.btn {
    display: inline-block;
    padding: 14px 35px;
    background: var(--sl-green);
    color: var(--sl-white);
    text-decoration: none;
    border-radius: 5px;
    font-weight: 600;
    border: none;
    cursor: pointer;
    transition: all 0.3s ease;
    font-size: 16px;
}

.btn:hover {
    background: var(--dark-green);
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(30, 181, 58, 0.3);
}

.btn-blue {
    background: var(--sl-blue);
}

.btn-blue:hover {
    background: #005a9c;
}

/* Map Container */
.map-container {
    width: 100%;
    height: 450px;
    border-radius: 10px;
    overflow: hidden;
    border: 3px solid var(--sl-green);
    margin: 40px 0;
}

.map-container iframe {
    width: 100%;
    height: 100%;
    border: 0;
}

/* Social Media */
.social-links {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
    margin: 40px 0;
}

.social-link {
    background: var(--sl-white);
    padding: 20px 35px;
    border-radius: 10px;
    text-decoration: none;
    color: var(--text-dark);
    font-weight: 600;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
}

.social-link:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.2);
    background: var(--sl-green);
    color: var(--sl-white);
}

/* Footer */
.footer {
    background: linear-gradient(135deg, var(--dark-green) 0%, var(--sl-green) 100%);
    color: var(--sl-white);
    padding: 50px 20px 20px;
    margin-top: 60px;
}

.footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 40px;
    margin-bottom: 30px;
}

.footer-section h3 {
    margin-bottom: 20px;
    font-size: 20px;
}

.footer-section p,
.footer-section ul {
    line-height: 2;
    opacity: 0.9;
}

.footer-section ul {
    list-style: none;
}

.footer-section ul li a {
    color: var(--sl-white);
    text-decoration: none;
    transition: all 0.3s ease;
}

.footer-section ul li a:hover {
    padding-left: 10px;
    color: var(--sl-blue);
}

.footer-bottom {
    text-align: center;
    padding-top: 30px;
    border-top: 1px solid rgba(255,255,255,0.2);
    margin-top: 30px;
}

/* No Results Message */
.no-results {
    text-align: center;
    padding: 40px;
    background: var(--light-green);
    border-radius: 10px;
    margin: 20px 0;
}

.no-results h3 {
    color: var(--sl-green);
    font-size: 24px;
    margin-bottom: 10px;
}

/* Animations */
@keyframes fadeInDown {
    from {
        opacity: 0;
        transform: translateY(-20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Responsive Design */
@media (max-width: 768px) {
    .header-main .container {
        flex-direction: column;
        text-align: center;
    }
    
    .nav-menu {
        flex-direction: column;
        width: 100%;
        margin-top: 20px;
    }
    
    .hero h1 {
        font-size: 32px;
    }
    
    .stats-bar {
        grid-template-columns: 1fr 1fr;
    }
    
    .card-grid {
        grid-template-columns: 1fr;
    }
    
    .contact-grid {
        grid-template-columns: 1fr;
    }
    
    .two-col-grid {
        grid-template-columns: 1fr;
    }
    
    .match-score {
        flex-direction: column;
    }
    
    .match-score .vs {
        margin: 20px 0;
    }

    .search-box {
        flex-direction: column;
    }
}

##index.html - Home Page code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home - Football Agency Sierra Leone</title>
    <link rel="stylesheet" href="../CSS/style.css">
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="header-top">
            <div class="container">
                <div class="contact-info">
                    <span>📧 info@fasl.sl</span>
                    <span>📞 +232 76 123 456</span>
                </div>
                <div class="social-info">
                    <span>Follow Us: Facebook | Twitter | Instagram</span>
                </div>
            </div>
        </div>
        <div class="header-main">
            <div class="container">
                <div class="logo">
                    <div class="logo-img">
                        <img src="../IMAGES/slfa-logo.jpg" alt="FASL Logo">
                    </div>
                    <div class="logo-text">
                        <h1>FASL</h1>
                        <p>Football Agency Sierra Leone</p>
                    </div>
                </div>
                <nav>
                    <ul class="nav-menu">
                        <li><a href="index.html" class="active">HOME</a></li>
                        <li><a href="players.html">PLAYERS</a></li>
                        <li><a href="matches.html">MATCHES</a></li>
                        <li><a href="about.html">ABOUT US</a></li>
                        <li><a href="contact.html">CONTACT</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Welcome to Football Agency Sierra Leone</h1>
            <p>Discover the finest football talent in Sierra Leone. We are dedicated to nurturing, managing, and promoting exceptional football players who represent the pride and passion of our nation. Join us in celebrating the beautiful game and supporting our talented athletes as they pursue excellence on the field.</p>
        </div>
    </section>

    <!-- Statistics Section -->
    <div class="stats-bar">
        <div class="stat-item">
            <span class="stat-number">50+</span>
            <span class="stat-label">Active Players</span>
        </div>
        <div class="stat-item">
            <span class="stat-number">120+</span>
            <span class="stat-label">Matches Played</span>
        </div>
        <div class="stat-item">
            <span class="stat-number">15+</span>
            <span class="stat-label">Championships</span>
        </div>
        <div class="stat-item">
            <span class="stat-number">8</span>
            <span class="stat-label">Years Experience</span>
        </div>
    </div>

    <!-- Featured Players Section -->
    <section class="section">
        <div class="container">
            <h2 class="section-title">Our Star Players</h2>
            <div class="card-grid">
                <div class="card">
                    <div class="card-img">
                        <img src="../IMAGES/kei.jpg" alt="IMAGES">
                    </div>
                    <div class="card-content">
                        <h3>Kei Kamara</h3>
                        <p class="position">Forward</p>
                        <p><strong>Age:</strong> 24 years</p>
                        <p><strong>Goals:</strong> 45 in 60 matches</p>
                        <p>Known for his speed and exceptional goal-scoring ability.</p>
                    </div>
                </div>

                <div class="card">
                    <div class="card-img">
                        <img src="../IMAGES/tombo.jpg" alt="Tombo">
                    </div>
                    <div class="card-content">
                        <h3>Musa Noah Kamara</h3>
                        <p class="position">Forward</p>
                        <p><strong>Age:</strong> 25 years</p>
                        <p><strong>Assists:</strong> 38 in 70 matches</p>
                        <p>Excellent ball control and vision on the field.</p>
                    </div>
                </div>

                <div class="card">
                    <div class="card-img">
                        <img src="../IMAGES/A-B-Jumah.jpg" alt="Juma Bah">
                    </div>
                    <div class="card-content">
                        <h3>Abdulay Juma Bah</h3>
                        <p class="position">Defender</p>
                        <p><strong>Age:</strong> 28 years</p>
                        <p><strong>Clean Sheets:</strong> 45</p>
                        <p>Strong aerial ability and natural leadership qualities.</p>
                    </div>
                </div>

                <div class="card">
                    <div class="card-img">
                        <img src="../IMAGES/M-N-Kamara.jpg" alt="Mohamed N Kamara">
                    </div>
                    <div class="card-content">
                        <h3>Mohamed N Kamara</h3>
                        <p class="position">Goalkeeper</p>
                        <p><strong>Age:</strong> 29 years</p>
                        <p><strong>Saves:</strong> 320</p>
                        <p>Most experienced goalkeeper with commanding presence.</p>
                    </div>
                </div>
            </div>
            <div style="text-align: center; margin-top: 40px;">
                <a href="players.html" class="btn">View All Players</a>
            </div>
        </div>
    </section>

    <!-- Next Match Section -->
    <section class="section" style="background: #f9f9f9;">
        <div class="container">
            <h2 class="section-title">Upcoming Match</h2>
            <div class="match-card upcoming">
                <span class="match-badge upcoming">NEXT MATCH</span>
                <div class="match-info">
                    <span><strong>Date:</strong> December 5, 2025 - 7:00 PM</span>
                    <span><strong>Venue:</strong> National Stadium, Freetown</span>
                </div>
                <div class="match-score">
                    <div class="team">
                        <div class="team-name">Sierra Leone</div><div class="logo-img"> 
                        <img src="../IMAGES/sl-flag.jpg" alt="FASL Logo">
                    </div>
                        <div style="font-size: 36px; color: #666; margin-top: 20px;">vs</div>
                    </div>
                    <div class="team">
                        <div class="team-name">Ghana</div><div class="logo-img"> 
                        <img src="../IMAGES/ghana.jpg" alt="FASL Logo">
                    </div>
                    </div>
                </div>
                <div class="match-details">
                    <p><strong>Competition:</strong> Africa Cup of Nations Qualifier</p>
                    <p><strong>Tickets:</strong> Available at stadium box office</p>
                </div>
            </div>
            <div style="text-align: center; margin-top: 30px;">
                <a href="matches.html" class="btn btn-blue">View All Matches</a>
            </div>
        </div>
    </section>

    <!-- Why Choose Us Section -->
    <section class="section">
        <div class="container">
            <h2 class="section-title">Why Choose FASL</h2>
            <div class="card-grid">
                <div class="card">
                    <div class="card-img">
                        <img src="images/professional.jpg" alt="Professional Management">
                    </div>
                    <div class="card-content">
                        <h3>Professional Management</h3>
                        <p>Expert player representation with proven track record in local and international transfers.</p>
                    </div>
                </div>

                <div class="card">
                    <div class="card-img">
                        <img src="images/development.jpg" alt="Career Development">
                    </div>
                    <div class="card-content">
                        <h3>Career Development</h3>
                        <p>Comprehensive support for players' growth both on and off the field.</p>
                    </div>
                </div>

                <div class="card">
                    <div class="card-img">
                        <img src="images/network.jpg" alt="Global Network">
                    </div>
                    <div class="card-content">
                        <h3>Global Network</h3>
                        <p>Strong connections with clubs across Africa, Europe, and beyond.</p>
                    </div>
                </div>

                <div class="card">
                    <div class="card-img">
                        <img src="images/youth.jpg" alt="Youth Development">
                    </div>
                    <div class="card-content">
                        <h3>Youth Development</h3>
                        <p>Dedicated programs to identify and nurture young talent from grassroots level.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Advertising Our Jersey -->
    <section class="section">
        <div class="container">
            <h2 class="section-title">Our Jersey</h2>
            <div class="card-grid">
                <div class="card">
                    <div class="card-img">
                        <img src="../IMAGES/SL-home-jersey.jpg" alt="Jersey">
                    </div>
                    <div class="card-content">
                        <h3>Home Jersey</h3>
                        <p>Our Home Jersey. Purchase it for a small amount.</p>
                    </div>
                </div>

            
                <div class="card">
                    <div class="card-img">
                        <img src="../IMAGES/SL-away-jersey.jpg" alt="Jersey">
                    </div>
                    <div class="card-content">
                        <h3>Away Jersey</h3>
                        <p>Our Away Jersey. Purchase it for a small amount.</p>
                    </div>
                </div>

                <div class="card">
                    <div class="card-img">
                        <img src="../IMAGES/SL-jersey.jpg" alt="Jersey">
                    </div>
                    <div class="card-content">
                        <h3>Home and Away Jersey</h3>
                        <p>Our Home and Away Jersey. Purchase it for a small amount.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>About FASL</h3>
                    <p>Football Agency Sierra Leone is dedicated to discovering, developing, and representing the finest football talent in Sierra Leone.</p>
                </div>
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="index.html">Home</a></li>
                        <li><a href="players.html">Players</a></li>
                        <li><a href="matches.html">Matches</a></li>
                        <li><a href="about.html">About Us</a></li>
                        <li><a href="contact.html">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Contact Info</h3>
                    <p>📍 123 Stadium Road, Freetown</p>
                    <p>📞 +232 76 123 456</p>
                    <p>📧 info@fasl.sl</p>
                </div>
                <div class="footer-section">
                    <h3>Follow Us</h3>
                    <p>Facebook: @FASLOfficial</p>
                    <p>Twitter: @FASL_SL</p>
                    <p>Instagram: @footballagencysl</p>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 Football Agency Sierra Leone. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
web design repo and wireframe



                                                              

