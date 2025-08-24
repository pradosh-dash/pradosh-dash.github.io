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
.about-container {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.7;
    color: #333;
    max-width: 800px;
}

.about-intro {
    font-size: 1.2em;
    color: #2d3748;
    margin-bottom: 30px;
    padding: 25px;
    background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
    border-radius: 10px;
    border-left: 5px solid #2c5282;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.about-section {
    margin: 30px 0;
}

.about-section-title {
    font-size: 1.4em;
    font-weight: bold;
    color: #2c5282;
    margin-bottom: 15px;
    padding-bottom: 8px;
    border-bottom: 2px solid #e2e8f0;
}

.about-content {
    font-size: 1.05em;
    color: #4a5568;
    margin-bottom: 20px;
}

.research-areas {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
    margin: 25px 0;
}

.research-card {
    background-color: #f8f9fa;
    padding: 20px;
    border-radius: 8px;
    border-left: 4px solid #2c5282;
    box-shadow: 0 2px 6px rgba(0,0,0,0.08);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.research-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}

.research-card-title {
    font-weight: bold;
    color: #2c5282;
    font-size: 1.1em;
    margin-bottom: 8px;
}

.research-card-content {
    color: #4a5568;
    font-size: 0.95em;
    line-height: 1.6;
}

.journey-timeline {
    position: relative;
    margin: 30px 0;
    padding-left: 30px;
}

.journey-timeline::before {
    content: '';
    position: absolute;
    left: 15px;
    top: 0;
    bottom: 0;
    width: 2px;
    background: linear-gradient(to bottom, #2c5282, #e2e8f0);
}

.timeline-item {
    position: relative;
    margin-bottom: 25px;
    background-color: #f8f9fa;
    padding: 15px 20px;
    border-radius: 8px;
    margin-left: 20px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.08);
}

.timeline-item::before {
    content: '';
    position: absolute;
    left: -35px;
    top: 20px;
    width: 12px;
    height: 12px;
    background-color: #2c5282;
    border-radius: 50%;
    border: 3px solid #fff;
    box-shadow: 0 0 0 3px #2c5282;
}

.timeline-title {
    font-weight: bold;
    color: #2c5282;
    margin-bottom: 5px;
}

.timeline-period {
    color: #718096;
    font-size: 0.9em;
    font-style: italic;
    margin-bottom: 8px;
}

.timeline-content {
    color: #4a5568;
    font-size: 0.95em;
    line-height: 1.6;
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 15px;
    margin: 25px 0;
}

.skill-category {
    background-color: #f8f9fa;
    padding: 15px;
    border-radius: 8px;
    border-left: 4px solid #2c5282;
}

.skill-category-title {
    font-weight: bold;
    color: #2c5282;
    margin-bottom: 8px;
    font-size: 1.05em;
}

.skill-list {
    color: #4a5568;
    font-size: 0.95em;
    line-height: 1.5;
}

.highlight {
    color: #2c5282;
    font-weight: 600;
}

.contact-info {
    background: linear-gradient(135deg, #2c5282 0%, #3d5a9c 100%);
    color: white;
    padding: 25px;
    border-radius: 10px;
    text-align: center;
    margin-top: 30px;
}

.contact-info a {
    color: #bee3f8;
    text-decoration: none;
    font-weight: 500;
}

.contact-info a:hover {
    color: white;
    text-decoration: underline;
}

@media (max-width: 768px) {
    .about-intro {
        font-size: 1.1em;
        padding: 20px;
    }
    
    .research-areas {
        grid-template-columns: 1fr;
    }
    
    .skills-grid {
        grid-template-columns: 1fr;
    }
    
    .journey-timeline {
        padding-left: 20px;
    }
    
    .timeline-item {
        margin-left: 15px;
    }
    
    .timeline-item::before {
        left: -30px;
    }
}
</style>

<div class="about-container">
    
    <div class="about-intro">
        I am a <span class="highlight">Research Scientist Intern at Meta Reality Labs Research</span> and a <span class="highlight">Ph.D. candidate in Mechanical Engineering</span> at the Georgia Institute of Technology. My work spans soft wearable technologies, acoustic sensing for AR/VR and robotics, and transcranial focused ultrasound for imaging and neuromodulation using nonlinear acoustics. Combining rigorous experimentation with high-fidelity simulations, I investigate skull–brain dynamics and develop acoustic-hologram systems with fast, parallelized models for skull aberration correction.
    </div>

    <div class="about-section">
        <div class="about-section-title">Research Focus</div>
        <div class="research-areas">
            <div class="research-card">
                <div class="research-card-title">Wearable Acoustic Technologies</div>
                <div class="research-card-content">
                    Developing next-generation soft wearable technologies and high-performance acoustic-based sensors for AR/VR integration and applied robotics at Meta Reality Labs Research.
                </div>
            </div>
            
            <div class="research-card">
                <div class="research-card-title">Transcranial Focused Ultrasound</div>
                <div class="research-card-content">
                    Advancing imaging and neuromodulation techniques using nonlinear acoustics, with focus on skull-brain dynamics and acoustic-hologram systems for therapeutic applications.
                </div>
            </div>
            
            <div class="research-card">
                <div class="research-card-title">Computational Acoustics</div>
                <div class="research-card-content">
                    Creating fast, parallelized acoustic propagation models for skull aberration correction, combining high-fidelity simulations with experimental validation.
                </div>
            </div>
            
            <div class="research-card">
                <div class="research-card-title">Vibroacoustics & NVH</div>
                <div class="research-card-content">
                    Expertise in structural acoustics, vibration analysis, and noise control from automotive industry experience and academic research on tire dynamics.
                </div>
            </div>
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Academic & Professional Journey</div>
        <div class="journey-timeline">
            <div class="timeline-item">
                <div class="timeline-title">Research Scientist Intern - Meta Reality Labs Research</div>
                <div class="timeline-period">May 2025 - Present</div>
                <div class="timeline-content">
                    Developing soft wearable technologies and acoustic-based sensors for AR/VR integration, collaborating with interdisciplinary teams on next-generation sensing solutions.
                </div>
            </div>
            
            <div class="timeline-item">
                <div class="timeline-title">Ph.D. Candidate - Georgia Institute of Technology</div>
                <div class="timeline-period">2020 - Present</div>
                <div class="timeline-content">
                    Research focus on transcranial focused ultrasound therapy and neuromodulation using nonlinear acoustics. Developing acoustic hologram systems and parallelized models for skull aberration correction.
                </div>
            </div>
            
            <div class="timeline-item">
                <div class="timeline-title">M.S. in Mechanical Engineering - Virginia Tech</div>
                <div class="timeline-period">2018 - 2020</div>
                <div class="timeline-content">
                    Specialized in tire vibroacoustics and structure-borne noise prediction. Developed experimental modal analysis procedures for rolling tire conditions and designed tuned absorbers for medical applications.
                </div>
            </div>
            
            <div class="timeline-item">
                <div class="timeline-title">Senior Design Engineer - Bajaj Auto Ltd.</div>
                <div class="timeline-period">2015 - 2018</div>
                <div class="timeline-content">
                    Led engine design and noise, vibration, and harshness (NVH) engineering projects. Optimized powertrain systems, conducted durability testing, and developed advanced vibration analysis methodologies for automotive applications.
                </div>
            </div>
            
            <div class="timeline-item">
                <div class="timeline-title">B.Tech. in Mechanical Engineering - NIT Rourkela</div>
                <div class="timeline-period">2011 - 2015</div>
                <div class="timeline-content">
                    University Gold Medalist with research in MEMS accelerometer design. Recognized by the President of India for academic excellence and research innovation.
                </div>
            </div>
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Technical Expertise</div>
        <div class="skills-grid">
            <div class="skill-category">
                <div class="skill-category-title">Computational Methods</div>
                <div class="skill-list">
                    Wave simulation, acoustic modeling, finite element analysis (COMSOL, Ansys), numerical acoustics, parallelized algorithms, MATLAB, Python
                </div>
            </div>
            
            <div class="skill-category">
                <div class="skill-category-title">Experimental Techniques</div>
                <div class="skill-list">
                    Acoustic transducer characterization, modal testing, laser vibrometry, digital signal processing, hardware prototyping, data acquisition systems
                </div>
            </div>
            
            <div class="skill-category">
                <div class="skill-category-title">Design & Development</div>
                <div class="skill-list">
                    CAD modeling (SolidWorks, Siemens NX), mechanical design, sensor development, wearable technologies, acoustic system design
                </div>
            </div>
            
            <div class="skill-category">
                <div class="skill-category-title">Specialized Applications</div>
                <div class="skill-list">
                    Transcranial ultrasound, AR/VR sensing, neuromodulation, automotive NVH, psychoacoustics, medical device development
                </div>
            </div>
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Research Philosophy</div>
        <div class="about-content">
            My research approach combines <strong>rigorous experimentation</strong> with <strong>high-fidelity computational modeling</strong> to tackle complex challenges in acoustics and mechanical engineering. I believe in bridging fundamental scientific understanding with practical engineering solutions, whether developing breakthrough medical technologies or advancing consumer electronics. My interdisciplinary background—spanning academic research, industry experience, and cutting-edge technology development—enables me to approach problems from multiple perspectives and create innovative solutions that have real-world impact.
        </div>
    </div>

    <div class="contact-info">
        <div style="font-size: 1.1em; margin-bottom: 10px;">
            <strong>Let's Connect</strong>
        </div>
        <div>
            <a href="mailto:ppdash@gatech.edu">ppdash@gatech.edu</a> | 
            <a href="https://linkedin.com/in/ppdash" target="_blank">LinkedIn</a>
            {% if site.author.googlescholar %}
             | <a href="{{ site.author.googlescholar }}" target="_blank">Google Scholar</a>
            {% endif %}
        </div>
    </div>

</div>
