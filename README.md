<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <meta name="description" content="Professional portfolio of Sajeesh K - Machine Learning Enthusiast">
    <meta name="theme-color" content="#000000">
    <title>Anmol Agarwal | Portfolio</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=Orbitron:wght@700&display=swap" rel="stylesheet">
    <link rel="icon" type="image/x-icon" href="favi.png">
    <style>
        /* Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }

        body {
            background: #000000;
            color: #FFFFFF;
            min-height: 100vh;
            overflow-x: hidden;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Heading Styles */
        h1, h2, h3 {
            color: #00FFFF;
            font-family: Georgia, serif;
            font-weight: 700;
        }

        /* Top Navigation Bar */
        nav.navbar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: #000000;
            padding: 15px 20px;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #FFFFFF;
        }

        .navbar .logo h1 {
            font-size: 1.8rem;
        }

        .navbar ul {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        .navbar ul li a {
            color: #FFFFFF;
            text-decoration: none;
            font-size: 1.1rem;
            font-weight: 400;
            transition: color 0.3s ease;
        }

        .navbar ul li a:hover {
            color: #CCCCCC;
        }

        .menu-toggle {
            display: none;
            font-size: 1.8rem;
            color: #FFFFFF;
            cursor: pointer;
        }
 /* Certifications section */
 .certifications {
            padding: 100px 0;
            position: relative;
            z-index: 1;
        }
        
        .certifications h2 {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 50px;
            position: relative;
            padding-bottom: 10px;
            color: #2adbe1;
        }
        
        .certifications h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 3px;
            background: linear-gradient(90deg, #7ee8fa, #80ff72);
        }
        
        .certificates-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            padding: 20px;
        }
        
        .certificate-item {
            background: rgba(20, 20, 20, 0.7); /* Changed from rgba(22, 27, 34, 0.7) */
            border-radius: 12px;
            overflow: hidden;
            transition: all 0.3s ease;
            position: relative;
            height: 240px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        .certificate-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            border-color: rgba(255, 255, 255, 0.2);
        }
        
        .certificate-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: all 0.3s ease;
            opacity: 0.8;
            object-position: center;
            filter: brightness(0.7);
        }
        
        .certificate-item:hover img {
            filter: brightness(0.5);
        }
        
        .certificate-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(0, 0, 0, 0.95), rgba(0, 0, 0, 0.7), transparent); /* Changed from rgba(13, 17, 23, ...) */
            padding: 30px 20px 20px;
            color: white;
            transform: translateY(60%);
            transition: all 0.3s ease;
            height: auto;
            max-height: 100%;
        }
        
        .certificate-item:hover .certificate-overlay {
            transform: translateY(0);
        }
        
        .certificate-overlay h3 {
            font-size: 1.2rem;
            margin-bottom: 8px;
            color: #fff;
        }
        
        .certificate-overlay p {
            font-size: 0.9rem;
            margin-bottom: 8px;
            line-height: 1.4;
            color: #adbac7;
        }
        
        .certificate-overlay p:first-of-type {
            color: #7ee8fa;
            font-weight: 500;
        }
        
        .certificate-overlay p:last-of-type {
            color: rgba(255, 255, 255, 0.8);
            margin-top: 10px;
        }
        
        /* Performance optimizations for smoother scrolling */
        body {
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
            text-rendering: optimizeLegibility;
            will-change: scroll-position;
            overflow-anchor: none;
        }
        
        /* Force hardware acceleration for animations and transitions */
        .portfolio-item, 
        .certificate-item, 
        .floating-element,
        .btn:hover,
        .modal-content,
        nav ul li a,
        .resume-item:hover,
        .floating-object,
        header {
            transform: translateZ(0);
            backface-visibility: hidden;
            -webkit-backface-visibility: hidden;
            will-change: transform, opacity;
            perspective: 1000px;
        }
        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 40px 20px;
            margin-top: 70px;
        }

        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
        }

        .hero-content p {
            font-size: 1.2rem;
            line-height: 1.8;
            max-width: 600px;
            margin: 0 auto 30px;
            color: #FFFFFF;
        }

        .btn {
            display: inline-block;
            padding: 12px 30px;
            background: transparent;
            color: #FFFFFF;
            text-decoration: none;
            font-weight: 600;
            border: 2px solid #FFFFFF;
            border-radius: 5px;
            transition: background 0.3s ease, color 0.3s ease;
            margin: 0 10px;
        }

        .btn:hover {
            background: #333333;
            color: #FFFFFF;
        }

        /* Section Styles */
        section {
            padding: 80px 0;
        }

        .section-heading {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 40px;
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        .section-heading::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 50px;
            height: 3px;
            background: #FFFFFF;
        }

        /* Interactive Logo for Achievements */
        .section-heading .trophy {
            font-size: 2rem;
            color: #00FFFF;
            transition: transform 0.3s ease;
        }

        .section-heading .trophy:hover {
            transform: scale(1.2);
        }

        /* Subheading for Skills */
        .subheading {
            font-size: 1.8rem;
            margin-bottom: 20px;
            text-align: center;
        }

        /* About Section */
        /* .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .about-text p {
            font-size: 1.1rem;
            line-height: 1.8;
            color: #FFFFFF;
            margin-bottom: 20px;
        }

        .about-image img {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            border: 5px solid #FFFFFF;
            transition: transform 0.3s ease;
            object-fit: cover;
        }

        .about-image:hover img {
            transform: scale(1.05);
        } */
/* About Section */
.about-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 40px;
    align-items: start; /* Changed from center */
}

.about-text {
    order: 1;
    text-align: left;
}

.about-image {
    order: 2;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-left: auto; /* Push image container to right */
}

.about-image img {
    width: 280px;
    height: 280px;
    border-radius: 50%;
    border: 5px solid #FFFFFF;
    transition: transform 0.3s ease;
    object-fit: cover;
}

/* Improved text alignment */
.about-text p {
    font-size: 1.1rem;
    line-height: 1.8;
    color: #FFFFFF;
    margin-bottom: 20px;
    text-align: justify;
    hyphens: auto;
}

/* Button container alignment */
.about-text .btn-container {
    display: flex;
    gap: 15px;
    margin-top: 25px;
}

/* Mobile Responsiveness */
@media (max-width: 768px) {
    .about-content {
        grid-template-columns: 1fr;
        text-align: center;
    }
    
    .about-image {
        order: 1;
        margin: 0 auto;
    }
    
    .about-text {
        order: 2;
    }
    
    .about-text .btn-container {
        flex-direction: column;
        align-items: center;
    }
}
        /* Skills Section */
        .skills-container {
            margin-bottom: 40px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            text-align: center;
        }

        .technical-skill-item {
            background: #000000;
            padding: 20px;
            border: 1px solid #FFFFFF;
            border-radius: 10px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .technical-skill-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(255, 255, 255, 0.2);
        }

        .technical-skill-item i {
            font-size: 2rem;
            color: #FFFFFF;
            margin-bottom: 10px;
        }

        .technical-skill-item p {
            font-size: 1rem;
            color: #FFFFFF;
        }

        .soft-skill-item {
            background: #000000;
            padding: 15px;
            border: 2px solid #FFFFFF;
            border-radius: 15px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .soft-skill-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(255, 255, 255, 0.2);
        }

        .soft-skill-item i {
            font-size: 1.8rem;
            color: #FFFFFF;
            margin-bottom: 10px;
        }

        .soft-skill-item p {
            font-size: 0.95rem;
            color: #FFFFFF;
            font-weight: 500;
            line-height: 1.4;
        }

        /* Experience Section */
        .experience-list {
            max-width: 800px;
            margin: 0 auto;
        }

        .experience-item {
            background: #000000;
            padding: 20px;
            border: 1px solid #FFFFFF;
            border-radius: 10px;
            margin-bottom: 20px;
            transition: transform 0.3s ease;
        }

        .experience-item:hover {
            transform: translateY(-5px);
        }

        .experience-item .company {
            font-size: 1.1rem;
            color: #FFFFFF;
            margin-bottom: 5px;
        }

        .experience-item .date {
            font-size: 0.9rem;
            color: #FFFFFF;
            margin-bottom: 10px;
        }

        .experience-item p {
            font-size: 1rem;
            color: #FFFFFF;
            line-height: 1.6;
        }

        /* Achievements Section */
        .achievements-list {
            max-width: 800px;
            margin: 0 auto;
        }

        .achievement-item {
            background: #000000;
            padding: 20px;
            border: 1px solid #FFFFFF;
            border-radius: 10px;
            margin-bottom: 20px;
            transition: transform 0.3s ease;
        }

        .achievement-item:hover {
            transform: translateY(-5px);
        }

        .achievement-item p {
            font-size: 1rem;
            color: #FFFFFF;
            line-height: 1.6;
        }

        /* Portfolio Section */
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .portfolio-item {
            background: #000000;
            border: 1px solid #FFFFFF;
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            cursor: pointer;
        }

        .portfolio-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(255, 255, 255, 0.2);
        }

        .portfolio-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .portfolio-overlay {
            padding: 20px;
            text-align: center;
        }

        .portfolio-overlay p {
            font-size: 1rem;
            color: #FFFFFF;
            margin-bottom: 10px;
        }

        .project-links {
            display: none;
            gap: 10px;
            justify-content: center;
        }

        .project-links.active {
            display: flex;
        }

        .project-links a {
            padding: 8px 20px;
            background: transparent;
            color: #FFFFFF;
            text-decoration: none;
            font-size: 0.9rem;
            border: 1px solid #FFFFFF;
            border-radius: 5px;
            transition: background 0.3s ease;
        }

        .project-links a:hover {
            background: #333333;
        }

        /* Contact Section */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: #000000;
            padding: 30px;
            border: 1px solid #FFFFFF;
            border-radius: 10px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            font-size: 1rem;
            margin-bottom: 8px;
            color: #FFFFFF;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 10px;
            background: #000000;
            border: 1px solid #FFFFFF;
            border-radius: 5px;
            color: #FFFFFF;
            font-size: 1rem;
        }

        .form-group textarea {
            height: 150px;
            resize: none;
        }

        /* Footer */
        footer {
            padding: 30px 0;
            text-align: center;
            background: #000000;
            border-top: 1px solid #FFFFFF;
        }

        .social-links a {
            color: #FFFFFF;
            font-size: 1.5rem;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: #CCCCCC;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .navbar ul {
                display: none;
                flex-direction: column;
                position: absolute;
                top: 60px;
                left: 0;
                width: 100%;
                background: #000000;
                padding: 20px;
                border-bottom: 1px solid #FFFFFF;
            }

            .navbar ul.active {
                display: flex;
            }

            .menu-toggle {
                display: block;
            }

            .hero-content h1 {
                font-size: 2.5rem;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .portfolio-grid {
                grid-template-columns: 1fr;
            }

            .skills-grid {
                grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            }

            .project-links {
                flex-direction: column;
                gap: 5px;
            }

            .about-image img {
                width: 200px;
                height: 200px;
            }

            .about-text .btn {
                display: block;
                margin: 10px auto;
            }
            /* Animated Background Effect */
    body::before {
        content: '';
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(45deg, #000000 25%, #001a1a 50%, #000000 75%);
        background-size: 400% 400%;
        animation: gradientBG 15s ease infinite;
        z-index: -1;
    }

    @keyframes gradientBG {
        0% { background-position: 0% 50%; }
        50% { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }

   
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="logo">
            <h1>my portfolio</h1>
        </div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#certificates">Certificates</a></li>
            <li><a href="#portfolio">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
        <div class="menu-toggle"><i class="fas fa-bars"></i></div>
    </nav>

    <div class="container">
        <!-- Hero Section -->
        <section class="hero" id="home">
            <div class="hero-content">
                <h1>Hi, I'm Anmol Agarwal</h1>
                <p>Aspiring Software Engineer with hands-on experience in full-stack development, 
                    cloud computing, and machine learning.</p>
                <a href="#portfolio" class="btn">Explore My Work</a>
            </div>
        </section>

        <!-- About Section -->
        <section class="about" id="about">
            <h2 class="section-heading">About Me</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>A passionate tech enthusiast and computer science student at Lovely Professional University, specializing in Machine Learning and Artificial Intelligence. I love building impactful projects that blend innovation with practicality, from autonomous robots to secure note vaults and real-time collaborative platforms.

                        With a solid foundation in Python, Java, C++, and full-stack development (React, Node.js, PostgreSQL), I enjoy solving real-world problems through clean, efficient code and creative thinking. I'm also deeply interested in system programming, robotics, and compiler development.
                        
                        When I'm not coding, you’ll find me exploring films, cooking something new, or collaborating on creative content as a tech creator. I'm currently aiming to secure a software engineering role at a top-tier tech company like Microsoft — and every line of code I write is a step closer to that goal.</p>
                    <div class="btn-container">
                        <a href="#contact" class="btn">Get In Touch</a>
                        <a href="sajeeshspecialised cv.pdf" class="btn">View CV</a>
                    </div>
                </div>
                <div class="about-image">
                    <img src="profile.png" alt="Sajeesh K">
                </div>
            </div>
        </section>

        <!-- Skills Section -->
        <section class="skills" id="skills">
            <h2 class="section-heading">My Skills</h2>
            <div class="skills-container">
                <h3 class="subheading">Technical Skills</h3>
                <div class="skills-grid">
                    <div class="technical-skill-item">
                        <i class="fab fa-python"></i>
                        <p>Python</p>
                    </div>
                    <div class="technical-skill-item">
                        <i class="fas fa-code"></i>
                        <p>R</p>
                    </div>
                    <div class="technical-skill-item">
                        <i class="fab fa-java"></i>
                        <p>Java</p>
                    </div>
                    <div class="technical-skill-item">
                        <i class="fas fa-code"></i>
                        <p>C++</p>
                    </div>
                    <div class="technical-skill-item">
                        <i class="fas fa-cogs"></i>
                        <p>DSA</p>
                    </div>
                    <div class="technical-skill-item">
                        <i class="fas fa-brain"></i>
                        <p>TensorFlow</p>
                    </div>
                    <div class="technical-skill-item">
                        <i class="fas fa-robot"></i>
                        <p>PyTorch</p>
                    </div>
                    <div class="technical-skill-item">
                        <i class="fas fa-database"></i>
                        <p>SQL</p>
                    </div>
                    <div class="technical-skill-item">
                        <i class="fas fa-chart-line"></i>
                        <p>Data Analysis</p>
                    </div>
                </div>
            </div>
            <div class="skills-container">
                <h3 class="subheading">Soft Skills</h3>
                <div class="skills-grid">
                    <div class="soft-skill-item">
                        <i class="fas fa-star"></i>
                        <p>Leadership and Influence</p>
                    </div>
                    <div class="soft-skill-item">
                        <i class="fas fa-lightbulb"></i>
                        <p>Problem-Solving and Critical Thinking</p>
                    </div>
                    <div class="soft-skill-item">
                        <i class="fas fa-users"></i>
                        <p>Collaboration and Teamwork</p>
                    </div>
                    <div class="soft-skill-item">
                        <i class="fas fa-comments"></i>
                        <p>Communication</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Experience Section -->
        <section class="experience" id="experience">
            <h2 class="section-heading">Experience</h2>
            <div class="experience-list">
                <div class="experience-item">
                    <h3>Azure Cloud Computing Intern</h3>
                    <p class="company">Verzeo Pvt. Ltd.</p>
                    <p class="date">February 2023 - March 2023</p>
                    <p>Designed and deployed 3+ scalable cloud solutions using Azure services virtual machines, storage,
                        networking, reducing manual deployment time by 30% through automation scripts</p>
                </div>
                <div class="experience-item">
                    <h3>Student Ambassador</h3>
                    <p class="company">Lets Upgrade</p>
                    <p class="date">July 2024 - August 2024</p>
                    <p>Adressing students in college and conducting workshops</p>
                </div>
            </div>
        </section>

        <!-- Achievements Section -->
        
        
        </section>
        <section class="certifications" id="certificates">
            <h2>Certificates</h2>
            <div class="certificates-grid">
                
                <div class="certificate-item">
                    <img src="image.png" alt="UiPath Automation Developer Associate Training">
                    <div class="certificate-overlay">
                        <h3>Design and implemention of human interface</h3>
                        <p>NPTEL</p>
                        <p>Issued: 04/10/2024</p>
                    </div>
                </div>
                <!-- Certificate 1 (Now Supervised ML) -->
                <div class="certificate-item">
                    <img src="https://imagizer.imageshack.com/img924/8930/I3mLne.png" alt="Supervised Machine Learning Certificate">
                    <div class="certificate-overlay">
                        <h3>SQL for Data Science</h3>
                        <p>Great Learning</p>
                        <p>Issued: May, 2023</p>
                    </div>
                </div>
                <!--certificate 3-->
                <div class="certificate-item">
                    <img src="dsa.png" alt="Supervised Machine Learning Certificate">
                    <div class="certificate-overlay">
                        <h3>Data Structures and Algorithms </h3>
                        <p>Lovely Professional University</p>
                        <p>Issued: August 3, 2024</p>
                    </div>
                </div>
                <!--certificate 4-->
                <div class="certificate-item">
                    <img src="https://imagizer.imageshack.com/img923/1927/gyUuv2.png" alt="Supervised Machine Learning Certificate">
                    <div class="certificate-overlay">
                        <h3>Project Leadership</h3>
                        <p>linkedin</p>
                        <p>Issued: April 2, 2025</p>
                    </div>
                </div>

                <div class="certificate-item">
                    <img src="https://imagizer.imageshack.com/img922/5228/BIXOJ1.png" alt="Supervised Machine Learning Certificate">
                    <div class="certificate-overlay">
                        <h3>Full-stack Webdevelopment Bootcamp</h3>
                        <p>Udemy</p>
                        <p>Issued: December 2, 2022</p>
                    </div>
                </div>

                <div class="certificate-item">
                    <img src="https://imagizer.imageshack.com/img924/519/ZoTF1G.png" alt="Supervised Machine Learning Certificate">
                    <div class="certificate-overlay">
                        <h3>Introduction to Responsible AI</h3>
                        <p>Coursera</p>
                        <p>Issued: May 12, 2024</p>
                    </div>
                </div>
                </div>
        </section>
               <!-- Portfolio Section -->
        <section class="portfolio" id="portfolio">
            <h2 class="section-heading">My Projects</h2>
            <div class="portfolio-grid">
                <div class="portfolio-item">
                    <img src="homepage.png" alt="Sentiment Analysis">
                    <div class="portfolio-overlay">
                        <h3>Linkode</h3>
                        <p>LinKode is a lightweight, real-time collaboration platform designed for seamless team interaction. 
                            It allows users to join virtual rooms and collaboratively edit code
                             or text with live synchronization—no installations or sign-ups required</p>
                        <div class="project-links">
                            <a href="https://github.com/sajee-sajee/Collab-Room" target="_blank">Live Demo</a>
                            <a href="https://github.com/sajee-sajee/Collab-Room" target="_blank">Code</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="coders-guild-overview.png" alt="Coders Guild overview">
                    <div class="portfolio-overlay">
                        <h3>Coders Guild - Gamified DSA Learning Platform</h3>
                        <p>Coders Guild is an immersive, cyberpunk-themed React platform that turns Data Structures and Algorithms learning into a narrative-driven RPG. Users progress through a story-led Cyber Campaign, mastering coding challenges while helping liberate a digital city.</p>
                        <div class="project-links">
                            <a href="https://code-grid.onrender.com/" target="_blank">Live Demo</a>
                            <a href="https://github.com/sajee-sajee/code-grid" target="_blank">Code</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://imagizer.imageshack.com/img924/5876/FEgLi3.png" alt="Autonomous Navigation">
                    <div class="portfolio-overlay">
                        <h3>Code-Hub</h3>
                        <p>Code Hub is a sleek, real-time online compiler designed for developers and 
                            learners to write, execute, download, and share code effortlessly — all from the browser.</p>
                        <div class="project-links">
                            <a href="https://code-collabin.vercel.app/" target="_blank">Live Demo</a>
                            <a href="https://github.com/sajee-sajee/Code-Hub" target="_blank">Code</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://imagizer.imageshack.com/img924/9550/YuaMTR.png" alt="Sentiment Analysis">
                    <div class="portfolio-overlay">
                        <h3>Termino</h3>
                        <p>A feature-rich custom Linux shell written in C++. This lightweight and 
                            interactive shell brings the power of command execution along with cool custom 
                            commands like weather updates, note-taking,
                             reminders, background job handling, I/O redirection, and pipelines — all in one terminal interface!</p>
                        <div class="project-links">
                            <a href="https://github.com/sajee-sajee/Terminal-by-CPP" target="_blank">Live Demo</a>
                            <a href="https://github.com/sajee-sajee/Terminal-by-CPP" target="_blank">Code</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="image copy 2.png" alt="Sentiment Analysis">
                    <div class="portfolio-overlay">
                        <h3>Automated Fruit Counting Orchards Using Drones for Yield Estimation</h3>
                        <p>This project implements a computer vision-based system to automate fruit counting in 
                            orchards using drone-captured imagery, aiding in yield estimation for precision agriculture.</p>
                        <div class="project-links">
                            <a href="https://github.com/sajee-sajee/Counting-apples-using-image-processing" target="_blank">Live Demo</a>
                            <a href="https://github.com/sajee-sajee/Counting-apples-using-image-processing" target="_blank">Code</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio-item">
                    <img src="https://imagizer.imageshack.com/img923/5233/0jkpgY.png" alt="Sentiment Analysis">
                    <div class="portfolio-overlay">
                        <h3>Chatbot using gemini api</h3>
                        <p>A simple chatbot application powered by the Gemini API. This project allows 
                            users to interact with a conversational AI using a provided API key. Built with Python and Flask,
                             it demonstrates 
                            how to integrate the Gemini API into a chatbot interface.</p>
                        <div class="project-links">
            
                            <a href="https://github.com/sajee-sajee/Chatbotbygeminiapi" target="_blank">Code</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section class="contact" id="contact">
            <h2 class="section-heading">Contact Me</h2>
            <div class="contact-form">
                <form action="https://formspree.io/f/xldbgpdq" method="POST">
                    <div class="form-group">
                        <label for="name">Name</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="_replyto" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" name="message" required></textarea>
                    </div>
                    <button type="submit" class="btn">Send Message</button>
                </form>
            </div>
        </section>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="social-links">
                <a href="https://www.linkedin.com/in/sajeeshk1" target="_blank"><i class="fab fa-linkedin"></i></a>
                <a href="https://github.com/sajee-sajee" target="_blank"><i class="fab fa-github"></i></a>
            </div>
            <p>© 2025 Sajeesh K. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const menuToggle = document.querySelector('.menu-toggle');
        const navLinks = document.querySelector('.navbar ul');

        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });

        // Close menu when clicking a link
        document.querySelectorAll('.navbar ul li a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
            });
        });

        // Smooth Scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });

        // Portfolio Project Links Toggle
        document.querySelectorAll('.portfolio-item').forEach(item => {
            item.addEventListener('click', () => {
                const links = item.querySelector('.project-links');
                links.classList.toggle('active');
            });
        });
    </script>
</body>
</html>
