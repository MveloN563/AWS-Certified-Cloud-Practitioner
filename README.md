<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AWS re/Start Journey – Chiara</title>
  <!-- Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Roboto, system-ui, -apple-system, sans-serif;
      background: #f5f7fb;
      color: #1e2a3a;
      line-height: 1.7;
      padding: 2rem 1.5rem;
    }

    .container {
      max-width: 1100px;
      margin: 0 auto;
      background: white;
      border-radius: 28px;
      box-shadow: 0 20px 60px rgba(0, 0, 0, 0.08);
      padding: 2.5rem 3rem;
    }

    /* header */
    .header {
      text-align: center;
      padding-bottom: 2rem;
      border-bottom: 3px solid #f0f3f8;
      margin-bottom: 2.5rem;
    }

    .header h1 {
      font-size: 2.8rem;
      font-weight: 700;
      letter-spacing: -0.5px;
      background: linear-gradient(145deg, #1e2a3a, #2c3e66);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      margin-bottom: 0.5rem;
    }

    .header p {
      font-size: 1.2rem;
      color: #3d4e6b;
      margin-top: 0.25rem;
    }

    .badge-strip {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin: 1.5rem 0 1rem;
    }

    .badge-strip span {
      background: #eef2f7;
      padding: 0.4rem 1.2rem;
      border-radius: 40px;
      font-size: 0.9rem;
      font-weight: 600;
      color: #1e2a3a;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
    }

    .badge-strip i {
      color: #f90;
      font-size: 1.2rem;
    }

    /* intro */
    .intro {
      background: #f8faff;
      border-radius: 20px;
      padding: 1.8rem 2.2rem;
      margin-bottom: 2.8rem;
      border-left: 6px solid #ff9900;
    }

    .intro h2 {
      font-size: 1.6rem;
      font-weight: 600;
      margin-bottom: 0.75rem;
      color: #0b1a33;
    }

    .intro p {
      font-size: 1.05rem;
      color: #1f334a;
    }

    .cert-badges {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2.5rem;
      margin: 2.5rem 0 3rem;
      padding: 1.8rem 0;
      background: #fafcff;
      border-radius: 30px;
    }

    .cert-badges a {
      display: inline-block;
      transition: transform 0.2s ease;
    }

    .cert-badges a:hover {
      transform: scale(1.07);
    }

    .cert-badges img {
      width: 140px;
      height: auto;
      border-radius: 16px;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
    }

    /* sections */
    .section-title {
      font-size: 2rem;
      font-weight: 700;
      margin: 2.8rem 0 1.2rem;
      padding-bottom: 0.4rem;
      border-bottom: 4px solid #ff9900;
      display: inline-block;
    }

    .grid-2col {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 1.8rem;
      margin: 1.5rem 0 2rem;
    }

    .card {
      background: #fafcff;
      border-radius: 18px;
      padding: 1.5rem 1.8rem;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.02);
      border: 1px solid #e9edf4;
      transition: all 0.2s ease;
    }

    .card:hover {
      border-color: #ff9900;
      box-shadow: 0 8px 24px rgba(255, 153, 0, 0.08);
    }

    .card h3 {
      font-size: 1.3rem;
      font-weight: 600;
      color: #0b1a33;
      display: flex;
      align-items: center;
      gap: 0.5rem;
      margin-bottom: 0.5rem;
    }

    .card h3 i {
      color: #ff9900;
      font-size: 1.2rem;
      width: 1.8rem;
    }

    .card ul {
      list-style: none;
      padding-left: 0.2rem;
      margin-top: 0.6rem;
    }

    .card li {
      padding: 0.25rem 0;
      padding-left: 1.6rem;
      position: relative;
    }

    .card li::before {
      content: "▹";
      position: absolute;
      left: 0;
      color: #ff9900;
      font-weight: bold;
    }

    .skill-tag {
      display: inline-block;
      background: #eef2f7;
      padding: 0.25rem 1rem;
      border-radius: 30px;
      font-size: 0.85rem;
      font-weight: 500;
      margin: 0.2rem 0.2rem;
      color: #1e2a3a;
      border: 1px solid #dce3ed;
    }

    .key-skills .skill-tag {
      background: #e5edf9;
      border-color: #b8cbe0;
    }

    .footer {
      margin-top: 3.5rem;
      padding-top: 2rem;
      border-top: 2px solid #eef2f7;
      text-align: center;
      color: #4a5c78;
      font-size: 0.95rem;
    }

    /* responsive */
    @media (max-width: 700px) {
      .container {
        padding: 1.5rem 1.2rem;
      }
      .header h1 {
        font-size: 2rem;
      }
      .cert-badges img {
        width: 110px;
      }
    }

    /* small tweaks */
    .mt-1 { margin-top: 0.6rem; }
    .mb-1 { margin-bottom: 0.6rem; }
    .text-muted { color: #4d637f; }
  </style>
</head>
<body>

<div class="container">

  <!-- Header -->
  <div class="header">
    <h1>🌩️ AWS re/Start Portfolio</h1>
    <p>Chiara Tardioli · Cloud &amp; IT Learning Journey</p>
    <div class="badge-strip">
      <span><i class="fab fa-aws"></i> AWS Cloud</span>
      <span><i class="fab fa-linux"></i> Linux Admin</span>
      <span><i class="fab fa-python"></i> Python Automation</span>
      <span><i class="fas fa-cloud"></i> Hands-on Labs</span>
    </div>
  </div>

  <!-- Intro -->
  <div class="intro">
    <h2>☁️ About This Journey</h2>
    <p>Hi, I'm Chiara. This repository documents my learning through the <strong>AWS re/Start program</strong> — a full-time, hands-on training initiative covering cloud fundamentals, IT operations, networking, security, and automation using Amazon Web Services. I built practical skills through labs, structured modules, and projects that simulate real-world cloud environments.</p>
  </div>

  <!-- Certifications & Badges -->
  <div class="cert-badges">
    <a href="https://www.credly.com/badges/fee7e849-146d-41c3-8c61-e13a63e83073/public_url" target="_blank">
      <img src="https://via.placeholder.com/150x150/FF9900/FFFFFF?text=AWS+re/Start" alt="AWS re/Start Graduate Badge" />
    </a>
    <a href="https://www.credly.com/badges/d9e2d128-be81-48a5-a192-4030273b65cc/public_url" target="_blank">
      <img src="https://via.placeholder.com/150x150/232F3E/FFFFFF?text=AWS+Certified" alt="AWS Certified Cloud Practitioner" />
    </a>
  </div>

  <!-- Core Concepts -->
  <h2 class="section-title">📘 Core Concepts</h2>
  <div class="grid-2col">
    <div class="card"><h3><i class="fas fa-microchip"></i> EC2 & Compute</h3><p>Virtual machines, instance types, and compute workloads on AWS.</p></div>
    <div class="card"><h3><i class="fab fa-linux"></i> Linux</h3><p>Command line, file systems, user management, and system operations.</p></div>
    <div class="card"><h3><i class="fas fa-network-wired"></i> Networking</h3><p>Subnets, routing, DNS, VPC, and hybrid connectivity.</p></div>
    <div class="card"><h3><i class="fas fa-robot"></i> ML & GenAI</h3><p>Introductory concepts and applications of machine learning and generative AI.</p></div>
    <div class="card"><h3><i class="fas fa-wordpress"></i> WordPress</h3><p>Web hosting fundamentals and deployment on AWS.</p></div>
  </div>

  <!-- Labs (grouped) -->
  <h2 class="section-title">🧪 Hands-on Labs</h2>
  <div class="grid-2col">
    <div class="card"><h3><i class="fas fa-expand-arrows-alt"></i> Cloud Architecture & Scaling</h3><ul><li>Auto Scaling & ELB</li><li>CloudFormation (IaC)</li><li>Route 53 failover</li><li>System optimization</li></ul></div>
    <div class="card"><h3><i class="fas fa-server"></i> Compute Infrastructure</h3><ul><li>EC2 deployment</li><li>Static website hosting (S3)</li><li>Architecture analysis</li></ul></div>
    <div class="card"><h3><i class="fas fa-database"></i> Databases & Data</h3><ul><li>RDS migration</li><li>SQL / Aurora / DynamoDB</li><li>Advanced DB manipulation</li></ul></div>
    <div class="card"><h3><i class="fas fa-code"></i> DevOps & Automation</h3><ul><li>Python & AWS CLI scripting</li><li>System Manager</li><li>Debugging & automation workflows</li></ul></div>
    <div class="card"><h3><i class="fas fa-terminal"></i> Linux & Systems</h3><ul><li>Bash scripting</li><li>Cron jobs & log analysis</li><li>Package management, backups</li></ul></div>
    <div class="card"><h3><i class="fas fa-brain"></i> ML & Generative AI</h3><ul><li>Basic ML model training</li><li>AI portfolio project</li><li>Intro to GenAI concepts</li></ul></div>
    <div class="card"><h3><i class="fas fa-chart-line"></i> Monitoring</h3><ul><li>CloudWatch metrics</li><li>CloudTrail logging</li></ul></div>
    <div class="card"><h3><i class="fas fa-cloud"></i> Networking</h3><ul><li>VPC, subnets, routing</li><li>IP addressing & troubleshooting</li><li>Web server connectivity</li></ul></div>
    <div class="card"><h3><i class="fas fa-shield-alt"></i> Security</h3><ul><li>IAM policies & access control</li><li>Encryption & system hardening</li><li>Malware protection</li></ul></div>
    <div class="card"><h3><i class="fas fa-cubes"></i> Serverless & Containers</h3><ul><li>Lambda functions</li><li>Event-driven architecture</li><li>Serverless challenges</li></ul></div>
    <div class="card"><h3><i class="fas fa-archive"></i> Storage & Archiving</h3><ul><li>S3 bucket management</li><li>EBS configuration</li><li>Storage optimization</li></ul></div>
  </div>

  <!-- Projects -->
  <h2 class="section-title">🚀 Projects</h2>
  <div class="grid-2col">
    <div class="card"><h3><i class="fas fa-cart-plus"></i> 3D E‑commerce</h3><p>Cloud-based simulation of a modern e‑commerce deployment environment.</p></div>
    <div class="card"><h3><i class="fas fa-globe"></i> S3 Static Website</h3><p>Fully deployed static website hosted on AWS S3 — real‑world cloud hosting.</p></div>
  </div>

  <!-- Key Skills -->
  <h2 class="section-title">⚡ Key Skills Developed</h2>
  <div class="card key-skills" style="background: #f8faff; border: 1px solid #dce3ed;">
    <div style="display: flex; flex-wrap: wrap; gap: 0.4rem 0.6rem;">
      <span class="skill-tag">Cloud infrastructure management</span>
      <span class="skill-tag">AWS service integration</span>
      <span class="skill-tag">Linux system administration</span>
      <span class="skill-tag">Networking design & troubleshooting</span>
      <span class="skill-tag">Database design & querying</span>
      <span class="skill-tag">Python scripting & automation</span>
      <span class="skill-tag">Security best practices</span>
      <span class="skill-tag">Technical documentation (GitHub)</span>
    </div>
  </div>

  <!-- Summary -->
  <div style="margin-top: 3rem; background: #f0f5ff; border-radius: 24px; padding: 1.8rem 2rem; border: 1px solid #dce3ed;">
    <h3 style="display: flex; align-items: center; gap: 0.6rem; font-size: 1.5rem;"><i class="fas fa-graduation-cap" style="color: #ff9900;"></i> Summary</h3>
    <p style="font-size: 1.05rem;">This repository represents a complete learning journey through cloud computing fundamentals and practical AWS workloads. It documents consistent hands‑on experience across infrastructure, security, automation, and application deployment.</p>
  </div>

  <!-- Footer -->
  <div class="footer">
    <p><i class="fas fa-code"></i> Built from the AWS re/Start README &nbsp;·&nbsp; <i class="fab fa-github"></i> <a href="#" style="color: #1e2a3a; text-decoration: none; font-weight: 500;">Chiara Tardioli</a></p>
    <p style="margin-top: 0.4rem; font-size: 0.85rem; opacity: 0.7;">Portfolio page generated from learning journey documentation</p>
  </div>

</div>
</body>
</html>
