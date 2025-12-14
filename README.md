<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Notes Hub - Easy Study</title>
  <style>
    :root {
      --primary: #4da3ff;
      --secondary: #1e1e1e;
      --light: #f4f9ff;
      --text-dark: #222;
      --text-light: #fff;
      --accent: #ffbf47;
      --radius: 12px;
    }* { box-sizing: border-box; margin: 0; padding: 0; }
body {
  font-family: Arial, sans-serif;
  background: var(--light);
  color: var(--text-dark);
  line-height: 1.5;
}

/* Header */
header {
  background: var(--secondary);
  color: var(--text-light);
  padding: 20px 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
header .logo { font-weight: bold; font-size: 22px; }
header nav a {
  color: var(--text-light);
  text-decoration: none;
  margin-left: 20px;
  font-size: 16px;
}

/* Hero Section */
.hero {
  display: flex;
  justify-content: space-between;
  padding: 60px 40px;
  background: linear-gradient(135deg, #e8f3ff, #d0e7ff);
  align-items: center;
  border-radius: var(--radius);
  margin: 20px;
}
.hero-text { max-width: 55%; }
.hero-text h1 { font-size: 38px; margin-bottom: 15px; }
.hero-text p { font-size: 18px; margin-bottom: 20px; color: #555; }
.hero-text button {
  padding: 12px 24px;
  background: var(--primary);
  color: white;
  border: none;
  border-radius: var(--radius);
  font-size: 16px;
  cursor: pointer;
}
.hero-img { width: 40%; height: 250px; background: var(--primary); border-radius: var(--radius); }

/* Features Section */
.features {
  padding: 60px 40px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 30px;
}
.feature-box {
  background: white;
  padding: 20px;
  border-radius: var(--radius);
  box-shadow: 0 4px 10px rgba(0,0,0,0.05);
  text-align: center;
}
.feature-box h3 { margin-bottom: 10px; }
.feature-box p { color: #555; }

/* Stats Section */
.stats {
  display: flex;
  justify-content: space-around;
  padding: 40px;
  background: #e0f0ff;
  border-radius: var(--radius);
  margin: 20px;
}
.stat-box { text-align: center; }
.stat-box h2 { font-size: 32px; color: var(--primary); margin-bottom: 8px; }
.stat-box p { color: #555; }

/* Search Notes Section */
.search-section {
  padding: 40px;
  text-align: center;
}
.search-section input {
  padding: 10px 14px;
  width: 60%;
  border-radius: var(--radius);
  border: 1px solid #ccc;
  margin-right: 8px;
  font-size: 16px;
}
.search-section button {
  padding: 10px 18px;
  border: none;
  border-radius: var(--radius);
  background: var(--primary);
  color: white;
  font-size: 16px;
  cursor: pointer;
}

/* Pricing Section */
.pricing {
  display: flex;
  justify-content: space-around;
  padding: 40px;
  gap: 20px;
  flex-wrap: wrap;
}
.pricing-box {
  background: white;
  padding: 20px;
  border-radius: var(--radius);
  box-shadow: 0 4px 10px rgba(0,0,0,0.05);
  flex: 1 1 250px;
  text-align: center;
}
.pricing-box h3 { margin-bottom: 10px; }
.pricing-box p { color: #555; margin-bottom: 12px; }
.pricing-box button { padding: 10px 18px; background: var(--accent); border: none; border-radius: var(--radius); color: white; cursor: pointer; }

/* Call-to-Action Section */
.cta-section {
  text-align: center;
  padding: 40px;
  background: #d0e7ff;
  border-radius: var(--radius);
  margin: 20px;
}
.cta-section button {
  padding: 12px 24px;
  background: var(--primary);
  border: none;
  border-radius: var(--radius);
  color: white;
  font-size: 18px;
  cursor: pointer;
}

/* Footer */
footer {
  background: var(--secondary);
  color: var(--text-light);
  padding: 20px 40px;
  text-align: center;
  margin-top: 40px;
}

/* Responsive */
@media(max-width: 900px){
  .hero { flex-direction: column; text-align: center; }
  .hero-img { width: 80%; margin-top: 20px; }
  .features { grid-template-columns: repeat(2, 1fr); }
  .stats { flex-direction: column; gap: 20px; }
  .pricing { flex-direction: column; align-items: center; }
}
@media(max-width: 600px){
  .features { grid-template-columns: 1fr; }
  header { flex-direction: column; align-items: flex-start; }
  header nav { margin-top: 10px; }
  .search-section input { width: 100%; margin-bottom: 10px; }
}

  </style>
</head>
<body>  <header>
    <div class="logo">Notes Hub</div>
    <nav>
      <a href="#features">Features</a>
      <a href="#stats">Stats</a>
      <a href="#pricing">Pricing</a>
      <a href="#contact">Contact</a>
      <a href="#" style="background: var(--primary); padding: 6px 14px; border-radius: var(--radius); color: white;">Get Notes</a>
    </nav>
  </header>  <section class="hero">
    <div class="hero-text">
      <h1>Easy Notes for Easy Learning</h1>
      <p>Download structured notes for your subjects and improve your study efficiency. Simple, clean, and organized.</p>
      <button>Get Started</button>
    </div>
    <div class="hero-img"></div>
  </section>  <section class="features" id="features">
    <div class="feature-box">
      <h3>Organized Notes</h3>
      <p>All notes are properly categorized by subjects and topics for quick access.</p>
    </div>
    <div class="feature-box">
      <h3>Easy to Download</h3>
      <p>Download PDF notes instantly and start learning without delays.</p>
    </div>
    <div class="feature-box">
      <h3>Free Resources</h3>
      <p>Access high-quality study materials completely free for all students.</p>
    </div>
  </section>  <!-- Stats Section -->  <section class="stats" id="stats">
    <div class="stat-box">
      <h2>500+</h2>
      <p>Notes Available</p>
    </div>
    <div class="stat-box">
      <h2>200+</h2>
      <p>Subjects Covered</p>
    </div>
    <div class="stat-box">
      <h2>1000+</h2>
      <p>Students Helped</p>
    </div>
  </section>  <!-- Search Notes Section -->  <section class="search-section">
    <input type="text" placeholder="Search notes by subject...">
    <button>Search</button>
  </section>  <!-- Pricing Section -->  <section class="pricing" id="pricing">
    <div class="pricing-box">
      <h3>Free Plan</h3>
      <p>Access basic notes for all subjects.</p>
      <button>Get Free Notes</button>
    </div>
    <div class="pricing-box">
      <h3>Pro Plan</h3>
      <p>Access all notes, premium content, and updates.</p>
      <button>Get Pro</button>
    </div>
  </section>  <!-- Call to Action Section -->  <section class="cta-section">
    <h2>Start Learning Today!</h2>
    <button>Download Notes Now</button>
  </section>  <footer id="contact">
    © 2025 Notes Hub — Contact: hello@noteshub.example
  </footer></body>
</html>
