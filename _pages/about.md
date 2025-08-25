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
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    line-height: 1.6;
    color: #333;
    max-width: 900px;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

.about-intro {
    font-size: 1.05em;
    color: #1a1a1a;
    background: #ffffff;
    margin-bottom: 25px;
    padding: 20px;
    border-radius: 6px;
    border: 1px solid #e8e8e8;
    border-left: 3px solid #4a4a4a;
    animation: fadeIn 0.5s ease-out;
}

.about-section {
    margin: 30px 0;
}

.about-section-title {
    font-size: 1.3em;
    font-weight: 600;
    color: #1a1a1a;
    margin-bottom: 15px;
    padding-bottom: 8px;
    border-bottom: 2px solid #e5e5e5;
    letter-spacing: -0.3px;
}

.about-content {
    font-size: 1em;
    color: #333;
    background: #ffffff;
    margin-bottom: 25px;
    padding: 18px 20px;
    border-radius: 6px;
    border: 1px solid #e8e8e8;
    border-left: 3px solid #5a5a5a;
    line-height: 1.7;
}

.research-areas {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 18px;
    margin: 25px 0;
}

.research-card {
    background: #ffffff;
    padding: 16px 18px;
    border-radius: 6px;
    border: 1px solid #e8e8e8;
    border-left: 3px solid #6a6a6a;
    margin-bottom: 12px;
    transition: all 0.2s ease;
}

.research-card:hover {
    border-left-width: 4px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.06);
}

.research-card-title {
    font-weight: 600;
    color: #1a1a1a;
    font-size: 1.05em;
    margin-bottom: 8px;
}

.research-card-content {
    color: #606060;
    font-size: 0.95em;
    line-height: 1.6;
}

.journey-timeline {
    position: relative;
    margin: 25px 0;
    padding-left: 25px;
}

.journey-timeline::before {
    content: '';
    position: absolute;
    left: 12px;
    top: 0;
    bottom: 0;
    width: 1px;
    background-color: #d0d0d0;
}

.timeline-item {
    position: relative;
    margin-bottom: 20px;
    background: #ffffff;
    padding: 16px 18px;
    border-radius: 6px;
    border: 1px solid #e8e8e8;
    margin-left: 20px;
    transition: all 0.2s ease;
}

.timeline-item:hover {
    box-shadow: 0 2px 6px rgba(0,0,0,0.06);
}

.timeline-item::before {
    content: '';
    position: absolute;
    left: -28px;
    top: 18px;
    width: 8px;
    height: 8px;
    background-color: #4a4a4a;
    border-radius: 50%;
    border: 2px solid #fff;
    box-shadow: 0 0 0 1px #d0d0d0;
}

.timeline-title {
    font-weight: 600;
    color: #1a1a1a;
    margin-bottom: 4px;
    font-size: 1.05em;
}

.timeline-period {
    color: #707070;
    font-size: 0.9em;
    margin-bottom: 8px;
}

.timeline-content {
    color: #606060;
    font-size: 0.95em;
    line-height: 1.6;
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 16px;
    margin: 25px 0;
}

.skill-category {
    background: #ffffff;
    padding: 16px 18px;
    border-radius: 6px;
    border: 1px solid #e8e8e8;
    border-left: 3px solid #7a7a7a;
    margin-bottom: 12px;
    transition: all 0.2s ease;
}

.skill-category:hover {
    border-left-width: 4px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.06);
}

.skill-category-title {
    font-weight: 600;
    color: #1a1a1a;
    margin-bottom: 10px;
    font-size: 1.05em;
}

.skill-list {
    color: #606060;
    font-size: 0.95em;
    line-height: 1.7;
}

.highlight {
    color: #1a1a1a;
    font-weight: 600;
    background: linear-gradient(180deg, transparent 60%, rgba(255, 215, 0, 0.15) 60%);
}

.about-content strong {
    color: #1a1a1a;
    font-weight: 600;
}

.contact-info {
    background: #2a2a2a;
    color: white;
    padding: 22px;
    border-radius: 6px;
    text-align: center;
    margin-top: 30px;
    border: 1px solid #1a1a1a;
}

.contact-info a {
    color: #f0f0f0;
    text-decoration: none;
    font-weight: 500;
    padding: 0 3px;
    transition: all 0.15s ease;
}

.contact-info a:hover {
    color: white;
    background: rgba(255, 255, 255, 0.1);
    border-radius: 3px;
}

/* Subtle animations */
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(5px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.about-intro, .about-content, .research-card, .timeline-item, .skill-category {
    animation: fadeIn 0.5s ease-out;
}

/* Responsive design */
@media (max-width: 768px) {
    .about-container {
        max-width: 100%;
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
        padding: 14px;
    }
    
    .timeline-item::before {
        left: -23px;
    }
    
    .about-intro, .about-content {
        padding: 16px;
    }
    
    .about-section-title {
        font-size: 1.2em;
    }
}

/* Print styles */
@media print {
    .about-intro, .about-content, .research-card, .timeline-item, .skill-category {
        border: 1px solid #d0d0d0;
        box-shadow: none;
    }
    
    .contact-info {
        background: white;
        color: #1a1a1a;
        border: 2px solid #1a1a1a;
    }
    
    .contact-info a {
        color: #1a1a1a;
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
<!--
    <div class="contact-info">
        <div style="font-size: 1.0em; margin-bottom: 10px;">
            <strong>Let's Connect</strong>
        </div>
        <div>
            <a href="mailto:ppdash@gatech.edu">Email</a> | 
            <a href="https://linkedin.com/in/ppdash" target="_blank">LinkedIn</a>
        </div>
    </div>
    -->
    </div>


