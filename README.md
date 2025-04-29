<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aimable Mugwaneza | Cloud & DevOps Engineer</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    :root {
      --primary: #0099ff;
      --primary-dark: #0077cc;
      --secondary: #2d3748;
      --light: #f7fafc;
      --dark: #1a202c;
      --success: #48bb78;
      --warning: #f6ad55;
      --danger: #f56565;
      --gray-100: #f7fafc;
      --gray-200: #edf2f7;
      --gray-300: #e2e8f0;
      --gray-400: #cbd5e0;
      --gray-500: #a0aec0;
      --gray-600: #718096;
      --gray-700: #4a5568;
      --gray-800: #2d3748;
      --gray-900: #1a202c;
      --border-radius: 8px;
      --transition: all 0.3s ease;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background-color: var(--gray-100);
      color: var(--gray-800);
      line-height: 1.6;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 2rem;
    }

    header {
      text-align: center;
      padding: 3rem 0;
      background: linear-gradient(135deg, #0099ff 0%, #0077cc 100%);
      color: white;
      border-radius: var(--border-radius);
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      margin-bottom: 2rem;
      position: relative;
      overflow: hidden;
    }

    header::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-image: 
        radial-gradient(circle at 20% 80%, rgba(255, 255, 255, 0.1) 0%, transparent 20%),
        radial-gradient(circle at 80% 20%, rgba(255, 255, 255, 0.1) 0%, transparent 20%);
      opacity: 0.8;
    }

    h1, h2, h3, h4, h5, h6 {
      color: var(--secondary);
      margin-bottom: 1rem;
    }

    header h1, header h2, header h3 {
      color: white;
      position: relative;
      z-index: 2;
    }

    .profile-pic {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      border: 4px solid white;
      margin-bottom: 1rem;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      position: relative;
      z-index: 2;
      background-color: var(--gray-300);
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 0 auto 1rem auto;
    }

    .profile-pic i {
      font-size: 60px;
      color: var(--gray-600);
    }

    .section {
      background-color: white;
      border-radius: var(--border-radius);
      padding: 2rem;
      margin-bottom: 2rem;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
      transition: var(--transition);
    }

    .section:hover {
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      transform: translateY(-2px);
    }

    .section-title {
      display: flex;
      align-items: center;
      margin-bottom: 1.5rem;
      padding-bottom: 0.5rem;
      border-bottom: 2px solid var(--gray-200);
    }

    .section-title i {
      margin-right: 0.75rem;
      color: var(--primary);
      font-size: 1.5rem;
    }

    .tech-stack {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin-top: 1rem;
    }

    .category {
      margin-bottom: 1.5rem;
    }

    .badge-container {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-top: 0.5rem;
    }

    .badge {
      background-color: var(--gray-200);
      color: var(--gray-700);
      border-radius: 20px;
      padding: 0.25rem 0.75rem;
      font-size: 0.85rem;
      font-weight: 500;
      display: inline-flex;
      align-items: center;
      transition: var(--transition);
    }

    .badge i {
      margin-right: 0.25rem;
      font-size: 0.85rem;
    }

    .badge:hover {
      background-color: var(--primary);
      color: white;
      transform: translateY(-2px);
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .badge.aws {
      background-color: #FF9900;
      color: white;
    }

    .badge.docker {
      background-color: #2496ED;
      color: white;
    }

    .badge.github {
      background-color: #181717;
      color: white;
    }

    .badge.terraform {
      background-color: #7B42BC;
      color: white;
    }

    .badge.react {
      background-color: #61DAFB;
      color: #282c34;
    }

    .badge.node {
      background-color: #339933;
      color: white;
    }

    .badge.mongodb {
      background-color: #47A248;
      color: white;
    }

    .badge.mysql {
      background-color: #4479A1;
      color: white;
    }

    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 1.5rem;
      margin-top: 1rem;
    }

    .project-card {
      border: 1px solid var(--gray-200);
      border-radius: var(--border-radius);
      padding: 1.5rem;
      transition: var(--transition);
      height: 100%;
      display: flex;
      flex-direction: column;
    }

    .project-card:hover {
      border-color: var(--primary);
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      transform: translateY(-4px);
    }

    .project-title {
      font-size: 1.1rem;
      font-weight: 600;
      margin-bottom: 0.5rem;
      color: var(--primary-dark);
    }

    .project-description {
      color: var(--gray-700);
      font-size: 0.9rem;
      margin-bottom: 1rem;
      flex-grow: 1;
    }

    .project-tech {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .project-tech .badge {
      font-size: 0.75rem;
      padding: 0.15rem 0.5rem;
    }

    .certs {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 1rem;
      margin-top: 1rem;
    }

    .cert-card {
      border: 1px solid var(--gray-200);
      border-radius: var(--border-radius);
      padding: 1rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      transition: var(--transition);
    }

    .cert-card i {
      font-size: 2rem;
      margin-bottom: 0.5rem;
    }

    .cert-card.completed {
      border-color: var(--success);
    }

    .cert-card.completed i {
      color: var(--success);
    }

    .cert-card.in-progress {
      border-color: var(--warning);
    }

    .cert-card.in-progress i {
      color: var(--warning);
    }

    .cert-card.planned {
      border-color: var(--gray-400);
    }

    .cert-card.planned i {
      color: var(--gray-500);
    }

    .cert-card:hover {
      transform: translateY(-2px);
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .cert-name {
      font-weight: 600;
      margin-bottom: 0.25rem;
    }

    .cert-status {
      font-size: 0.85rem;
      color: var(--gray-600);
    }

    .contact {
      display: flex;
      justify-content: center;
      gap: 1.5rem;
      margin-top: 1rem;
    }

    .contact-item {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      transition: var(--transition);
    }

    .contact-item:hover {
      transform: translateY(-2px);
    }

    .contact-icon {
      width: 50px;
      height: 50px;
      background-color: var(--primary);
      color: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 0.5rem;
      font-size: 1.25rem;
      transition: var(--transition);
    }

    .contact-item:hover .contact-icon {
      transform: scale(1.1);
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .contact-label {
      font-weight: 600;
      margin-bottom: 0.25rem;
    }

    .contact-value {
      font-size: 0.9rem;
      color: var(--primary);
    }

    .contact-value a {
      color: inherit;
      text-decoration: none;
      transition: var(--transition);
    }

    .contact-value a:hover {
      text-decoration: underline;
    }

    .about-grid {
      display: grid;
      grid-template-columns: 3fr 1fr;
      gap: 2rem;
      margin-top: 1rem;
    }

    .about-content {
      line-height: 1.8;
    }

    .about-stats {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    .stat-card {
      background-color: var(--gray-100);
      border-radius: var(--border-radius);
      padding: 1rem;
      text-align: center;
      transition: var(--transition);
    }

    .stat-card:hover {
      background-color: var(--primary);
      color: white;
      transform: translateY(-2px);
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .stat-card:hover .stat-value,
    .stat-card:hover .stat-label {
      color: white;
    }

    .stat-value {
      font-size: 1.5rem;
      font-weight: 700;
      color: var(--primary);
      margin-bottom: 0.25rem;
      transition: var(--transition);
    }

    .stat-label {
      font-size: 0.85rem;
      font-weight: 500;
      color: var(--gray-600);
      transition: var(--transition);
    }

    .footer {
      text-align: center;
      padding: 2rem 0;
      color: var(--gray-600);
      font-size: 0.9rem;
    }

    .footer a {
      color: var(--primary);
      text-decoration: none;
    }

    .footer a:hover {
      text-decoration: underline;
    }

    .highlight {
      color: var(--primary);
      font-weight: 600;
    }

    .divider {
      height: 1px;
      background-color: var(--gray-200);
      margin: 2rem 0;
    }

    .personal-qualities {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 1rem;
      margin-top: 1rem;
    }

    .quality-card {
      background-color: var(--gray-100);
      border-radius: var(--border-radius);
      padding: 1.5rem;
      text-align: center;
      transition: var(--transition);
    }

    .quality-card:hover {
      background-color: var(--primary);
      color: white;
      transform: translateY(-2px);
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .quality-card i {
      font-size: 2rem;
      color: var(--primary);
      margin-bottom: 1rem;
      transition: var(--transition);
    }

    .quality-card:hover i {
      color: white;
    }

    .quality-title {
      font-weight: 600;
      margin-bottom: 0.5rem;
    }

    .quality-description {
      font-size: 0.9rem;
      color: var(--gray-600);
      transition: var(--transition);
    }

    .quality-card:hover .quality-description {
      color: white;
    }

    @media (max-width: 768px) {
      .container {
        padding: 1rem;
      }

      header {
        padding: 2rem 1rem;
      }

      .section {
        padding: 1.5rem;
      }

      .about-grid {
        grid-template-columns: 1fr;
      }

      .contact {
        flex-direction: column;
        gap: 2rem;
      }

      .projects, .certs {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="profile-pic">
        <i class="fas fa-user"></i>
      </div>
      <h1>Aimable Mugwaneza</h1>
      <h2>Cloud & DevOps Engineer</h2>
      <h3>B.S. in Computer Science (Graduating May 2025)</h3>
    </header>

    <section class="section" id="about">
      <div class="section-title">
        <i class="fas fa-user-circle"></i>
        <h2>About Me</h2>
      </div>
      <div class="about-grid">
        <div class="about-content">
          <p>I'm a soon-to-be Computer Science graduate deeply passionate about <span class="highlight">Cloud, DevOps, and Infrastructure Engineering</span>. Originally set on the path of software development, I pivoted into cloud and systems design after realizing I enjoyed orchestrating and deploying scalable, secure, and production-ready infrastructure more than writing isolated code features.</p>
          <br>
          <p>What started as curiosity turned into hands-on projects — containerizing apps with Docker, automating deployment with CI/CD pipelines, provisioning infrastructure with Terraform, and securing cloud architectures with IAM, Security Groups, and best practices.</p>
          <br>
          <p>I'm driven by problem-solving, self-learning, and architecting systems that scale — and I document every step of my growth through deep technical write-ups, diagrams, and infrastructure breakdowns.</p>
        </div>
        <div class="about-stats">
          <div class="stat-card">
            <div class="stat-value">2025</div>
            <div class="stat-label">Graduation Year</div>
          </div>
          <div class="stat-card">
            <div class="stat-value">4+</div>
            <div class="stat-label">AWS Services Used</div>
          </div>
          <div class="stat-card">
            <div class="stat-value">3+</div>
            <div class="stat-label">Major Projects</div>
          </div>
          <div class="stat-card">
            <div class="stat-value">1+</div>
            <div class="stat-label">AWS Certification</div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="tech-stack">
      <div class="section-title">
        <i class="fas fa-layer-group"></i>
        <h2>Tech Stack & Tools</h2>
      </div>
      <div class="tech-stack">
        <div class="category">
          <h3>Cloud & Infrastructure:</h3>
          <div class="badge-container">
            <div class="badge aws"><i class="fab fa-aws"></i> AWS</div>
            <div class="badge terraform"><i class="fas fa-cubes"></i> Terraform</div>
            <div class="badge docker"><i class="fab fa-docker"></i> Docker</div>
            <div class="badge"><i class="fas fa-server"></i> Nginx</div>
            <div class="badge"><i class="fab fa-linux"></i> Linux</div>
            <div class="badge"><i class="fas fa-chart-line"></i> Prometheus</div>
            <div class="badge"><i class="fas fa-tachometer-alt"></i> Grafana</div>
          </div>
        </div>
        
        <div class="category">
          <h3>CI/CD Pipelines:</h3>
          <div class="badge-container">
            <div class="badge github"><i class="fab fa-github"></i> GitHub Actions</div>
            <div class="badge github"><i class="fab fa-git-alt"></i> Git & GitHub</div>
          </div>
        </div>
        
        <div class="category">
          <h3>Frontend:</h3>
          <div class="badge-container">
            <div class="badge react"><i class="fab fa-react"></i> React</div>
            <div class="badge"><i class="fab fa-html5"></i> HTML/CSS</div>
            <div class="badge"><i class="fab fa-css3"></i> Tailwind CSS</div>
          </div>
        </div>
        
        <div class="category">
          <h3>Backend & APIs:</h3>
          <div class="badge-container">
            <div class="badge node"><i class="fab fa-node-js"></i> Node.js (Express)</div>
            <div class="badge mongodb"><i class="fas fa-database"></i> MongoDB</div>
            <div class="badge mysql"><i class="fas fa-database"></i> MySQL</div>
          </div>
        </div>
        
        <div class="category">
          <h3>Auth & Secrets:</h3>
          <div class="badge-container">
            <div class="badge"><i class="fas fa-lock"></i> Clerk</div>
            <div class="badge"><i class="fas fa-key"></i> .env management</div>
          </div>
        </div>
        
        <div class="category">
          <h3>Programming Languages:</h3>
          <div class="badge-container">
            <div class="badge"><i class="fab fa-js"></i> JavaScript (Advanced)</div>
            <div class="badge"><i class="fab fa-python"></i> Python (Intermediate)</div>
            <div class="badge"><i class="fab fa-java"></i> Java (Intermediate)</div>
            <div class="badge"><i class="fab fa-html5"></i> HTML/CSS (Advanced)</div>
            <div class="badge"><i class="fas fa-database"></i> SQL (Intermediate)</div>
            <div class="badge"><i class="fas fa-terminal"></i> Bash/Shell (Beginner-Intermediate)</div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="current-focus">
      <div class="section-title">
        <i class="fas fa-bullseye"></i>
        <h2>Current Focus Areas</h2>
      </div>
      <ul class="focus-list">
        <li>Cloud Engineering (AWS core services, IAM, network security)</li>
        <li>DevOps practices (CI/CD pipelines, logging, automation)</li>
        <li>Infrastructure as Code (Terraform)</li>
        <li>Docker containerization and system orchestration</li>
        <li>Secure multi-tier deployments (Frontend ↔ Backend ↔ Database)</li>
        <li>Home lab setups and self-hosting</li>
        <li>Writing and publishing technical documentation & cloud blogs</li>
      </ul>
    </section>

    <section class="section" id="certifications">
      <div class="section-title">
        <i class="fas fa-certificate"></i>
        <h2>Certifications</h2>
      </div>
      <div class="certs">
        <div class="cert-card completed">
          <i class="fab fa-aws"></i>
          <div class="cert-name">AWS Certified Cloud Practitioner</div>
          <div class="cert-status">✅ Completed (2025)</div>
        </div>
        
        <div class="cert-card in-progress">
          <i class="fas fa-shield-alt"></i>
          <div class="cert-name">CompTIA Security+</div>
          <div class="cert-status">🛡️ In Progress</div>
        </div>
        
        <div class="cert-card planned">
          <i class="fas fa-cubes"></i>
          <div class="cert-name">Terraform Associate</div>
          <div class="cert-status">🛠️ Planned</div>
        </div>
        
        <div class="cert-card planned">
          <i class="fab fa-aws"></i>
          <div class="cert-name">AWS Solutions Architect – Associate</div>
          <div class="cert-status">📦 Planned</div>
        </div>
      </div>
    </section>

    <section class="section" id="projects">
      <div class="section-title">
        <i class="fas fa-code-branch"></i>
        <h2>Projects</h2>
      </div>
      <div class="projects">
        <div class="project-card">
          <div class="project-title">FlowLedger</div>
          <div class="project-description">
            Open-source ERP/CRM fullstack system using MERN stack, Dockerized, CI/CD pipeline, database per service
          </div>
          <div class="project-tech">
            <div class="badge mongodb"><i class="fas fa-database"></i> MongoDB</div>
            <div class="badge react"><i class="fab fa-react"></i> React</div>
            <div class="badge node"><i class="fab fa-node-js"></i> Node.js</div>
            <div class="badge docker"><i class="fab fa-docker"></i> Docker</div>
            <div class="badge github"><i class="fab fa-github"></i> CI/CD</div>
          </div>
        </div>
        
        <div class="project-card">
          <div class="project-title">Cloud Portfolio Site</div>
          <div class="project-description">
            Deployed on Amplify and EC2 with GitHub Actions, Docker, ECR, custom domain via Route 53
          </div>
          <div class="project-tech">
            <div class="badge aws"><i class="fab fa-aws"></i> AWS</div>
            <div class="badge docker"><i class="fab fa-docker"></i> Docker</div>
            <div class="badge github"><i class="fab fa-github"></i> GitHub Actions</div>
            <div class="badge react"><i class="fab fa-react"></i> React</div>
          </div>
        </div>
        
        <div class="project-card">
          <div class="project-title">Spring Boot Microservices Banking App</div>
          <div class="project-description">
            Learning and deploying microservices with service registry, API Gateway, Docker, and MySQL
          </div>
          <div class="project-tech">
            <div class="badge"><i class="fab fa-java"></i> Spring Boot</div>
            <div class="badge docker"><i class="fab fa-docker"></i> Docker</div>
            <div class="badge mysql"><i class="fas fa-database"></i> MySQL</div>
            <div class="badge"><i class="fas fa-network-wired"></i> Microservices</div>
          </div>
        </div>
        
        <div class="project-card">
          <div class="project-title">Monitoring Stack Integration</div>
          <div class="project-description">
            Prometheus + Grafana for container metrics, exploring local vs production monitoring
          </div>
          <div class="project-tech">
            <div class="badge"><i class="fas fa-chart-line"></i> Prometheus</div>
            <div class="badge"><i class="fas fa-tachometer-alt"></i> Grafana</div>
            <div class="badge docker"><i class="fab fa-docker"></i> Docker</div>
            <div class="badge"><i class="fas fa-server"></i> Infrastructure</div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="learning-style">
      <div class="section-title">
        <i class="fas fa-brain"></i>
        <h2>Learning Style</h2>
      </div>
      <ul>
        <li><strong>Hands-on.</strong> I learn best by building, breaking, debugging, and documenting the process.</li>
        <li>I often deploy real apps just to understand how systems communicate, scale, and stay secure.</li>
        <li>Each project is not just a build — it's a mini-case study I convert into blogs, diagrams, or README breakdowns.</li>
      </ul>
    </section>

    <section class="section" id="personal-strengths">
      <div class="section-title">
        <i class="fas fa-star"></i>
        <h2>Personal Strengths</h2>
      </div>
      <div class="personal-qualities">
        <div class="quality-card">
          <i class="fas fa-search"></i>
          <div class="quality-title">Detail-Oriented</div>
          <div class="quality-description">Obsessively thorough when it comes to system design and architecture</div>
        </div>
        
        <div class="quality-card">
          <i class="fas fa-rocket"></i>
          <div class="quality-title">Quick Learner</div>
          <div class="quality-description">Push beyond tutorials to customize and optimize real solutions</div>
        </div>
        
        <div class="quality-card">
          <i class="fas fa-comments"></i>
          <div class="quality-title">Strong Communicator</div>
          <div class="quality-description">Translate technical concepts into clear, accessible explanations</div>
        </div>
        
        <div class="quality-card">
          <i class="fas fa-lightbulb"></i>
          <div class="quality-title">Systems Thinker</div>
          <div class="quality-description">Thrive when connecting components to deliver real-world functionality</div>
        </div>
      </div>
    </section>

    <section class="section" id="contact">
      <div class="section-title">
        <i class="fas fa-envelope"></i>
        <h2>Contact & Links</h2>
      </div>
      <div class="contact">
        <div class="contact-item">
          <div class="contact-icon">
            <i class="fas fa-globe"></i>
          </div>
          <div class="contact-label">Website</div>
          <div class="contact-value">
            <a href="https://aimablem.dev" target="_blank">aimablem.dev</a>
          </div>
        </div>
        
        <div class="contact-item">
          <div class="contact-icon">
            <i class="fab fa-github"></i>
          </div>
          <div class="contact-label">GitHub</div>
          <div class="contact-value">
            <a href="https://github.com/AimableMugwaneza" target="_blank">AimableMugwaneza</a>
          </div>
        </div>
        
        <div class="contact-item">
          <div class="contact-icon">
            <i class="fab fa-linkedin"></i>
          </div>
          <div class="contact-label">LinkedIn</div>
          <div class="contact-value">
            <a href="https://linkedin.com/in/aimablemugwaneza" target="_blank">aimablemugwaneza</a>
          </div>
        </div>
      </div>
    </section>

    <div class="footer">
      <p>© 2025 Aimable Mugwaneza | Made with <i class="fas fa-heart" style="color: #f56565;"></i> and modern web technologies</p>
    </div>
  </div>
</body>
</html>