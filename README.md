# THE-WAFFLE-BUZZ
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>THE WAFFLE BUZZ</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-color: #d2691e; /* Brown color */
            color: white;
            padding: 1rem;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #ffd700; /* Yellow */
        }
        nav a {
            color: #333;
            padding: 0.5rem 1rem;
            text-decoration: none;
            font-weight: bold;
        }
        nav a:hover {
            background-color: #d2691e;
            color: white;
        }
        .hero {
            background-image: url('https://via.placeholder.com/1200x400?text=Waffles+Here!'); /* Replace with your image URL */
            background-size: cover;
            height: 400px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
        }
        .hero h1 {
            font-size: 3rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }
        section {
            padding: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        .menu {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1rem;
        }
        .menu-item {
            background-color: white;
            border-radius: 8px;
            padding: 1rem;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .menu-item h3 {
            color: #d2691e;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1rem;
        }
        @media (max-width: 768px) {
            nav {
                flex-direction: column;
            }
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>THE WAFFLE BUZZ</h1>
        <p>Your go-to spot for crispy, delicious waffles!</p>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="home" class="hero">
        <div>
            <h1>Welcome to THE WAFFLE BUZZ!</h1>
            <p>Indulge in our mouth-watering waffles, made fresh daily. Buzzing with flavor!</p>
        </div>
    </section>
    <section id="menu">
        <h2>Our Menu</h2>
        <div class="menu">
            <div class="menu-item">
                <h3>Classic Waffle</h3>
                <p>Golden waffle with butter and syrup. ₹150</p>
            </div>
            <div class="menu-item">
                <h3>Chocolate Waffle</h3>
                <p>Loaded with chocolate chips and whipped cream. ₹200</p>
            </div>
            <div class="menu-item">
                <h3>Fruit Waffle</h3>
                <p>Fresh strawberries, bananas, and honey. ₹180</p>
            </div>
            <div class="menu-item">
                <h3>Nutty Waffle</h3>
                <p>With almonds, walnuts, and maple syrup. ₹220</p>
            </div>
        </div>
    </section>
    <section id="contact">
        <h2>Contact Us</h2>
        <p>Address: [Your Shop Address, e.g., 123 Waffle Street, City]</p>
        <p>Phone: [Your Phone Number]</p>
        <p>Email: info@thewafflebuzz.com</p>
        <p>Hours: Mon-Sun: 9 AM - 9 PM</p>
    </section>
    <footer>
        <p>&copy; 2023 THE WAFFLE BUZZ. All rights reserved.</p>
    </footer>
    <script>
        // Simple menu toggle for mobile (if needed)
        const nav = document.querySelector('nav');
        nav.addEventListener('click', (e) => {
            if (e.target.tagName === 'A') {
                // Smooth scroll to section
                const target = document.querySelector(e.target.getAttribute('href'));
                target.scrollIntoView({ behavior: 'smooth' });
            }
        });
    </script>
</body>
</html>
