# MatthewMaree.github.io
Elvian Intelligence website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elvian Intelligence - IoT & AIoT Solutions</title>
    <style>
        /* Global Styles */
        :root {
            --primary-color: #1a237e;
            --secondary-color: #3949ab;
            --accent-color: #00bcd4;
            --light-color: #f5f5f5;
            --dark-color: #212121;
            --text-color: #333;
            --text-light: #777;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Helvetica Neue', Arial, sans-serif;
        }
        
        body {
            color: var(--text-color);
            line-height: 1.6;
            background-color: white;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        section {
            padding: 80px 0;
        }
        
        h1, h2, h3, h4 {
            font-weight: 300;
            margin-bottom: 20px;
            color: var(--dark-color);
        }
        
        h1 {
            font-size: 2.5rem;
        }
        
        h2 {
            font-size: 2rem;
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        h2:after {
            content: '';
            display: block;
            width: 60px;
            height: 2px;
            background: var(--accent-color);
            margin: 15px auto;
        }
        
        h3 {
            font-size: 1.5rem;
        }
        
        p {
            margin-bottom: 15px;
            color: var(--text-light);
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background: var(--primary-color);
            color: white;
            text-decoration: none;
            border-radius: 4px;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }
        
        .btn:hover {
            background: var(--secondary-color);
            transform: translateY(-2px);
        }
        
        .btn-outline {
            background: transparent;
            border: 1px solid var(--primary-color);
            color: var(--primary-color);
        }
        
        .btn-outline:hover {
            background: var(--primary-color);
            color: white;
        }
        
        /* Header Styles */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            z-index: 1000;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 40px;
            margin-right: 10px;
        }
        
        .logo-text {
            display: flex;
            flex-direction: column;
        }
        
        .logo-text .main {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-color);
            line-height: 1;
        }
        
        .logo-text .sub {
            font-size: 0.8rem;
            color: var(--text-light);
            line-height: 1;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--dark-color);
            font-weight: 400;
            transition: color 0.3s ease;
        }
        
        nav ul li a:hover {
            color: var(--primary-color);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #f5f7fa 0%, #e4e8eb 100%);
            padding: 180px 0 100px;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--dark-color);
        }
        
        .hero p {
            max-width: 700px;
            margin: 0 auto 40px;
            font-size: 1.2rem;
            color: var(--text-light);
        }
        
        .hero-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        
        /* About Section */
        .about {
            background-color: white;
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-image {
            flex: 1;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        /* Services Section */
        .services {
            background-color: var(--light-color);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .service-icon {
            font-size: 2.5rem;
            color: var(--accent-color);
            margin-bottom: 20px;
        }
        
        /* Features Section */
        .features {
            background-color: white;
        }
        
        .features-container {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
        }
        
        .feature {
            flex: 1 1 300px;
            display: flex;
            gap: 20px;
        }
        
        .feature-icon {
            font-size: 1.5rem;
            color: var(--accent-color);
            margin-top: 5px;
        }
        
        .feature-text h3 {
            margin-bottom: 10px;
        }
        
        /* Stats Section */
        .stats {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            color: white;
            text-align: center;
        }
        
        .stats h2 {
            color: white;
        }
        
        .stats h2:after {
            background: var(--accent-color);
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
        }
        
        .stat-item h3 {
            font-size: 3rem;
            margin-bottom: 10px;
            color: white;
        }
        
        .stat-item p {
            color: rgba(255,255,255,0.8);
        }
        
        /* Contact Section */
        .contact {
            background-color: var(--light-color);
        }
        
        .contact-container {
            display: flex;
            gap: 50px;
        }
        
        .contact-form {
            flex: 1;
            background: white;
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: var(--dark-color);
        }
        
        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 1rem;
        }
        
        .form-group textarea {
            height: 150px;
        }
        
        .contact-info {
            flex: 1;
        }
        
        .info-item {
            display: flex;
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .info-icon {
            font-size: 1.5rem;
            color: var(--accent-color);
        }
        
        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 60px 0 20px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-col h3 {
            color: white;
            margin-bottom: 20px;
            font-size: 1.2rem;
        }
        
        .footer-col ul {
            list-style: none;
        }
        
        .footer-col ul li {
            margin-bottom: 10px;
        }
        
        .footer-col ul li a {
            color: rgba(255,255,255,0.7);
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-col ul li a:hover {
            color: white;
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: rgba(255,255,255,0.5);
            font-size: 0.9rem;
        }
        
        /* Responsive Styles */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                padding: 15px 0;
            }
            
            nav ul {
                margin-top: 15px;
            }
            
            nav ul li {
                margin: 0 10px;
            }
            
            .hero {
                padding: 150px 0 80px;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .about-content {
                flex-direction: column;
            }
            
            .contact-container {
                flex-direction: column;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <img src="Elvian intelligence logo.jpg" alt="Elvian Intelligence Logo">
                <div class="logo-text">
                    <span class="main">ELVIAN</span>
                    <span class="sub">INTELLIGENCE</span>
                </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#solutions">Solutions</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Elegance Engineered.<br>Intelligence Delivered.</h1>
            <p>We pioneer IoT and AIoT solutions that transform businesses through intelligent sensing, seamless connectivity, and data-driven insights.</p>
            <div class="hero-buttons">
                <a href="#contact" class="btn">Get Started</a>
                <a href="#solutions" class="btn btn-outline">Our Solutions</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <h2>About Elvian Intelligence</h2>
            <div class="about-content">
                <div class="about-text">
                    <h3>Innovating at the Intersection of IoT and AI</h3>
                    <p>Elvian Intelligence is a leading technology firm specializing in intelligent IoT and AIoT solutions. We combine cutting-edge sensor technology with advanced artificial intelligence to deliver systems that are not just connected, but truly intelligent.</p>
                    <p>Our team of engineers and data scientists work closely with corporate clients to develop customized solutions that drive efficiency, enhance security, and unlock new opportunities through data.</p>
                    <p>With a focus on elegant design and robust frameworks, we bring the future of connected intelligence to enterprises across industries.</p>
                    <a href="#services" class="btn">Explore Our Services</a>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="IoT Technology">
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <h2>Our Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-network-wired"></i>
                    </div>
                    <h3>IoT Infrastructure</h3>
                    <p>Design and implementation of robust IoT networks with secure connectivity and edge computing capabilities for enterprise environments.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-brain"></i>
                    </div>
                    <h3>AIoT Integration</h3>
                    <p>Seamless integration of artificial intelligence with IoT systems to create intelligent, self-optimizing networks and devices.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-sensor"></i>
                    </div>
                    <h3>Smart Sensor Solutions</h3>
                    <p>Custom sensor arrays and RFID tags tailored to your specific operational needs with real-time data collection and analysis.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-database"></i>
                    </div>
                    <h3>Data Intelligence</h3>
                    <p>Advanced analytics and visualization tools to transform raw IoT data into actionable business intelligence and predictive insights.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Security & Compliance</h3>
                    <p>End-to-end security solutions for IoT ecosystems, ensuring data integrity and compliance with industry regulations.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-project-diagram"></i>
                    </div>
                    <h3>System Integration</h3>
                    <p>Integration of IoT solutions with existing enterprise systems for seamless operations and unified data management.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="solutions">
        <div class="container">
            <h2>Why Choose Our Solutions</h2>
            <div class="features-container">
                <div class="feature">
                    <div class="feature-icon">
                        <i class="fas fa-cubes"></i>
                    </div>
                    <div class="feature-text">
                        <h3>Modular Architecture</h3>
                        <p>Our solutions are built on flexible, scalable frameworks that grow with your business needs.</p>
                    </div>
                </div>
                <div class="feature">
                    <div class="feature-icon">
                        <i class="fas fa-user-tie"></i>
                    </div>
                    <div class="feature-text">
                        <h3>Corporate Focus</h3>
                        <p>Designed specifically for enterprise requirements with enterprise-grade security and reliability.</p>
                    </div>
                </div>
                <div class="feature">
                    <div class="feature-icon">
                        <i class="fas fa-lightbulb"></i>
                    </div>
                    <div class="feature-text">
                        <h3>Intelligent Automation</h3>
                        <p>AI-driven automation that learns and adapts to optimize your operations continuously.</p>
                    </div>
                </div>
                <div class="feature">
                    <div class="feature-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <div class="feature-text">
                        <h3>Proven ROI</h3>
                        <p>Measurable business outcomes with clear metrics for performance and return on investment.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="stats">
        <div class="container">
            <h2>Our Impact</h2>
            <div class="stats-grid">
                <div class="stat-item">
                    <h3>150+</h3>
                    <p>Enterprise Clients</p>
                </div>
                <div class="stat-item">
                    <h3>99.9%</h3>
                    <p>System Uptime</p>
                </div>
                <div class="stat-item">
                    <h3>10M+</h3>
                    <p>Connected Devices</p>
                </div>
                <div class="stat-item">
                    <h3>24/7</h3>
                    <p>Global Support</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <h2>Get In Touch</h2>
            <div class="contact-container">
                <div class="contact-form">
                    <form id="contactForm">
                        <div class="form-group">
                            <label for="name">Name</label>
                            <input type="text" id="name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" name="email" required>
                        </div>
                        <div class="form-group">
                            <label for="company">Company</label>
                            <input type="text" id="company" name="company" required>
                        </div>
                        <div class="form-group">
                            <label for="message">How can we help?</label>
                            <textarea id="message" name="message" required></textarea>
                        </div>
                        <button type="submit" class="btn">Send Message</button>
                    </form>
                </div>
                <div class="contact-info">
                    <div class="info-item">
                        <div class="info-icon">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <div>
                            <h3>Location</h3>
                            <p>123 Corporate Drive<br>Tech Park, Silicon Valley<br>CA 94025, USA</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon">
                            <i class="fas fa-phone"></i>
                        </div>
                        <div>
                            <h3>Phone</h3>
                            <p>+1 (555) 123-4567</p>
                            <p>Mon-Fri: 9am-6pm EST</p>
                        </div>
                    </div>
                    <div class="info-item">
                        <div class="info-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div>
                            <h3>Email</h3>
                            <p>info@elvianintel.com</p>
                            <p>support@elvianintel.com</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-col">
                    <h3>Elvian Intelligence</h3>
                    <p>Elegance Engineered. Intelligence Delivered.</p>
                    <p>Pioneering IoT and AIoT solutions for the modern enterprise.</p>
                </div>
                <div class="footer-col">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#solutions">Solutions</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Services</h3>
                    <ul>
                        <li><a href="#">IoT Infrastructure</a></li>
                        <li><a href="#">AIoT Integration</a></li>
                        <li><a href="#">Smart Sensors</a></li>
                        <li><a href="#">Data Intelligence</a></li>
                        <li><a href="#">Security Solutions</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h3>Connect</h3>
                    <ul>
                        <li><a href="#"><i class="fab fa-linkedin"></i> LinkedIn</a></li>
                        <li><a href="#"><i class="fab fa-twitter"></i> Twitter</a></li>
                        <li><a href="#"><i class="fab fa-facebook"></i> Facebook</a></li>
                        <li><a href="#"><i class="fab fa-instagram"></i> Instagram</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 Elvian Intelligence. All Rights Reserved. | Privacy Policy | Terms of Service</p>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Form submission handling
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Here you would typically send the form data to your server
            // For demonstration, we'll just show an alert
            alert('Thank you for your message! We will contact you soon.');
            this.reset();
        });
        
        // Header scroll effect
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 50) {
                header.style.boxShadow = '0 2px 10px rgba(0,0,0,0.1)';
            } else {
                header.style.boxShadow = 'none';
            }
        });
    </script>
</body>
</html>**
