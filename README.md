# WALAHI
WALAHI
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Walahi Bro | IShowSpeed Auto Detailing</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&family=Bangers&family=Poppins:wght@400;600;700;900&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: #0a0a0a;
            color: #fff;
            overflow-x: hidden;
        }
        
        .bg-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 50%, rgba(255, 0, 60, 0.08) 0%, transparent 50%),
                radial-gradient(circle at 80% 50%, rgba(255, 204, 0, 0.05) 0%, transparent 50%);
            z-index: -1;
        }
        
        header {
            background: linear-gradient(180deg, #1a0000, #0a0a0a);
            padding: 1.5rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 2px solid #ff003c;
            flex-wrap: wrap;
        }
        
        .logo {
            font-family: 'Bangers', cursive;
            font-size: 2rem;
            background: linear-gradient(90deg, #ff003c, #ffcc00, #ff003c);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            letter-spacing: 2px;
        }
        
        nav {
            display: flex;
            gap: 1.5rem;
            flex-wrap: wrap;
        }
        
        nav a {
            color: #ffcc00;
            text-decoration: none;
            font-weight: 700;
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            transition: all 0.3s;
        }
        
        nav a:hover {
            color: #ff003c;
        }
        
        .hero {
            text-align: center;
            padding: 5rem 2rem;
            position: relative;
            background: 
                radial-gradient(ellipse at center, rgba(255, 0, 60, 0.1) 0%, transparent 70%);
        }
        
        .hero h1 {
            font-family: 'Bangers', cursive;
            font-size: 5rem;
            background: linear-gradient(90deg, #ff003c, #ffcc00, #ff003c, #ffcc00);
            background-size: 300% 100%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradientShift 3s ease infinite;
            line-height: 1.2;
            text-transform: uppercase;
            margin-bottom: 1rem;
        }
        
        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }
        
        .hero .subtitle {
            font-family: 'Press Start 2P', cursive;
            font-size: 0.7rem;
            color: #ffcc00;
            margin: 1.5rem 0;
            letter-spacing: 3px;
        }
        
        .hero .walahi-bro {
            font-size: 1.8rem;
            color: #ff6680;
            margin-top: 1.5rem;
            font-weight: 900;
        }
        
        .hero .walahi-bro span {
            color: #ffcc00;
        }
        
        .marquee {
            background: #ff003c;
            color: #fff;
            padding: 0.8rem;
            text-align: center;
            font-weight: 700;
            letter-spacing: 2px;
            text-transform: uppercase;
            font-size: 0.85rem;
            overflow: hidden;
            white-space: nowrap;
        }
        
        .marquee span {
            display: inline-block;
            animation: scroll 15s linear infinite;
        }
        
        @keyframes scroll {
            0% { transform: translateX(100%); }
            100% { transform: translateX(-100%); }
        }
        
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 3rem 2rem;
        }
        
        .walahi-section {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .walahi-section h2 {
            font-family: 'Bangers', cursive;
            font-size: 2.5rem;
            color: #ff003c;
            margin-bottom: 0.5rem;
        }
        
        .walahi-section .catchphrase {
            font-size: 1.5rem;
            color: #ffcc00;
            font-weight: 900;
            margin-bottom: 1rem;
        }
        
        .walahi-section p {
            color: #999;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }
        
        .price-card {
            background: linear-gradient(145deg, #1a0a0a, #111);
            border: 2px solid #ff003c;
            border-radius: 16px;
            padding: 2.5rem;
            text-align: center;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }
        
        .price-card:hover {
            transform: translateY(-8px);
            border-color: #ffcc00;
            box-shadow: 0 0 40px rgba(255, 0, 60, 0.3);
        }
        
        .price-card.popular {
            border-color: #ffcc00;
        }
        
        .price-card .popular-badge {
            position: absolute;
            top: 15px;
            right: -35px;
            background: #ffcc00;
            color: #000;
            padding: 0.3rem 2rem;
            font-size: 0.6rem;
            font-weight: 700;
            letter-spacing: 1px;
            transform: rotate(45deg);
        }
        
        .price-card .emoji {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .price-card h3 {
            font-family: 'Bangers', cursive;
            font-size: 1.5rem;
            color: #ffcc00;
            margin-bottom: 1rem;
        }
        
        .price-card .price {
            font-size: 3.5rem;
            font-weight: 900;
            color: #ff003c;
            margin: 1rem 0;
        }
        
        .price-card ul {
            list-style: none;
            padding: 0;
            text-align: left;
            margin: 1.5rem 0;
        }
        
        .price-card li {
            padding: 0.5rem 0;
            padding-left: 1.5rem;
            position: relative;
            color: #999;
            font-size: 0.9rem;
            border-bottom: 1px solid #222;
        }
        
        .price-card li::before {
            content: 'WALAHI';
            position: absolute;
            left: 0;
            color: #ff003c;
            font-size: 0.7rem;
            font-weight: 700;
        }
        
        .price-card .btn {
            display: inline-block;
            margin-top: 1rem;
            padding: 0.8rem 2rem;
            background: #ff003c;
            color: #fff;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 700;
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s;
        }
        
        .price-card .btn:hover {
            background: #ffcc00;
            color: #000;
            transform: scale(1.05);
        }
        
        .walahi-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-bottom: 3rem;
        }
        
        .walahi-card {
            background: linear-gradient(145deg, #1a0a0a, #111);
            border: 2px solid #ff003c;
            border-radius: 16px;
            padding: 2rem;
            text-align: center;
            transition: all 0.3s;
        }
        
        .walahi-card:hover {
            transform: translateY(-5px);
            border-color: #ffcc00;
            box-shadow: 0 0 30px rgba(255, 0, 60, 0.3);
        }
        
        .walahi-card .emoji {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .walahi-card h3 {
            font-family: 'Bangers', cursive;
            font-size: 1.2rem;
            color: #ffcc00;
            margin-bottom: 0.5rem;
        }
        
        .walahi-card p {
            color: #999;
            font-size: 0.85rem;
        }
        
        .review-strip {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1rem;
            margin-bottom: 3rem;
        }
        
        .review-mini {
            background: #111;
            border-left: 3px solid #ff003c;
            padding: 1.2rem;
            border-radius: 0 8px 8px 0;
        }
        
        .review-mini .stars {
            color: #ffcc00;
            font-size: 0.8rem;
            margin-bottom: 0.5rem;
        }
        
        .review-mini p {
            color: #999;
            font-size: 0.85rem;
            font-style: italic;
        }
        
        .review-mini .name {
            color: #ff6680;
            font-weight: 600;
            margin-top: 0.5rem;
            font-size: 0.8rem;
        }
        
        .chat-box {
            max-width: 600px;
            margin: 3rem auto;
            background: #111;
            border: 2px solid #333;
            border-radius: 16px;
            overflow: hidden;
        }
        
        .chat-header {
            background: linear-gradient(90deg, #ff003c, #ff6600);
            padding: 1rem;
            font-weight: 700;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .chat-header span {
            font-family: 'Press Start 2P', cursive;
            font-size: 0.6rem;
            color: #fff;
        }
        
        .chat-messages {
            padding: 1.5rem;
            max-height: 300px;
            overflow-y: auto;
        }
        
        .chat-message {
            margin-bottom: 1rem;
            padding: 0.8rem 1rem;
            border-radius: 12px;
            background: #1a1a1a;
            border-left: 3px solid #333;
        }
        
        .chat-message.speed {
            border-left-color: #ff003c;
            background: #1a0000;
        }
        
        .chat-message .username {
            color: #ff003c;
            font-weight: 700;
            font-size: 0.85rem;
            margin-bottom: 0.3rem;
        }
        
        .chat-message .text {
            color: #ccc;
            font-size: 0.9rem;
        }
        
        .chat-message .text .walahi {
            color: #ff003c;
            font-weight: 700;
        }
        
        .contact-section {
            background: linear-gradient(145deg, #1a0a0a, #111);
            border: 2px solid #ff003c;
            border-radius: 16px;
            padding: 3rem;
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .contact-section h2 {
            font-family: 'Bangers', cursive;
            font-size: 2.5rem;
            color: #ffcc00;
            margin-bottom: 2rem;
        }
        
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            text-align: center;
        }
        
        .contact-item .icon {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }
        
        .contact-item h4 {
            color: #ffcc00;
            margin-bottom: 0.5rem;
            font-family: 'Bangers', cursive;
            font-size: 1.2rem;
        }
        
        .contact-item a {
            color: #ff003c;
            text-decoration: none;
            font-weight: 700;
            font-size: 1rem;
        }
        
        .contact-item a:hover {
            text-decoration: underline;
        }
        
        .walahi-banner {
            background: linear-gradient(90deg, #ff003c, #ff6600, #ffcc00);
            padding: 2rem;
            text-align: center;
            border-radius: 16px;
            margin-bottom: 3rem;
        }
        
        .walahi-banner h3 {
            font-family: 'Bangers', cursive;
            font-size: 2rem;
            color: #000;
            margin-bottom: 0.5rem;
        }
        
        .walahi-banner p {
            color: #000;
            font-weight: 700;
            font-size: 1.2rem;
        }
        
        footer {
            background: #000;
            text-align: center;
            padding: 2rem;
            border-top: 2px solid #ff003c;
        }
        
        footer p {
            color: #666;
            font-size: 0.85rem;
        }
        
        footer .walahi-footer {
            font-family: 'Bangers', cursive;
            font-size: 1.5rem;
            color: #ff003c;
            margin-bottom: 1rem;
        }
        
        @media (max-width: 600px) {
            .hero h1 {
                font-size: 3rem;
            }
            header {
                flex-direction: column;
                gap: 1rem;
            }
            nav a {
                margin: 0 0.5rem;
                font-size: 0.75rem;
            }
        }
    </style>
</head>
<body>
    <div class="bg-animation"></div>
    
    <header>
        <div class="logo">WALAHI BRO</div>
        <nav>
            <a href="#pricing">Pricing</a>
            <a href="#services">Services</a>
            <a href="#reviews">Reviews</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <div class="hero">
        <h1>WALAHI</h1>
        <p class="subtitle">◈ AUTO DETAILING ◈</p>
        <div class="walahi-bro">
            <span>Walahi Bro, Say Walahi!</span>
        </div>
        <p style="color: #999; margin-top: 1rem; font-size: 1rem;">
            The #1 Walahi-themed auto care in Queen Creek 🚗✨
        </p>
    </div>

    <div class="marquee">
        <span>⚡ WALAHI BRO SAY WALAHI ⚡ WALAHI AUTO DETAILING ⚡ $60 CAR WASH ⚡ $120 DETAIL ⚡ $180 DELUXE DETAIL ⚡ WALK-INS WELCOME ⚡ WALAHI ⚡</span>
    </div>

    <div class="container">
        <div class="walahi-banner">
            <h3>⚡ WALAHI BRO SAY WALAHI ⚡</h3>
            <p>Premium Auto Care That Hits Different</p>
        </div>

        <section id="pricing">
            <div class="walahi-section">
                <h2>🔥 WALAHI PRICING 🔥</h2>
                <div class="catchphrase">Say Walahi Before You Book, Bro!</div>
            </div>
            
            <div class="pricing-grid">
                <div class="price-card">
                    <div class="emoji">🚿</div>
                    <h3>Car Wash</h3>
                    <div class="price">$60</div>
                    <ul>
                        <li>Exterior hand wash</li>
                        <li>Tire & rim cleaning</li>
                        <li>Window cleaning</li>
                        <li>Detailing spray finish</li>
                        <li>Door jamb wipe</li>
                    </ul>
                    <a href="tel:6028819996" class="btn">Book Walahi Bro</a>
                </div>

                <div class="price-card popular">
                    <div class="popular-badge">WALAHI</div>
                    <div class="emoji">✨</div>
                    <h3>Detail</h3>
                    <div class="price">$120</div>
                    <ul>
                        <li>Everything in Car Wash</li>
                        <li>Full exterior polish</li>
                        <li>Interior deep clean</li>
                        <li>Vacuum & shampoo</li>
                        <li>Dashboard care</li>
                        <li>Leather conditioning</li>
                    </ul>
                    <a href="tel:6028819996" class="btn">Book Walahi Bro</a>
                </div>

                <div class="price-card">
                    <div class="emoji">🔥</div>
                    <h3>Deluxe Detail</h3>
                    <div class="price">$180</div>
                    <ul>
                        <li>Everything in Detail</li>
                        <li>Engine bay cleaning</li>
                        <li>Clay bar treatment</li>
                        <li>Paint sealant</li>
                        <li>Headlight restore</li>
                        <li>Odor elimination</li>
                        <li>Ceramic shine</li>
                    </ul>
                    <a href="tel:6028819996" class="btn">Book Walahi Bro</a>
                </div>
            </div>
        </section>

        <div class="walahi-section">
            <h2>⚡ WALAHI SERVICES ⚡</h2>
            <div class="catchphrase">Say Walahi To These Services, Bro!</div>
        </div>
        
        <div class="walahi-cards">
            <div class="walahi-card">
                <div class="emoji">🧽</div>
                <h3>Clay Bar</h3>
                <p>Walahi smooth paint finish</p>
            </div>
            <div class="walahi-card">
                <div class="emoji">💎</div>
                <h3>Ceramic Coating</h3>
                <p>Long-lasting Walahi protection</p>
            </div>
            <div class="walahi-card">
                <div class="emoji">🛞</div>
                <h3>Wheel Detail</h3>
                <p>Make those rims Walahi clean</p>
            </div>
            <div class="walahi-card">
                <div class="emoji">💨</div>
                <h3>Odor Removal</h3>
                <p>No more Walahi smells bro</p>
            </div>
            <div class="walahi-card">
                <div class="emoji">🔦</div>
                <h3>Headlight Restore</h3>
                <p>Crystal clear Walahi shine</p>
            </div>
            <div class="walahi-card">
                <div class="emoji">🏎️</div>
                <h3>Paint Correction</h3>
                <p>Fix swirls Walahi style</p>
            </div>
        </div>

        <div class="chat-box">
            <div class="chat-header">
                <span>WALAHICHAT</span>
                <span>🔴 LIVE</span>
            </div>
            <div class="chat-messages">
                <div class="chat-message speed">
                    <div class="username">IShowSpeed</div>
                    <div class="text">Walahi bro say Walahi! This car detailing is <span class="walahi">WALAHI</span> 🔥🔥🔥</div>
                </div>
                <div class="chat-message">
                    <div class="username">Fan_123</div>
                    <div class="text">Walahi bro this place is insane! My truck looks <span class="walahi">WALAHI</span> clean</div>
                </div>
                <div class="chat-message speed">
                    <div class="username">IShowSpeed</div>
                    <div class="text">Say Walahi if you love clean cars! <span class="walahi">WALAHI</span> ⚡</div>
                </div>
                <div class="chat-message">
                    <div class="username">SpeedFan</div>
                    <div class="text">Walahi bro booked the deluxe detail. Can't wait! 🚗✨</div>
                </div>
                <div class="chat-message speed">
                    <div class="username">IShowSpeed</div>
                    <div class="text">$180 deluxe detail hits different bro. Say Walahi! <span class="walahi">WALAHI</span> 🏎️</div>
                </div>
            </div>
        </div>

        <section id="reviews">
            <div class="walahi-section">
                <h2>⭐ WALAHIBRO REVIEWS ⭐</h2>
                <div class="catchphrase">What People Say About Walahi Auto Care</div>
            </div>
            
            <div class="review-strip">
                <div class="review-mini">
                    <div class="stars">★★★★★</div>
                    <p>"Walahi bro this place is 🔥 My truck looks brand new after deluxe detail!"</p>
                    <div class="name">— Robert H.</div>
                </div>
                <div class="review-mini">
                    <div class="stars">★★★★★</div>
                    <p>"Best $120 I ever spent. Interior detail is Walahi clean!"</p>
                    <div class="name">— Ashley R.</div>
                </div>
                <div class="review-mini">
                    <div class="stars">★★★★★</div>
                    <p>"Quick car wash, Walahi thorough. Coming back every month!"</p>
                    <div class="name">— David K.</div>
                </div>
                <div class="review-mini">
                    <div class="stars">★★★★</div>
                    <p>"Took a bit longer but final result was Walahi worth it!"</p>
                    <div class="name">— Jennifer P.</div>
                </div>
                <div class="review-mini">
                    <div class="stars">★★★★★</div>
                    <p>"Ceramic coating they applied is Walahi unreal. My car glows!"</p>
                    <div class="name">— Tiffany L.</div>
                </div>
                <div class="review-mini">
                    <div class="stars">★★★★★</div>
                    <p>"Third time here. Consistent Walahi quality every visit. Say Walahi!"</p>
                    <div class="name">— Marcus T.</div>
                </div>
            </div>
        </section>

        <section id="contact">
            <div class="contact-section">
                <h2>📞 WALAHIBRO CONTACT 📞</h2>
                <div class="contact-grid">
                    <div class="contact-item">
                        <div class="icon">📞</div>
                        <h4>Call Walahi Bro</h4>
                        <a href="tel:6028819996">602-881-9996</a>
                        <p style="color: #666; font-size: 0.8rem; margin-top: 0.5rem;">Tap to call</p>
                    </div>
                    <div class="contact-item">
                        <div class="icon">📧</div>
                        <h4>Email Walahi Bro</h4>
                        <a href="mailto:ewhitehad@asuprep.org">ewhitehad@asuprep.org</a>
                        <p style="color: #666; font-size: 0.8rem; margin-top: 0.5rem;">Tap to email</p>
                    </div>
                    <div class="contact-item">
                        <div class="icon">📍</div>
                        <h4>Visit Walahi Bro</h4>
                        <p>22332 E Calle de Flores<br>Queen Creek, AZ 85142</p>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <footer>
        <div class="walahi-footer">⚡ WALAHI BRO SAY WALAHI ⚡</div>
        <p>© 2026 Walahi Auto Detailing. All rights reserved.</p>
    </footer>
</body>
</html>
