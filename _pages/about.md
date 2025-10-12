---
layout: archive
title: "About"
permalink: /
author_profile: true
redirect_from:
  - /about.html
---

{% include base_path %}

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');

.about-container {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    line-height: 1.6;
    color: #1a1a1a;
    max-width: 920px;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

/* Hero Introduction Section */
.about-intro {
    font-size: 1.1em;
    color: #1a1a1a;
    background: rgba(30, 58, 138, 0.08);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    margin-bottom: 35px;
    padding: 35px;
    border-radius: 20px;
    border: 1px solid rgba(30, 58, 138, 0.15);
    box-shadow: 0 10px 30px rgba(30, 58, 138, 0.05);
    animation: fadeInUp 0.8s ease-out;
}

.about-intro .highlight {
    color: #1e3a8a;
    font-weight: 700;
}

/* Section Styling */
.about-section {
    margin: 45px 0;
    animation: fadeInUp 0.6s ease-out;
}

.about-section-title {
    font-size: 1.5em;
    font-weight: 700;
    color: #2d3748;
    margin-bottom: 25px;
    position: relative;
    padding-bottom: 12px;
    letter-spacing: -0.5px;
}

.about-section-title::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 60px;
    height: 3px;
    background: #1e3a8a;
    border-radius: 2px;
}

/* Content Cards */
.about-content {
    font-size: 1.05em;
    color: #4a5568;
    background: #ffffff;
    margin-bottom: 25px;
    padding: 28px;
    border-radius: 16px;
    border: 1px solid #e2e8f0;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
    transition: all 0.3s ease;
}

.about-content:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(30, 58, 138, 0.1);
}

.about-content strong {
    color: #1e3a8a;
    font-weight: 600;
}

/* Research Areas Grid */
.research-areas {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 24px;
    margin: 35px 0;
}

.research-card {
    background: #ffffff;
    padding: 28px;
    border-radius: 16px;
    border: 1px solid #e2e8f0;
    transition: all 0.3s ease;
    cursor: pointer;
    position: relative;
    overflow: hidden;
}

.research-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 4px;
    background: #1e3a8a;
    transform: scaleX(0);
    transition: transform 0.4s ease;
    transform-origin: left;
}

.research-card:hover::before {
    transform: scaleX(1);
}

.research-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(30, 58, 138, 0.15);
}

.research-card-title {
    font-weight: 700;
    color: #2d3748;
    font-size: 1.15em;
    margin-bottom: 12px;
}

.research-card-content {
    color: #718096;
    font-size: 0.95em;
    line-height: 1.7;
}

/* Professional Journey Timeline */
.journey-timeline {
    position: relative;
    margin: 35px 0;
    padding-left: 50px;
}

.journey-timeline::before {
    content: '';
    position: absolute;
    left: 20px;
    top: 0;
    bottom: 0;
    width: 2px;
    background: linear-gradient(180deg, #1e3a8a 0%, #3b82f6 100%);
    border-radius: 1px;
}

.timeline-item {
    position: relative;
    margin-bottom: 35px;
    background: #ffffff;
    padding: 24px;
    border-radius: 16px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
    border: 1px solid #e2e8f0;
    transition: all 0.3s ease;
}

.timeline-item:hover {
    transform: translateX(8px);
    box-shadow: 0 10px 30px rgba(30, 58, 138, 0.15);
}

.timeline-item::before {
    content: '';
    position: absolute;
    left: -36px;
    top: 28px;
    width: 12px;
    height: 12px;
    background: #1e3a8a;
    border-radius: 50%;
    box-shadow: 0 0 0 4px #ffffff, 0 0 0 6px rgba(30, 58, 138, 0.2);
    z-index: 1;
}

.timeline-title {
    font-weight: 700;
    color: #1e3a8a;
    margin-bottom: 6px;
    font-size: 1.15em;
}

.timeline-period {
    color: #a0aec0;
    font-size: 0.9em;
    margin-bottom: 12px;
    font-weight: 500;
}

.timeline-content {
    color: #4a5568;
    font-size: 0.95em;
    line-height: 1.7;
}

.timeline-content ul {
    margin-top: 12px;
    margin-left: 0;
    padding-left: 20px;
}

.timeline-content ul li {
    margin-bottom: 8px;
    position: relative;
}

.timeline-content ul li::before {
    content: '▸';
    position: absolute;
    left: -18px;
    color: #1e3a8a;
    font-weight: 600;
}

/* Skills Grid */
.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
    margin: 35px 0;
}

.skill-category {
    background: #ffffff;
    padding: 24px;
    border-radius: 16px;
    border: 1px solid #e2e8f0;
    transition: all 0.3s ease;
}

.skill-category:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(30, 58, 138, 0.15);
}

.skill-category-title {
    font-weight: 700;
    color: #1e3a8a;
    margin-bottom: 14px;
    font-size: 1.1em;
}

.skill-list {
    color: #4a5568;
    font-size: 0.95em;
    line-height: 1.8;
}

/* Achievement Grid */
.achievement-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
    margin: 30px 0;
}

.achievement-item {
    background: linear-gradient(135deg, #fbbf24 0%, #f59e0b 100%);
    padding: 20px;
    border-radius: 14px;
    font-size: 0.95em;
    color: #2d3748;
    font-weight: 500;
    box-shadow: 0 4px 15px rgba(251, 191, 36, 0.2);
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}

.achievement-item::before {
    content: '★';
    position: absolute;
    top: 10px;
    right: 15px;
    font-size: 20px;
    opacity: 0.3;
}

.achievement-item:hover {
    transform: translateY(-3px);
    box-shadow: 0 8px 25px rgba(251, 191, 36, 0.3);
}

.achievement-year {
    font-weight: 800;
    color: #1a1a1a;
    margin-right: 8px;
}

/* Contact Section */
.contact-info {
    background: rgba(30, 58, 138, 0.08);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    padding: 35px;
    border-radius: 20px;
    text-align: center;
    margin-top: 45px;
    border: 1px solid rgba(30, 58, 138, 0.15);
    box-shadow: 0 10px 30px rgba(30, 58, 138, 0.05);
}

.contact-info a {
    color: #1e3a8a;
    text-decoration: none;
    font-weight: 600;
    padding: 8px 16px;
    margin: 0 5px;
    border-radius: 8px;
    border: 1px solid rgba(30, 58, 138, 0.2);
    transition: all 0.3s ease;
    display: inline-block;
}

.contact-info a:hover {
    background: rgba(30, 58, 138, 0.1);
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(30, 58, 138, 0.1);
    border-color: rgba(30, 58, 138, 0.3);
}

/* Animations */
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

/* Loading animation for sections */
.about-section:nth-child(2) { animation-delay: 0.1s; }
.about-section:nth-child(3) { animation-delay: 0.2s; }
.about-section:nth-child(4) { animation-delay: 0.3s; }
.about-section:nth-child(5) { animation-delay: 0.4s; }
.about-section:nth-child(6) { animation-delay: 0.5s; }
.about-section:nth-child(7) { animation-delay: 0.6s; }
.about-section:nth-child(8) { animation-delay: 0.7s; }

/* Responsive Design */
@media (max-width: 768px) {
    .about-intro {
        padding: 25px;
        font-size: 1em;
    }
    
    .research-areas, .skills-grid, .achievement-grid {
        grid-template-columns: 1fr;
    }
    
    .journey-timeline {
        padding-left: 40px;
    }
    
    .journey-timeline::before {
        left: 15px;
    }
    
    .timeline-item {
        padding: 20px;
    }
    
    .timeline-item::before {
        left: -28px;
    }
    
    .about-section-title {
        font-size: 1.3em;
    }
    
    .contact-info a {
        display: block;
        margin: 8px auto;
        max-width: 200px;
    }
}
</style>

<div class="about-container">
    
    <div class="about-intro">
        I am a <span class="highlight">Research Scientist Intern</span> at <span class="highlight">Meta Reality Labs Research</span> and a <span class="highlight">Ph.D. candidate in Mechanical Engineering</span> at Georgia Institute of Technology. With over 10 years of experience spanning academia and industry, I specialize in mechanical design, hardware development, and sensor integration for advanced applications in robotics, AR/VR, and medical ultrasound therapy. My unique background combines deep expertise in acoustics, vibration analysis, and multi-physics simulation with hands-on experience in translating research prototypes into manufacturable products.
    </div>

    <div class="about-section">
        <div class="about-section-title">Current Research</div>
        <div class="about-content">
            At <strong>Meta Reality Labs Research</strong>, I'm developing next-generation ultrasound-based sensing technologies for AR/VR wearable systems, focusing on high-performance sensor design and real-time signal processing algorithms. My doctoral research at Georgia Tech investigates <strong>transcranial focused ultrasound therapy</strong> and <strong>ultrasound system design</strong>, where I've developed novel acoustic hologram systems and fast parallelized models for skull aberration correction and neuro-navigation based on nonlinear acoustics
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Research Areas</div>
        <div class="research-areas">
            <div class="research-card">
                <div class="research-card-title">
                    Advanced Sensing Systems
                </div>
                <div class="research-card-content">
                    Designing and prototyping ultrasound-based sensors for AR/VR applications, developing tactile and force sensing technologies for robotics and wearables, with expertise in sensor characterization and performance optimization.
                </div>
            </div>
            <div class="research-card">
                <div class="research-card-title">
                    Transcranial Ultrasound Therapy
                </div>
                <div class="research-card-content">
                    Developing acoustic hologram-based systems for non-invasive brain therapy, implementing heterogeneous angular spectrum approaches for skull aberration correction, and advancing parametric array techniques for trans-skull monitoring.
                </div>
            </div>
            <div class="research-card">
                <div class="research-card-title">
                    Vibroacoustic Modeling
                </div>
                <div class="research-card-content">
                    Applying wave simulation and structural acoustics to complex systems, from tire NVH analysis to neuromodulation biophysics. Expertise in modal testing, transducer characterization, and multi-physics simulation.
                </div>
            </div>
            <div class="research-card">
                <div class="research-card-title">
                    Scientific Machine Learning
                </div>
                <div class="research-card-content">
                    Integrating AI/ML techniques with acoustic modeling for intelligent electromechanical design, implementing data-driven approaches for signal processing and system optimization in sensing applications.
                </div>
            </div>
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Professional Journey</div>
        <div class="journey-timeline">
            <div class="timeline-item">
                <div class="timeline-title">Research Scientist Intern - Meta Reality Labs</div>
                <div class="timeline-period">May 2025 - Present</div>
                <div class="timeline-content">
                    Leading development of cutting-edge ultrasound sensing technologies for next-generation AR/VR systems. Collaborating with cross-functional teams to solve complex technical challenges in sensor physics and real-time signal processing.
                </div>
            </div>
            <div class="timeline-item">
                <div class="timeline-title">Graduate Research Assistant - Georgia Tech</div>
                <div class="timeline-period">2020 - Present</div>
                <div class="timeline-content">
                    Pioneering research in transcranial ultrasound therapy and neuromodulation. Key achievements include:
                    <ul>
                        <li>Developed fast parallelized acoustic propagation models for skull aberration correction</li>
                        <li>Designed acoustic hologram systems accounting for skull heterogeneity</li>
                        <li>Investigated mechanical and acoustic interactions with neuronal circuits</li>
                    </ul>
                </div>
            </div>
            <div class="timeline-item">
                <div class="timeline-title">Senior Design Engineer - Bajaj Auto Ltd.</div>
                <div class="timeline-period">2015 - 2018</div>
                <div class="timeline-content">
                    Led powertrain integration and NVH optimization for automotive systems with 3+ years of industry experience in:
                    <ul>
                        <li>Hardware design (DFM/DFA) and product validation</li>
                        <li>Psychoacoustic tuning of exhaust systems</li>
                        <li>Vibration modeling and predictive analytics</li>
                        <li>Design failure analysis and reliability enhancement</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Technical Expertise</div>
        <div class="skills-grid">
            <div class="skill-category">
                <div class="skill-category-title">Core Competencies</div>
                <div class="skill-list">
                    Wave simulation & acoustic modeling • Hardware prototyping • Digital signal processing • Modal testing • Sensor integration • Noise & vibration analysis • AI/ML applications in acoustics
                </div>
            </div>
            <div class="skill-category">
                <div class="skill-category-title">Design & CAD</div>
                <div class="skill-list">
                    SolidWorks • Siemens NX • AutoCAD • GD&T • Design for Manufacturing (DFM/DFA) • Rapid prototyping • Product validation
                </div>
            </div>
            <div class="skill-category">
                <div class="skill-category-title">Analysis & Simulation</div>
                <div class="skill-list">
                    COMSOL • HyperMesh • ANSYS • Adams • ME'Scope • Finite Element Modeling (FEM) • Multi-physics simulation
                </div>
            </div>
            <div class="skill-category">
                <div class="skill-category-title">Programming</div>
                <div class="skill-list">
                    Python • MATLAB • Simulink • Scientific computing • Data processing • Real-time signal analysis • Algorithm development
                </div>
            </div>
        </div>
    </div>




    <div class="about-section">
        <div class="about-section-title">Research Philosophy</div>
        <div class="about-content">
            My research philosophy centers on bridging fundamental scientific understanding with practical engineering solutions. Whether developing breakthrough medical technologies or advancing consumer electronics, I combine <strong>rigorous experimentation</strong> with <strong>high-fidelity computational modeling</strong> to tackle complex challenges. My interdisciplinary background enables me to approach problems from multiple perspectives, creating innovative solutions that transition from laboratory prototypes to real-world applications. I believe the most impactful research occurs at the intersection of disciplines, where insights from acoustics, mechanics, materials science, and data science converge to solve society's most pressing challenges.
        </div>
    </div>

    <div class="contact-info">
        <div style="font-size: 1.2em; margin-bottom: 15px; font-weight: 700; color: #1e3a8a;">
            Let's Connect
        </div>
        <div>
            <a href="mailto:ppdash@gatech.edu">✉ Email</a>
            <a href="https://linkedin.com/in/ppdash" target="_blank">💼 LinkedIn</a>
            <a href="https://pradosh-dash.github.io/" target="_blank">🌐 Portfolio</a>
        </div>
    </div>
</div>
