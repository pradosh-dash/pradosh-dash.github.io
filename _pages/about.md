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
    background: rgba(255, 255, 255, 0.7);
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
    background: rgba(255, 255, 255, 0.7);
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
    background: rgba(255, 255, 255, 0.7);
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
    box-shadow: 0 0 0 4px rgba(255, 255, 255, 0.7), 0 0 0 6px rgba(30, 58, 138, 0.2);
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
    background: rgba(255, 255, 255, 0.7);
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
        I am a <span class="highlight">Ph.D. in Mechanical Engineering</span> from Georgia Institute of Technology and recently a <span class="highlight">Research Scientist Intern</span> at <span class="highlight">Meta Reality Labs Research</span>. With over 10 years of experience spanning academia and industry, I specialize in ultrasound system development, from multi-channel transducer array design and beamforming optimization to GPU-accelerated wave propagation simulation and real-time signal processing. My work bridges nonlinear acoustics in heterogeneous media with practical wearable sensing and medical ultrasound therapy applications, combining rigorous computational modeling with hands-on hardware prototyping and embedded DSP.
    </div>

    <div class="about-section">
        <div class="about-section-title">Current Research</div>
        <div class="about-content">
            At Meta Reality Labs Research, I developed next-generation wearable ultrasound sensing technologies for AR/VR systems, working on compact transducer arrays for strain imaging, building real-time signal processing pipelines, and implementing Doppler-based motion rejection algorithms for robust sensing in dynamic environments. My doctoral research at Georgia Tech investigated transcranial focused ultrasound therapy using lensed as phased array based ultrasound systems, where I developed GPU-accelerated aberration correction algorithms, optimized acoustic hologram topologies through heterogeneous skull bone, and volumetric trasn-skull passive acoustic mapping and image reconstruction.
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Research Areas</div>
        <div class="research-areas">
            <div class="research-card">
                <div class="research-card-title">
                    Wearable Ultrasound Sensing
                </div>
                <div class="research-card-content">
                    Designing and prototyping wearable ultrasound transducer arrays for AR/VR platforms. Expertise in multi-channel system optimization, beamforming parameter tuning, Doppler-based motion rejection, and SVD-based clutter filtering for high-sensitivity physiological monitoring.
                </div>
            </div>
            <div class="research-card">
                <div class="research-card-title">
                    Transcranial Ultrasound Therapy
                </div>
                <div class="research-card-content">
                    Developing acoustic hologram-based systems for non-invasive brain therapy using Verasonics multi-channel platforms. Implementing heterogeneous angular spectrum approaches for skull aberration correction, beamforming sequence optimization, and parametric array techniques for trans-skull monitoring.
                </div>
            </div>
            <div class="research-card">
                <div class="research-card-title">
                    Signal & Image Processing
                </div>
                <div class="research-card-content">
                    SVD-based spatiotemporal filtering, strain imaging and elastography, Doppler flow processing, advanced beamforming (delay-and-sum, angular spectrum), and ultrafast high-frame-rate acquisition for transient event capture and volumetric image reconstruction.
                </div>
            </div>
            <div class="research-card">
                <div class="research-card-title">
                    Vibroacoustic Modeling & NVH
                </div>
                <div class="research-card-content">
                    Experimental modal analysis, structural noise transfer path quantification, and active noise control with embedded DSP. Industry experience in powertrain NVH optimization, psychoacoustic tuning, and real-time adaptive filtering (FxLMS) on TMS320 platforms.
                </div>
            </div>
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Professional Journey</div>
        <div class="journey-timeline">
            <div class="timeline-item">
                <div class="timeline-title">Research Scientist Intern,  Meta Reality Labs Research</div>
                <div class="timeline-period">May 2025 – Nov 2025</div>
                <div class="timeline-content">
                    Developed and ehanced ultrasonic sensing modalitties for robotic and AR/VR platforms. Key contributions include:
                    <ul>
                        <li>Beamforming parameter tuning and multi-channel ultrasound imaging system performance benchmarking</li>
                        <li>Doppler-based motion rejection algorithms for robust wearable sensing</li>
                        <li>SVD-based signal filtering for clutter suppression and SNR enhancement</li>
                        <li>Cross-functional collaboration with hardware, firmware, and algorithm teams</li>
                    </ul>
                </div>
            </div>
            <div class="timeline-item">
                <div class="timeline-title">Graduate Research Assistant,  Georgia Tech</div>
                <div class="timeline-period">2020 – 2025</div>
                <div class="timeline-content">
                    Ph.D. research in transcranial focused ultrasound therapy and neuromodulation biophysics. Key achievements:
                    <ul>
                        <li>GPU-accelerated nonlinear wave propagation simulations for heterogeneous skull bone</li>
                        <li>Fast aberration correction algorithms using differentiable acoustic propagators and Verasonics arrays</li>
                        <li>Acoustic hologram topology optimization for improved spatial targeting and image reconstruction</li>
                        <li>Ultrafast acquisition for capturing transient neural responses in neuromodulation studies</li>
                    </ul>
                </div>
            </div>
            <div class="timeline-item">
                <div class="timeline-title">Graduate Research Assistant,  Virginia Tech</div>
                <div class="timeline-period">2018 – 2020</div>
                <div class="timeline-content">
                    M.S. research in vibroacoustic modeling and structural dynamics in the Vibration and Acoustics Laboratory. Key contributions:
                    <ul>
                        <li>Experimental modal analysis of rolling tires using laser vibrometry and accelerometer arrays for structure-borne noise prediction</li>
                        <li>Quantified structural noise and vibration transfer paths under realistic operating conditions</li>
                        <li>Designed a semi-active tuned absorber to reduce rest tremors in Parkinson's patients</li>
                    </ul>
                </div>
            </div>
            <div class="timeline-item">
                <div class="timeline-title">Senior Design Engineer,  Bajaj Auto Ltd.</div>
                <div class="timeline-period">2015 – 2018</div>
                <div class="timeline-content">
                    Led powertrain NVH optimization and active noise control system development with 3+ years of industry experience:
                    <ul>
                        <li>Embedded DSP implementation (TMS320) for real-time active noise cancellation</li>
                        <li>FxLMS adaptive filtering achieving 10 dB attenuation in engine intake noise</li>
                        <li>End-to-end hardware prototyping, testing, and product validation</li>
                        <li>Psychoacoustic tuning and pass-by-noise regulatory compliance</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Technical Expertise</div>
        <div class="skills-grid">
            <div class="skill-category">
                <div class="skill-category-title">Ultrasound Systems</div>
                <div class="skill-list">
                    Multi-channel array systems (Verasonics) • Beamforming & sequence optimization • Transducer characterization • Aberration correction • Passive acoustic mapping • Ultrafast imaging
                </div>
            </div>
            <div class="skill-category">
                <div class="skill-category-title">Signal & Image Processing</div>
                <div class="skill-list">
                    SVD-based spatiotemporal filtering • Strain imaging / elastography • Doppler processing & motion rejection • Digital Image Correlation (DIC) • Adaptive filtering (FxLMS)
                </div>
            </div>
            <div class="skill-category">
                <div class="skill-category-title">Simulation & Analysis</div>
                <div class="skill-list">
                    GPU-accelerated nonlinear wave propagation • FEM (COMSOL, Ansys, HyperMesh) • Multiphysics modeling • MATLAB/Simulink
                </div>
            </div>
            <div class="skill-category">
                <div class="skill-category-title">Programming & Hardware</div>
                <div class="skill-list">
                    Python • MATLAB • C/C++ (embedded DSP & hardware) • Simulink • Sensor prototyping • Signal acquisition (ADC/DAC) • CAD (SolidWorks, Siemens NX)
                </div>
            </div>
            <div class="skill-category">
                <div class="skill-category-title">Vibroacoustic Modeling</div>
                <div class="skill-list">
                    Experimental modal analysis • Laser vibrometry • Structure-borne noise prediction • Noise transfer path analysis • Active Noise Control (ANC) • Psychoacoustic tuning • NVH optimization
                </div>
            </div>
            <div class="skill-category">
                <div class="skill-category-title">Scientific Machine Learning</div>
                <div class="skill-list">
                    Data-driven acoustic modeling • Differentiable physics simulators • Machine vision • Imaging with learned models • Optimization techniques • Model order reduction
                </div>
            </div>
        </div>
    </div>

    <div class="about-section">
        <div class="about-section-title">Research Philosophy</div>
        <div class="about-content">
            My research philosophy centers on bridging fundamental wave physics with practical engineering solutions. Whether developing wearable ultrasound sensors or advancing non-invasive brain therapies, I combine <strong>rigorous experimentation</strong> with <strong>high-fidelity computational modeling</strong> to tackle complex challenges. My interdisciplinary background — spanning nonlinear acoustics, multi-channel array systems, embedded DSP, and signal processing — enables me to approach problems end-to-end, from transducer design through algorithm development to system validation. I believe the most impactful research emerges at the intersection of disciplines, and I thrive in collaborative environments that bring together academic researchers and industry partners.
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
