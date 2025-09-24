<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Educate Rural - Empowering Students in Rural Communities</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2563eb;
            --secondary: #059669;
            --accent: #dc2626;
            --light: #f8fafc;
            --dark: #0f172a;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
        }
        
        .navbar {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
        }
        
        .hero {
            background: linear-gradient(135deg, rgba(37, 99, 235, 0.9) 0%, rgba(5, 150, 105, 0.9) 100%), url('https://placehold.co/1920x1080/2563eb/ffffff?text=Rural+Students+Learning') center/cover no-repeat;
            color: white;
            padding: 100px 0;
            text-align: center;
        }
        
        .section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        .section-title:after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: var(--primary);
            margin: 15px auto;
            border-radius: 2px;
        }
        
        .program-card {
            transition: transform 0.3s, box-shadow 0.3s;
            border: none;
            border-radius: 15px;
            overflow: hidden;
            height: 100%;
        }
        
        .program-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .program-icon {
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .impact-stat {
            text-align: center;
            padding: 30px;
            border-radius: 15px;
            background: white;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
        }
        
        .impact-stat:hover {
            transform: scale(1.05);
        }
        
        .stat-number {
            font-size: 3rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 10px;
        }
        
        .testimonial-card {
            border: none;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .cta-section {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 80px 0;
            text-align: center;
        }
        
        .btn-primary {
            background: var(--primary);
            border: none;
            padding: 12px 30px;
            border-radius: 50px;
            font-weight: 600;
            transition: all 0.3s;
        }
        
        .btn-primary:hover {
            background: #1d4ed8;
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .btn-secondary {
            background: var(--secondary);
            border: none;
            padding: 12px 30px;
            border-radius: 50px;
            font-weight: 600;
        }
        
        .btn-secondary:hover {
            background: #047857;
        }
        
        footer {
            background: var(--dark);
            color: white;
            padding: 60px 0 30px;
        }
        
        .footer-link {
            color: #cbd5e1;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-link:hover {
            color: white;
        }
        
        .social-icon {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            display: inline-flex;
            align-items: center;
            justify-content: center;
            margin-right: 10px;
            transition: all 0.3s;
        }
        
        .social-icon:hover {
            background: var(--primary);
            transform: translateY(-3px);
        }
        
        .map-container {
            height: 400px;
            background: #e2e8f0;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #64748b;
        }
        
        @media (max-width: 768px) {
            .hero {
                padding: 60px 0;
            }
            
            .section {
                padding: 50px 0;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-light sticky-top">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#">
                <i class="fas fa-graduation-cap me-2"></i>Educate Rural
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
                    <li class="nav-item"><a class="nav-link" href="#programs">Programs</a></li>
                    <li class="nav-item"><a class="nav-link" href="#impact">Impact</a></li>
                    <li class="nav-item"><a class="nav-link" href="#stories">Stories</a></li>
                    <li class="nav-item"><a class="nav-link" href="#get-involved">Get Involved</a></li>
                </ul>
                <div class="ms-lg-3 mt-3 mt-lg-0">
                    <a href="#donate" class="btn btn-primary">Donate</a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-8">
                    <h1 class="display-4 fw-bold mb-4">Empowering Rural Students Through Education</h1>
                    <p class="lead mb-5">Bridging the educational gap by providing essential resources, technology, and opportunities to students in underserved communities.</p>
                    <div class="d-flex flex-column flex-md-row gap-3 justify-content-center">
                        <a href="#donate" class="btn btn-primary btn-lg">Donate Now</a>
                        <a href="#get-involved" class="btn btn-secondary btn-lg">Get Involved</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section bg-light">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6 mb-5 mb-lg-0">
                    <h2 class="section-title">Our Story</h2>
                    <p class="lead">Founded with a vision to transform education in rural communities, Educate Rural began as a small initiative to provide books to underserved schools.</p>
                    <p>Today, we've expanded our reach to provide comprehensive educational support including books, uniforms, technology, and scholarships to thousands of students across the country.</p>
                    <p>Our core values of equity, empowerment, and excellence drive every program we develop and every student we support.</p>
                    <div class="mt-4">
                        <h5>Our Mission</h5>
                        <p>To empower students and enhance learning in rural schools by providing essential resources and bridging the gap in educational access and opportunity.</p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="row g-3">
                        <div class="col-6">
                            <img src="https://placehold.co/600x400/2563eb/ffffff?text=Our+Team" class="img-fluid rounded shadow" alt="Our Team">
                        </div>
                        <div class="col-6">
                            <img src="https://placehold.co/600x400/059669/ffffff?text=Students" class="img-fluid rounded shadow" alt="Students">
                        </div>
                        <div class="col-12 mt-3">
                            <img src="https://placehold.co/800x300/dc2626/ffffff?text=Community+Impact" class="img-fluid rounded shadow" alt="Community Impact">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Programs Section -->
    <section id="programs" class="section">
        <div class="container">
            <h2 class="section-title">Our Programs</h2>
            <div class="row g-4">
                <div class="col-md-6 col-lg-4">
                    <div class="card program-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="program-icon">
                                <i class="fas fa-book"></i>
                            </div>
                            <h3 class="card-title">Book & Resource Distribution</h3>
                            <p class="card-text">Providing writing books, materials, and storybooks to rural schools to enhance learning experiences and literacy.</p>
                            <a href="#" class="btn btn-outline-primary">Learn More</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4">
                    <div class="card program-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="program-icon">
                                <i class="fas fa-tshirt"></i>
                            </div>
                            <h3 class="card-title">Essential Supplies</h3>
                            <p class="card-text">Distributing school uniforms and bags to boost student confidence and reduce barriers to education.</p>
                            <a href="#" class="btn btn-outline-primary">Learn More</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4">
                    <div class="card program-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="program-icon">
                                <i class="fas fa-laptop"></i>
                            </div>
                            <h3 class="card-title">Digital Learning</h3>
                            <p class="card-text">Bringing technology and assistive devices to rural areas to ensure inclusive education for all students.</p>
                            <a href="#" class="btn btn-outline-primary">Learn More</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4">
                    <div class="card program-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="program-icon">
                                <i class="fas fa-school"></i>
                            </div>
                            <h3 class="card-title">Adoption Programs</h3>
                            <p class="card-text">"Adopt a Classroom" and "Adopt a School" initiatives to provide comprehensive support to educational institutions.</p>
                            <a href="#" class="btn btn-outline-primary">Learn More</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4">
                    <div class="card program-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="program-icon">
                                <i class="fas fa-graduation-cap"></i>
                            </div>
                            <h3 class="card-title">Scholarships</h3>
                            <p class="card-text">Providing financial assistance to deserving students to continue their education and achieve their dreams.</p>
                            <a href="#" class="btn btn-outline-primary">Learn More</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-4">
                    <div class="card program-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="program-icon">
                                <i class="fas fa-book-reader"></i>
                            </div>
                            <h3 class="card-title">Countrywide Libraries</h3>
                            <p class="card-text">Establishing mini and e-libraries across rural communities to provide access to knowledge and resources.</p>
                            <a href="#" class="btn btn-outline-primary">Learn More</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Impact Section -->
    <section id="impact" class="section bg-light">
        <div class="container">
            <h2 class="section-title">Our Impact</h2>
            <div class="row g-4">
                <div class="col-md-3 col-6">
                    <div class="impact-stat">
                        <div class="stat-number">15,000+</div>
                        <div class="stat-text">Students Supported</div>
                    </div>
                </div>
                <div class="col-md-3 col-6">
                    <div class="impact-stat">
                        <div class="stat-number">250+</div>
                        <div class="stat-text>Schools Reached</div>
                    </div>
                </div>
                <div class="col-md-3 col-6">
                    <div class="impact-stat">
                        <div class="stat-number">50+</div>
                        <div class="stat-text>Libraries Built</div>
                    </div>
                </div>
                <div class="col-md-3 col-6">
                    <div class="impact-stat">
                        <div class="stat-number">1,200+</div>
                        <div class="stat-text>Scholarships Awarded</div>
                    </div>
                </div>
            </div>
            
            <div class="row mt-5">
                <div class="col-lg-6 mb-4 mb-lg-0">
                    <h3 class="mb-4">Countrywide Library Network</h3>
                    <p>Our interactive map shows the locations of our mini libraries and e-libraries across the country, serving as symbols of our widespread reach and commitment to education.</p>
                    <div class="map-container">
                        <div>
                            <i class="fas fa-map-marked-alt fa-3x mb-3"></i>
                            <p class="mb-0">Interactive Map of Library Locations</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6">
                    <h3 class="mb-4">Annual Impact Report</h3>
                    <div class="progress mb-3">
                        <div class="progress-bar bg-primary" role="progressbar" style="width: 85%">Books Distributed</div>
                    </div>
                    <div class="progress mb-3">
                        <div class="progress-bar bg-success" role="progressbar" style="width: 75%">Students Fed</div>
                    </div>
                    <div class="progress mb-3">
                        <div class="progress-bar bg-info" role="progressbar" style="width: 90%">Schools Supplied</div>
                    </div>
                    <div class="progress mb-3">
                        <div class="progress-bar bg-warning" role="progressbar" style="width: 70%">Digital Resources</div>
                    </div>
                    <p class="mt-4">Download our full annual impact report to see detailed statistics and success stories from our programs.</p>
                    <a href="#" class="btn btn-outline-primary">Download Report</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Stories Section -->
    <section id="stories" class="section">
        <div class="container">
            <h2 class="section-title">Success Stories</h2>
            <div class="row g-4">
                <div class="col-lg-4">
                    <div class="card testimonial-card h-100">
                        <img src="https://placehold.co/600x400/2563eb/ffffff?text=Student+Story" class="card-img-top" alt="Student Story">
                        <div class="card-body">
                            <h5 class="card-title">Maria's Journey to University</h5>
                            <p class="card-text">Thanks to our scholarship program, Maria became the first in her family to attend university. She now studies engineering and dreams of building sustainable housing for rural communities.</p>
                            <a href="#" class="btn btn-link p-0">Read Full Story <i class="fas fa-arrow-right ms-1"></i></a>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4">
                    <div class="card testimonial-card h-100">
                        <img src="https://placehold.co/600x400/059669/ffffff?text=Teacher+Story" class="card-img-top" alt="Teacher Story">
                        <div class="card-body">
                            <h5 class="card-title">Mr. Johnson's Classroom Transformation</h5>
                            <p class="card-text">After adopting his classroom, donors helped Mr. Johnson create a technology-rich learning environment. His students' test scores improved by 40% in one year.</p>
                            <a href="#" class="btn btn-link p-0">Read Full Story <i class="fas fa-arrow-right ms-1"></i></a>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4">
                    <div class="card testimonial-card h-100">
                        <img src="https://placehold.co/600x400/dc2626/ffffff?text=Community+Story" class="card-img-top" alt="Community Story">
                        <div class="card-body">
                            <h5 class="card-title">Green Valley's Digital Library</h5>
                            <p class="card-text">Our e-library transformed Green Valley community center into a hub of learning. Now over 300 students access digital resources daily, bridging the urban-rural education gap.</p>
                            <a href="#" class="btn btn-link p-0">Read Full Story <i class="fas fa-arrow-right ms-1"></i></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Get Involved Section -->
    <section id="get-involved" class="section bg-light">
        <div class="container">
            <h2 class="section-title">Get Involved</h2>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="card h-100 border-0 shadow-sm">
                        <div class="card-body text-center p-4">
                            <div class="program-icon text-primary">
                                <i class="fas fa-donate"></i>
                            </div>
                            <h3 class="card-title">Donate</h3>
                            <p>Your contribution helps us provide books, supplies, and technology to students in need.</p>
                            <a href="#donate" class="btn btn-primary">Donate Now</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card h-100 border-0 shadow-sm">
                        <div class="card-body text-center p-4">
                            <div class="program-icon text-success">
                                <i class="fas fa-hands-helping"></i>
                            </div>
                            <h3 class="card-title">Volunteer</h3>
                            <p>Join our team of volunteers to help distribute resources, mentor students, or assist with events.</p>
                            <a href="#" class="btn btn-success">Volunteer</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card h-100 border-0 shadow-sm">
                        <div class="card-body text-center p-4">
                            <div class="program-icon text-info">
                                <i class="fas fa-handshake"></i>
                            </div>
                            <h3 class="card-title">Partnerships</h3>
                            <p>Corporate and organizational partnerships help us expand our reach and impact more students.</p>
                            <a href="#" class="btn btn-info">Partner With Us</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section id="donate" class="cta-section">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-8">
                    <h2 class="display-5 fw-bold mb-4">Make a Difference Today</h2>
                    <p class="lead mb-5">Your support can transform a student's life. Whether it's $10 for books or $100 for a scholarship, every contribution matters.</p>
                    <div class="d-flex flex-column flex-md-row gap-3 justify-content-center">
                        <a href="#" class="btn btn-light btn-lg">Donate $25</a>
                        <a href="#" class="btn btn-light btn-lg">Donate $50</a>
                        <a href="#" class="btn btn-light btn-lg">Custom Amount</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-lg-4 mb-5 mb-lg-0">
                    <h4 class="mb-4">Educate Rural</h4>
                    <p>Empowering students and enhancing learning in rural schools through essential resources and opportunities.</p>
                    <div class="mt-4">
                        <a href="#" class="social-icon"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 mb-4 mb-md-0">
                    <h5 class="mb-4">Quick Links</h5>
                    <ul class="list-unstyled">
                        <li class="mb-2"><a href="#home" class="footer-link">Home</a></li>
                        <li class="mb-2"><a href="#about" class="footer-link">About Us</a></li>
                        <li class="mb-2"><a href="#programs" class="footer-link">Programs</a></li>
                        <li class="mb-2"><a href="#impact" class="footer-link">Impact</a></li>
                        <li class="mb-2"><a href="#stories" class="footer-link">Stories</a></li>
                    </ul>
                </div>
                <div class="col-lg-2 col-md-4 mb-4 mb-md-0">
                    <h5 class="mb-4">Get Involved</h5>
                    <ul class="list-unstyled">
                        <li class="mb-2"><a href="#donate" class="footer-link">Donate</a></li>
                        <li class="mb-2"><a href="#" class="footer-link">Volunteer</a></li>
                        <li class="mb-2"><a href="#" class="footer-link">Partner</a></li>
                        <li class="mb-2"><a href="#" class="footer-link">Events</a></li>
                        <li class="mb-2"><a href="#" class="footer-link">Newsletter</a></li>
                    </ul>
                </div>
                <div class="col-lg-4 col-md-4">
                    <h5 class="mb-4">Contact Us</h5>
                    <ul class="list-unstyled">
                        <li class="mb-2"><i class="fas fa-envelope me-2"></i> info@educaterural.org</li>
                        <li class="mb-2"><i class="fas fa-phone me-2"></i> +1 (555) 123-4567</li>
                        <li class="mb-2"><i class="fas fa-map-marker-alt me-2"></i> 123 Education Street, City, State 12345</li>
                    </ul>
                    <div class="mt-4">
                        <form>
                            <div class="input-group">
                                <input type="email" class="form-control" placeholder="Your Email">
                                <button class="btn btn-primary" type="button">Subscribe</button>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
            <hr class="my-5 bg-secondary">
            <div class="row">
                <div class="col-md-6 text-center text-md-start">
                    <p>&copy; 2023 Educate Rural. All rights reserved.</p>
                </div>
                <div class="col-md-6 text-center text-md-end">
                    <a href="#" class="footer-link me-3">Privacy Policy</a>
                    <a href="#" class="footer-link">Terms of Service</a>
                </div>
            </div>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
