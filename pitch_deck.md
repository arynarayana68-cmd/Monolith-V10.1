<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Monolith V10.1 - LinkedIn Carousel</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500&family=Montserrat:wght@700;900&display=swap" rel="stylesheet">
<style>
  body {
    background-color: #1a1a1a; /* Dark background to view slides against */
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 50px;
    padding: 50px;
    margin: 0;
  }
  
  /* 1080x1080 is the standard LinkedIn Carousel square size */
  .slide {
    width: 1080px;
    height: 1080px;
    background-color: #36454F; /* Charcoal Gray */
    color: #FFFFFF; /* Stark White */
    font-family: 'Inter', sans-serif;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 120px;
    box-sizing: border-box;
    position: relative;
    box-shadow: 0 20px 50px rgba(0,0,0,0.5);
    overflow: hidden;
  }

  /* Electric Blue Grid/Glow accent */
  .slide::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: radial-gradient(circle at top left, rgba(0, 240, 255, 0.15), transparent 60%);
    pointer-events: none;
  }

  .accent-bar {
    width: 120px;
    height: 12px;
    background-color: #00F0FF; /* Electric Blue */
    margin-bottom: 50px;
  }

  h1, h2 {
    font-family: 'Montserrat', sans-serif;
    text-transform: uppercase;
    font-weight: 900;
    margin: 0 0 40px 0;
    line-height: 1.1;
  }

  h1 { font-size: 85px; }
  h2 { font-size: 70px; }

  p {
    font-size: 40px;
    line-height: 1.5;
    margin: 0;
    font-weight: 400;
  }

  .electric-blue { color: #00F0FF; }
  
  .slide-number {
    position: absolute;
    bottom: 50px;
    right: 50px;
    font-family: 'Montserrat', sans-serif;
    font-size: 35px;
    font-weight: 700;
    color: rgba(255,255,255,0.4);
  }

  .center {
    align-items: center;
    text-align: center;
  }
  
  .center .accent-bar {
    margin: 0 auto 50px auto;
  }

  /* Footer for final slide */
  .footer-cta {
    margin-top: 80px;
    font-size: 32px;
    color: #00F0FF;
    font-weight: 500;
    border-top: 2px solid rgba(0, 240, 255, 0.3);
    padding-top: 40px;
  }
</style>
</head>
<body>

  <!-- Slide 1 -->
  <div class="slide">
    <div class="accent-bar"></div>
    <h1>THE ERA OF STATIC SEARCH <br><span class="electric-blue">IS OVER.</span></h1>
    <p>Is your B2B infrastructure ready for autonomous AI agents?</p>
    <div class="slide-number">01 / 07 &rarr;</div>
  </div>

  <!-- Slide 2 -->
  <div class="slide">
    <div class="accent-bar"></div>
    <h2>LEGACY WEBSITES ARE INVISIBLE.</h2>
    <p>DOM bloat, third-party trackers, and manual contact forms are being entirely bypassed by modern AI procurement pipelines. Search engines aren't fetching your site—agents are.</p>
    <div class="slide-number">02 / 07 &rarr;</div>
  </div>

  <!-- Slide 3 -->
  <div class="slide center">
    <div class="accent-bar"></div>
    <h1>ENTER <br><span class="electric-blue">MONOLITH V10.1</span></h1>
    <p>A sovereign, high-density edge infrastructure engineered specifically for Generative Engine Optimization (GEO).</p>
    <div class="slide-number">03 / 07 &rarr;</div>
  </div>

  <!-- Slide 4 -->
  <div class="slide">
    <div class="accent-bar"></div>
    <h2>MASTER BACKEND</h2>
    <p>Token-optimized microservices exposing machine-callable OpenAPI and MCP endpoints. Delivers sub-millisecond JSON-LD semantic schema injection directly to AI agents.</p>
    <div class="slide-number">04 / 07 &rarr;</div>
  </div>

  <!-- Slide 5 -->
  <div class="slide">
    <div class="accent-bar"></div>
    <h2>TRUE FACE BPS</h2>
    <p>Client-side biometric verification executing native vector cosine distance matching at the local database layer. Zero network latency. Zero centralized credential vulnerability.</p>
    <div class="slide-number">05 / 07 &rarr;</div>
  </div>

  <!-- Slide 6 -->
  <div class="slide">
    <div class="accent-bar"></div>
    <h2>MONOLITH MOBILE SUITE</h2>
    <p>Built for mobile-first workflows. Manage multi-port ingress daemons, monitor real-time telemetry, and run your sovereign operations directly from sandboxed hardware.</p>
    <div class="slide-number">06 / 07 &rarr;</div>
  </div>

  <!-- Slide 7 -->
  <div class="slide center">
    <div class="accent-bar"></div>
    <h1>ALIGN WITH<br><span class="electric-blue">AGENTIC INDEXING.</span></h1>
    <p>Upgrade your infrastructure before your data gets left behind.</p>
    <div class="footer-cta">Read the technical brief at the link in the comments.</div>
    <div class="slide-number">07 / 07</div>
  </div>

</body>
</html>
