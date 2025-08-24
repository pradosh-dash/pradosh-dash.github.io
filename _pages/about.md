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
    line-height: 1.6;
    color: #333;
    max-width: 800px;
}

.about-intro {
    font-size: 1.1em;
    color: #333;
    margin-bottom: 30px;
    padding: 20px;
    background-color: #f8f9fa;
    border-radius: 8px;
    border-left: 4px solid #343a40;
}

.about-section {
    margin: 25px 0;
}

.about-section-title {
    font-size: 1.2em;
    font-weight: 600;
    color: #343a40;
    margin-bottom: 15px;
    padding-bottom: 5px;
    border-bottom: 1px solid #dee2e6;
}

.about-content {
    font-size: 1em;
    color: #555;
    margin-bottom: 15px;
}

.research-areas {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
    margin: 25px 0;
}

.research-card {
    background-color: #f8f9fa;
    padding: 15px;
    border-radius: 5px;
    border-left: 3px solid #6c757d;
    margin-bottom: 15px;
}

.research-card:hover {
    border-left-color: #343a40;
}

.research-card-title {
    font-weight: 600;
    color: #343a40;
    font-size: 1em;
    margin-bottom: 8px;
}

.research-card-content {
    color: #555;
    font-size: 0.95em;
    line-height: 1.5;
}

.journey-timeline {
    position: relative;
    margin: 20px 0;
    padding-left: 20px;
}

.journey-timeline::before {
    content: '';
    position: absolute;
    left: 10px;
    top: 0;
    bottom: 0;
    width: 1px;
    background-color: #dee2e6;
}

.timeline-item {
    position: relative;
    margin-bottom: 20px;
    background-color: #f8f9fa;
    padding: 15px;
    border-radius: 5px;
    margin-left: 15px;
}

.timeline-item::before {
    content: '';
    position: absolute;
    left: -25px;
    top: 15px;
    width: 8px;
    height: 8px;
    background-color: #343a40;
    border-radius: 50%;
    border: 2px solid #fff;
}

.timeline-title {
    font-weight: 600;
    color: #343a40;
    margin-bottom: 3px;
    font-size: 1em;
}

.timeline-period {
    color: #6c757d;
    font-size: 0.9em;
    font-style: italic;
    margin-bottom: 8px;
}

.timeline-content {
    color: #555;
    font-size: 0.95em;
    line-height: 1.5;
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
    border-radius: 5px;
    border-left: 3px solid #6c757d;
    margin-bottom: 15px;
}

.skill-category-title {
    font-weight: 600;
    color: #343a40;
    margin-bottom: 8px;
    font-size: 1em;
}

.skill-list {
    color: #555;
    font-size: 0.95em;
    line-height: 1.5;
}

.highlight {
    color: #343a40;
    font-weight: 600;
}

.contact-info {
    background-color: #343a40;
    color: white;
    padding: 20px;
    border-radius: 5px;
    text-align: center;
    margin-top: 25px;
}

.contact-info a {
    color: #e9ecef;
    text-decoration: none;
    font-weight: normal;
}

.contact-info a:hover {
    color: white;
    text-decoration: underline;
}

@media (max-width: 768px) {
    .research-areas {
        grid-template-columns: 1fr;
    }
    
    .skills-grid {
        grid-template-columns: 1fr;
    }
    
    .journey-timeline {
        padding-left: 15px;
    }
    
    .timeline-item {
        margin-left: 10px;
    }
    
    .timeline-item::before {
        left: -20px;
    }
}
</style>

<div class="about-container">
    
    <div class="about-intro">
        I am a <span class="highlight">Research Scientist Intern at Meta Reality Labs Research</span> and a <span class="highlight">Ph.D. candidate in Mechanical Engineering</span> at the Georgia Institute of Technology. My work spans soft wearable technologies, acoustic sensing for AR/VR and robotics, and transcranial focused ultrasound for imaging and neuromodulation using nonlinear acoustics. Specifically, I investigate skull–brain dynamics and develop acoustic-hologram systems with fast, parallelized models for skull aberration correction.
    </div>


    <div class="about-section">
        <div class="about-section-title">Research Philosophy</div>
        <div class="about-content">
            My research approach combines <strong>rigorous experimentation</strong> with <strong>high-fidelity computational modeling</strong> to tackle complex challenges in acoustics and mechanical engineering. I believe in bridging fundamental scientific understanding with practical engineering solutions, whether developing breakthrough medical technologies or advancing consumer electronics. My interdisciplinary background—spanning academic research, industry experience, and cutting-edge technology development—enables me to approach problems from multiple perspectives and create innovative solutions that have real-world impact.
        </div>
    </div>

   
