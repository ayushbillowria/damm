<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ayush Billowria | Digital Portfolio</title>
    <style>
:root {
    --bg-color: #050505;
    --text-primary: #ffffff;
    --text-muted: #a0a0a0;
    --accent-color: #00f0ff;
    --accent-secondary: #7000ff;
    --glass-bg: rgba(255, 255, 255, 0.05);
    --glass-border: rgba(255, 255, 255, 0.1);
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background-color: var(--bg-color);
    color: var(--text-primary);
    font-family: 'Outfit', sans-serif;
    line-height: 1.6;
    overflow-x: hidden;
}

h1, h2, h3, .logo {
    font-family: 'Space Grotesk', sans-serif;
}

#particles-js {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
}

/* Navigation */
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.5rem 5%;
    background: rgba(5, 5, 5, 0.8);
    backdrop-filter: blur(10px);
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 100;
    border-bottom: 1px solid var(--glass-border);
}

.logo {
    font-size: 2rem;
    font-weight: 800;
    background: linear-gradient(45deg, var(--accent-color), var(--accent-secondary));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    cursor: pointer;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 2rem;
}

.nav-links a {
    color: var(--text-primary);
    text-decoration: none;
    font-weight: 600;
    transition: color 0.3s ease;
    position: relative;
}

.nav-links a::after {
    content: '';
    position: absolute;
    bottom: -5px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--accent-color);
    transition: width 0.3s ease;
}

.nav-links a:hover {
    color: var(--accent-color);
}

.nav-links a:hover::after {
    width: 100%;
}

/* Main Sections */
main {
    padding-top: 100px;
}

section {
    min-height: 100vh;
    padding: 5rem 10%;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.section-title {
    font-size: 2.5rem;
    margin-bottom: 3rem;
    text-align: center;
    position: relative;
    display: inline-block;
    align-self: center;
}

.section-title::after {
    content: '';
    position: absolute;
    bottom: -10px;
    left: 50%;
    transform: translateX(-50%);
    width: 50px;
    height: 3px;
    background: var(--accent-secondary);
}

/* Glassmorphism Effect */
.glass-effect {
    background: var(--glass-bg);
    backdrop-filter: blur(12px);
    border: 1px solid var(--glass-border);
    border-radius: 20px;
    padding: 2.5rem;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.glass-effect:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 30px rgba(0, 240, 255, 0.1);
}

/* Hero Section */
#hero {
    align-items: flex-start;
}

.hero-content {
    max-width: 800px;
}

.cta-button {
    display: inline-block;
    padding: 1rem 2.5rem;
    background: transparent;
    color: var(--text-primary);
    text-decoration: none;
    font-family: 'Space Grotesk', sans-serif;
    font-weight: bold;
    border: 2px solid var(--accent-color);
    border-radius: 30px;
    transition: all 0.3s ease;
    text-transform: uppercase;
    letter-spacing: 1px;
    box-shadow: 0 0 15px rgba(0, 240, 255, 0.2);
}

.cta-button:hover {
    background: var(--accent-color);
    color: #000;
    box-shadow: 0 0 30px rgba(0, 240, 255, 0.5);
}

/* Contact Section */
.contact-container {
    text-align: center;
    max-width: 600px;
    margin: 0 auto;
}

.social-links {
    display: flex;
    justify-content: center;
    gap: 2rem;
}

.social-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 60px;
    height: 60px;
    background: rgba(255, 255, 255, 0.05);
    border-radius: 50%;
    font-size: 1.5rem;
    color: var(--text-primary);
    text-decoration: none;
    transition: all 0.3s ease;
    border: 1px solid var(--glass-border);
}

.social-icon:hover {
    background: var(--accent-color);
    color: #000;
    transform: translateY(-5px);
    box-shadow: 0 5px 20px rgba(0, 240, 255, 0.4);
}

/* Footer */
footer {
    text-align: center;
    padding: 2rem;
    border-top: 1px solid var(--glass-border);
    color: var(--text-muted);
    font-size: 0.9rem;
}

.fade-in {
    opacity: 0;
    transform: translateY(30px);
    transition: opacity 0.8s ease, transform 0.8s ease;
}

.fade-in.visible {
    opacity: 1;
    transform: translateY(0);
}

@media (max-width: 768px) {
    .nav-links {
        display: none;
    }
}
    </style>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link
        href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600;800&family=Space+Grotesk:wght@400;700&display=swap"
        rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.15.1/devicon.min.css">
</head>

<body>
    <div id="particles-js"></div>

    <nav>
        <div class="logo">AB.</div>
        <ul class="nav-links">
            <li><a href="#about">Profile</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#achievements">Achievements</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <main>
        <section id="hero">
            <div class="hero-content">
                <h2 class="section-title" style="margin-bottom: 2rem;">1. Home / Profile Section</h2>
                <p class="description" style="font-size: 1.2rem; line-height: 1.8;">
                    <b>About Me</b> - Hello! I am Ayush Billowria, a passionate and driven B.Tech student at Model Institute of Engineering and Technology, Kot Bhalwal, Jammu. With a strong interest in technology and problem-solving, I am continuously building my skills in software development, programming, and emerging technologies.
                </p>
                <div class="key-highlights" style="margin-bottom: 2rem; color: #00f0ff;">
                    <p style="margin-bottom: 0.5rem; font-weight: bold; font-family: 'Space Grotesk', sans-serif;">Key
                        Highlights</p>
                    <ul style="list-style-position: inside; color: #a0a0a0; font-size: 1.1rem; line-height: 1.8;">
                        <li>Currently Pursuing B.Tech</li>
                        <li>Quick Learner | Team Player | Detail-Oriented</li>
                    </ul>
                </div>
                <a href="#contact" class="cta-button">Get In Touch</a>
            </div>
        </section>

        <section id="education" class="fade-in">
            <h2 class="section-title">Education</h2>
            <div class="card glass-effect">
                <div class="card-content" style="font-size: 1.2rem;">
                    <ul style="list-style-type: none;">
                        <li style="margin-bottom: 1rem;"><i class="fas fa-check-circle"
                                style="color: var(--accent-color); margin-right: 10px;"></i> <b>B.Tech (pursuing)</b>
                        </li>
                        <li style="margin-bottom: 1rem;"><i class="fas fa-check-circle"
                                style="color: var(--accent-color); margin-right: 10px;"></i> <b>12th</b></li>
                        <li><i class="fas fa-check-circle" style="color: var(--accent-color); margin-right: 10px;"></i>
                            <b>10th</b>
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="skills" class="fade-in">
            <h2 class="section-title">Technical Skills</h2>
            <div class="glass-effect" style="font-size: 1.2rem; line-height: 2;">
                <p><span style="color: var(--accent-color); font-weight: bold;">Programming Languages:</span> C
                    programming</p>
                <p><span style="color: var(--accent-color); font-weight: bold;">Tools & Technologies:</span> Git, VS
                    Code, Google Colab, etc.</p>
                <p><span style="color: var(--accent-color); font-weight: bold;">Soft Skills:</span> Problem Solving,
                    Teamwork, Communication, Time Management</p>
            </div>
        </section>

        <section id="achievements" class="fade-in">
            <h2 class="section-title">Key Achievements</h2>
            <div class="timeline">
                <div class="timeline-item glass-effect">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <h3>Problem Solving Milestone</h3>
                        <p>Successfully solved 50+ foundational programming problems on HackerRank using C, achieving a
                            3-star rating in logic building.</p>
                    </div>
                </div>
                <div class="timeline-item glass-effect">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <h3>Early Project Development</h3>
                        <p>Developed terminal-based interactive applications in C, including a text-based Calculator and
                            a robust student record management system.</p>
                    </div>
                </div>
                <div class="timeline-item glass-effect">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <h3>Coding Bootcamps & Workshops</h3>
                        <p>Active participant in introductory Web Development and C++ coding workshops organized by the
                            college tech club.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact" class="fade-in">
            <h2 class="section-title">Let's Connect</h2>
            <div class="contact-container glass-effect">
                <p>I'm always open to discussing tech, collaborations, or new opportunities!</p>
                <p style="margin-bottom: 2rem; color: var(--accent-color); font-size: 1.2rem;">
                    <i class="fas fa-map-marker-alt" style="margin-right: 10px;"></i> Location: Jammu, Jammu & Kashmir
                </p>
                <div class="social-links">
                    <a href="mailto:ayushbillowria108@gmail.com" class="social-icon" aria-label="Email"><i
                            class="fas fa-envelope"></i></a>
                    <a href="tel:+917889896968" class="social-icon" aria-label="Phone"><i class="fas fa-phone"></i></a>
                    <a href="https://www.linkedin.com/in/ayush-billowria-a2959b386?utm_source=share_via&utm_content=profile&utm_medium=member_android"
                        target="_blank" class="social-icon" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Ayush Billowria. Designed for Excellence.</p>
    </footer>

    <!-- Particles.js for interactive background -->
    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script>
document.addEventListener('DOMContentLoaded', () => {
    particlesJS('particles-js', {
        "particles": {
            "number": { "value": 80, "density": { "enable": true, "value_area": 800 } },
            "color": { "value": ["#00f0ff", "#7000ff"] },
            "shape": { "type": "circle" },
            "opacity": { "value": 0.5, "random": false },
            "size": { "value": 3, "random": true },
            "line_linked": { "enable": true, "distance": 150, "color": "#ffffff", "opacity": 0.1, "width": 1 },
            "move": { "enable": true, "speed": 2, "direction": "none", "random": false, "straight": false, "out_mode": "out", "bounce": false }
        },
        "interactivity": {
            "detect_on": "canvas",
            "events": {
                "onhover": { "enable": true, "mode": "grab" },
                "onclick": { "enable": true, "mode": "push" },
                "resize": true
            },
            "modes": {
                "grab": { "distance": 140, "line_linked": { "opacity": 0.5 } },
                "push": { "particles_nb": 4 }
            }
        },
        "retina_detect": true
    });

    const observerOptions = { root: null, rootMargin: '0px', threshold: 0.1 };
    const observer = new IntersectionObserver((entries, observer) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.classList.add('visible');
            }
        });
    }, observerOptions);

    const fadeElements = document.querySelectorAll('.fade-in');
    fadeElements.forEach(el => observer.observe(el));

    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            document.querySelector(this.getAttribute('href')).scrollIntoView({ behavior: 'smooth' });
        });
    });
});
    </script>
</body>

</html>
