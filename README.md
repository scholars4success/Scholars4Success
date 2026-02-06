<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Scholars 4 Success</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg-dark: #0b0f0d;
      --green-main: #1db954; /* high-quality nonprofit green */
      --green-soft: #7cffb2;
      --text-light: #e6f2ec;
      --card-dark: #121816;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      padding-top: 80px;
      background-color: var(--bg-dark);
      color: var(--text-light);
      line-height: 1.6;
    }

    /* NAVBAR */
    header {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 14px 32px;
      background: rgba(11, 15, 13, 0.95);
      backdrop-filter: blur(6px);
      z-index: 1000;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .logo-icon {
      width: 40px;
      height: 40px;
      border-radius: 10px;
      background: linear-gradient(135deg, #1db954, #2ee59d);
      display: flex;
      align-items: center;
      justify-content: center;
      color: #0b0f0d;
      font-weight: 800;
      font-size: 16px;
      box-shadow: 0 6px 16px rgba(29, 185, 84, 0.35);
      flex-shrink: 0;
    }

    .logo-text {
      font-size: 18px;
      font-weight: 600;
      letter-spacing: 0.4px;
      white-space: nowrap;
      line-height: 1;
    }

    nav a {
      margin-left: 20px;
      text-decoration: none;
      color: var(--text-light);
      font-weight: 400;
      font-size: 14.5px;
      line-height: 1;
      display: inline-flex;
      align-items: center;
      transition: color 0.3s;
    }

    .donate-btn {
      padding: 8px 18px;
      border-radius: 20px;
      background: var(--green-main);
      color: #0b0f0d !important;
      font-weight: 600;
      font-size: 14px;
      display: inline-flex;
      align-items: center;
    }

    .donate-btn:hover {
      box-shadow: 0 8px 20px rgba(29, 185, 84, 0.4);
    }

    nav a:hover {
      color: var(--green-main);
    }

    /* HERO SECTION */
    .hero {
      height: 100vh;
      background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
        url('https://images.unsplash.com/photo-1604881988758-f76ad2f7aac1?auto=format&fit=crop&w=1650&q=80');
      background-size: cover;
      background-position: center;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 0 20px;
    }

    .hero h1 {
      font-size: 48px;
      margin-bottom: 20px;
    }

    .hero span {
      color: var(--green-main);
    }

    .hero p {
      max-width: 700px;
      margin: 0 auto 30px;
      font-size: 18px;
      opacity: 0.9;
    }

    .btn {
      padding: 14px 32px;
      border-radius: 30px;
      border: none;
      background: var(--green-main);
      color: #0b0f0d;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 10px 25px rgba(29, 185, 84, 0.3);
    }

    /* SECTIONS */
    section {
      padding: 90px 8%;
    }

    .section-title {
      text-align: center;
      margin-bottom: 60px;
    }

    .section-title h2 {
      font-size: 36px;
      margin-bottom: 10px;
    }

    .section-title p {
      opacity: 0.8;
    }

    /* CARDS */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }

    .card {
      background: var(--card-dark);
      padding: 30px;
      border-radius: 16px;
      transition: transform 0.3s, border 0.3s;
      border: 1px solid transparent;
    }

    .card:hover {
      transform: translateY(-6px);
      border: 1px solid var(--green-main);
    }

    .card h3 {
      margin-bottom: 12px;
      color: var(--green-soft);
    }

    /* FOOTER */
    footer {
      background: #070a08;
      padding: 40px 8%;
      text-align: center;
      font-size: 14px;
      opacity: 0.8;
    }

    @media (max-width: 768px) {
      .hero h1 {
        font-size: 36px;
      }
  </style>
</head>
<body id="top">

  <!-- HEADER -->
  <header>
    <a href="#top" class="logo" style="text-decoration:none; color:inherit;">
      <div class="logo-icon">S4</div>
      <div class="logo-text">Scholars 4 Success</div>
    </a>
    <nav>
      <a href="#about">About</a>
      <a href="#programs">Programs</a>
      <a href="#mentors">Mentors</a>
      <a href="#impact">Impact</a>
      <a href="#contact">Contact</a>
      <a href="#donate" class="donate-btn">Donate</a>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div>
      <h1>Empowering the Next Generation of <span>Students</span></h1>
      <p>
        Scholars 4 Success is a student-led nonprofit dedicated to teaching
        middle school math and science through free, accessible education.
      </p>
      <button class="btn">Learn More</button>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about">
    <div class="section-title">
      <h2>Our Mission</h2>
      <p>Built by students, for students</p>
    </div>
    <p style="max-width: 900px; margin: 0 auto; text-align: center;">
      Scholars 4 Success is a 501(c)(3) nonprofit founded by high school students
      with a mission to make quality math and science education accessible to
      middle school learners, regardless of background. Founded in Monroe Township, New Jersey at Monroe Township High School (MTHS).
    </p>
  </section>

  <!-- PROGRAMS -->
  <section id="programs">
    <div class="section-title">
      <h2>Book a Session</h2>
      <p>One-on-one academic support</p>
    </div>
    <div class="card-grid">
      <a href="#book-math" class="card" style="text-decoration:none; color:inherit;">
        <h3>Middle School Math</h3>
        <p>Book a personalized session covering arithmetic, pre-algebra, and problem solving.</p>
      </a>
      <a href="#book-science" class="card" style="text-decoration:none; color:inherit;">
        <h3>Middle School Science</h3>
        <p>Schedule help with biology, chemistry, and physical science topics.</p>
      </a>
    </div>
  </section>

  <!-- IMPACT -->
  <!-- MENTORS -->
  <!-- BOOKING PAGES -->
  <section id="book-math">
    <div class="section-title">
      <h2>Book a Math Session</h2>
      <p>One-on-one middle school math support</p>
    </div>
    <div style="max-width:700px; margin:0 auto; text-align:center;">
      <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfPLACEHOLDER_MATH/viewform?embedded=true" width="100%" height="900" frameborder="0">Loading…</iframe>
    </div>
  </section>

  <section id="book-science">
    <div class="section-title">
      <h2>Book a Science Session</h2>
      <p>One-on-one middle school science support</p>
    </div>
    <div style="max-width:700px; margin:0 auto; text-align:center;">
      <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfPLACEHOLDER_SCIENCE/viewform?embedded=true" width="100%" height="900" frameborder="0">Loading…</iframe>
    </div>
  </section>

  <!-- MENTORS -->
  <section id="mentors">
    <div class="section-title">
      <h2>Meet the Mentors</h2>
      <p>Dedicated student volunteers</p>
    </div>
    <div class="card-grid">
      <div class="card">
        <h3>Mentor Name</h3>
        <p>Grade · Subject Focus · Short bio goes here.</p>
      </div>
      <div class="card">
        <h3>Mentor Name</h3>
        <p>Grade · Subject Focus · Short bio goes here.</p>
      </div>
      <div class="card">
        <h3>Mentor Name</h3>
        <p>Grade · Subject Focus · Short bio goes here.</p>
      </div>
    </div>
  </section>

  <section id="impact">
    <div class="section-title">
      <h2>Our Impact</h2>
      <p>Education that creates opportunity</p>
    </div>
    <div class="card-grid">
      <div class="card">
        <h3>Free Access</h3>
        <p>All programs are offered at no cost to students and families.</p>
      </div>
      <div class="card">
        <h3>Student-Led</h3>
        <p>Run by motivated high school students committed to service.</p>
      </div>
      <div class="card">
        <h3>Community Focused</h3>
        <p>Partnering with schools and communities to close learning gaps.</p>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <div class="section-title">
      <h2>Get Involved</h2>
      <p>Learn, volunteer, or support our mission</p>
    </div>
    <p style="text-align:center;">Email us at <strong>scholars4success28@gmail.com</strong></p>
  </section>

  <!-- DONATE -->
  <section id="donate">
    <div class="section-title">
      <h2>Support Our Mission</h2>
      <p>Your donation helps us provide free education</p>
    </div>
    <div style="text-align:center;">
      <form action="https://www.paypal.com/donate" method="post" target="_blank">
        <input type="hidden" name="business" value="scholars4success28@gmail.com" />
        <input type="hidden" name="currency_code" value="USD" />
        <button class="btn">Donate with PayPal</button>
      </form>
    </div>
  </section>

  <footer>
    © 2026 Scholars 4 Success · Student-Led Nonprofit Organization
  </footer>

</body>
</html>
