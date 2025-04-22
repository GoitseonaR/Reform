# Reform
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Re-form | Strategic Growth Consultancy</title>
    <style>
        /* Global Styles */
        :root {
            --primary: #2563eb;
            --dark: #1e293b;
            --light: #f8fafc;
            --accent: #f59e0b;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header & Navigation */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            z-index: 100;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            font-size: 24px;
            font-weight: 700;
            color: var(--primary);
        }
        
        .nav-links {
            display: flex;
            gap: 30px;
        }
        
        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        .cta-button {
            background-color: var(--primary);
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            font-weight: 600;
            transition: background-color 0.3s;
        }
        
        .cta-button:hover {
            background-color: #1d4ed8;
        }
        
        /* Hero Section */
        .hero {
            padding: 150px 0 100px;
            background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
            text-align: center;
        }
        
        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        .hero p {
            font-size: 20px;
            max-width: 700px;
            margin: 0 auto 40px;
            color: #475569;
        }
        
        /* About Section */
        .about {
            padding: 100px 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
            font-size: 36px;
            color: var(--dark);
        }
        
        .about-content {
            display: flex;
            gap: 50px;
            align-items: center;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            font-size: 24px;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .vision-box {
            background-color: #f8fafc;
            border-left: 4px solid var(--accent);
            padding: 20px;
            margin-top: 30px;
        }
        
        .vision-box p {
            font-style: italic;
            color: #475569;
        }
        
        /* Services Section */
        .services {
            padding: 100px 0;
            background-color: #f8fafc;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background-color: white;
            border-radius: 8px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
        }
        
        .service-card h3 {
            color: var(--primary);
            margin-bottom: 15px;
            font-size: 20px;
        }
        
        /* Case Studies */
        .case-studies {
            padding: 100px 0;
            background-color: white;
        }
        
        .case-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .case-card {
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .case-image {
            height: 200px;
            background-color: #e2e8f0;
            /* Replace with actual image */
        }
        
        .case-content {
            padding: 20px;
        }
        
        .case-content h3 {
            margin-bottom: 10px;
            color: var(--dark);
        }
        
        /* Contact Section */
        .contact {
            padding: 100px 0;
            background-color: #f8fafc;
        }
        
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: white;
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
            font-weight: 500;
        }
        
        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #e2e8f0;
            border-radius: 5px;
            font-size: 16px;
        }
        
        .form-group textarea {
            height: 150px;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
            text-align: center;
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .footer-links a {
            color: white;
            text-decoration: none;
        }
        
        .copyright {
            color: #94a3b8;
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .about-content {
                flex-direction: column;
            }
            
            .hero h1 {
                font-size: 36px;
            }
            
            .hero p {
                font-size: 18px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">Re-form</div>
                <div class="nav-links">
                    <a href="#home">Home</a>
                    <a href="#about">About</a>
                    <a href="#services">Services</a>
                    <a href="#cases">Case Studies</a>
                    <a href="#contact">Contact</a>
                    <a href="#contact" class="cta-button">Get Started</a>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Strategic Growth for Ambitious Businesses</h1>
            <p>Data-driven strategies that transform uncertainty into predictable, sustainable growth for SMEs and startups across the Netherlands.</p>
            <a href="#contact" class="cta-button">Scale Your Business</a>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <h2 class="section-title">About Re-form</h2>
            <div class="about-content">
                <div class="about-text">
                    <h3>We're changing how businesses grow</h3>
                    <p>Re-form is a strategic growth consultancy that empowers small and medium-sized enterprises (SMEs) and startups in the Netherlands to scale efficiently through data-driven strategies, market positioning, and operational optimization.</p>
                    <p>Unlike traditional marketing agencies, Re-form focuses on long-term strategic planning rather than just execution, helping businesses adapt, innovate, and outperform competitors.</p>
                    
                    <div class="vision-box">
                        <p><strong>Our Vision:</strong> "To become the Netherlands' most trusted strategic growth partner for innovative SMEs by 2030."</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <h2 class="section-title">Our Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <h3>Growth Strategy Development</h3>
                    <p>Comprehensive roadmaps tailored to your business objectives, market position, and growth potential.</p>
                </div>
                <div class="service-card">
                    <h3>Market Positioning</h3>
                    <p>Differentiate your brand and offerings to stand out in competitive markets.</p>
                </div>
                <div class="service-card">
                    <h3>Operational Optimization</h3>
                    <p>Streamline processes and systems to support scalable growth.</p>
                </div>
                <div class="service-card">
                    <h3>Data-Driven Decision Making</h3>
                    <p>Implement analytics frameworks to remove guesswork from growth strategies.</p>
                </div>
                <div class="service-card">
                    <h3>Customer Acquisition Systems</h3>
                    <p>Build predictable pipelines for qualified leads and conversions.</p>
                </div>
                <div class="service-card">
                    <h3>Retention Strategy</h3>
                    <p>Develop systems to increase customer lifetime value and reduce churn.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Case Studies -->
    <section class="case-studies" id="cases">
        <div class="container">
            <h2 class="section-title">Case Studies</h2>
            <div class="case-grid">
                <div class="case-card">
                    <div class="case-image"></div>
                    <div class="case-content">
                        <h3>E-commerce Platform</h3>
                        <p>Increased monthly revenue by 72% through strategic repositioning and customer journey optimization.</p>
                    </div>
                </div>
                <div class="case-card">
                    <div class="case-image"></div>
                    <div class="case-content">
                        <h3>B2B SaaS Startup</h3>
                        <p>Reduced customer acquisition costs by 40% while doubling lead flow in 6 months.</p>
                    </div>
                </div>
                <div class="case-card">
                    <div class="case-image"></div>
                    <div class="case-content">
                        <h3>Professional Services Firm</h3>
                        <p>Implemented operational systems that supported 3x growth without additional overhead.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <h2 class="section-title">Ready to Transform Your Growth?</h2>
            <div class="contact-form">
                <form>
                    <div class="form-group">
                        <label for="name">Name</label>
                        <input type="text" id="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" required>
                    </div>
                    <div class="form-group">
                        <label for="company">Company</label>
                        <input type="text" id="company">
                    </div>
                    <div class="form-group">
                        <label for="message">How can we help?</label>
                        <textarea id="message" required></textarea>
                    </div>
                    <button type="submit" class="cta-button" style="border: none; cursor: pointer;">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-links">
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#services">Services</a>
                <a href="#cases">Case Studies</a>
                <a href="#contact">Contact</a>
            </div>
            <div class="logo" style="color: white; margin-bottom: 20px;">Re-form</div>
            <p class="copyright">© 2023 Re-form Strategic Growth Consultancy. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
