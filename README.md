# Serenity-Touch-Massage-Spa
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Serenity Massage Spa</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
    }

    body{
      font-family:'Poppins', sans-serif;
      background:#f8f5f1;
      color:#333;
      line-height:1.6;
    }

    header{
      background:linear-gradient(rgba(0,0,0,.45), rgba(0,0,0,.45)),
      url('https://images.unsplash.com/photo-1544161515-4ab6ce6db874?q=80&w=1600&auto=format&fit=crop');
      background-size:cover;
      background-position:center;
      height:100vh;
      color:#fff;
      display:flex;
      flex-direction:column;
    }

    nav{
      display:flex;
      justify-content:space-between;
      align-items:center;
      padding:25px 8%;
      background:rgba(0,0,0,0.2);
      backdrop-filter:blur(6px);
      position:fixed;
      width:100%;
      z-index:1000;
    }

    .logo{
      font-size:28px;
      font-weight:700;
      letter-spacing:1px;
    }

    .logo span{
      color:#d8b48f;
    }

    nav ul{
      display:flex;
      list-style:none;
      gap:30px;
    }

    nav ul li a{
      text-decoration:none;
      color:#fff;
      font-weight:500;
      transition:.3s;
    }

    nav ul li a:hover{
      color:#d8b48f;
    }

    .hero{
      flex:1;
      display:flex;
      justify-content:center;
      align-items:center;
      text-align:center;
      padding:20px;
    }

    .hero-content h1{
      font-size:64px;
      margin-bottom:20px;
    }

    .hero-content p{
      font-size:20px;
      max-width:700px;
      margin:auto;
      margin-bottom:35px;
    }

    .btn{
      display:inline-block;
      padding:14px 34px;
      background:#d8b48f;
      color:#fff;
      text-decoration:none;
      border-radius:40px;
      font-weight:600;
      transition:.3s;
    }

    .btn:hover{
      background:#b8926f;
      transform:translateY(-2px);
    }

    section{
      padding:90px 8%;
    }

    .section-title{
      text-align:center;
      margin-bottom:60px;
    }

    .section-title h2{
      font-size:40px;
      color:#5d4c42;
      margin-bottom:10px;
    }

    .services{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(250px, 1fr));
      gap:30px;
    }

    .service-card{
      background:#fff;
      padding:35px;
      border-radius:18px;
      box-shadow:0 5px 20px rgba(0,0,0,0.08);
      transition:.3s;
    }

    .service-card:hover{
      transform:translateY(-8px);
    }

    .service-card h3{
      margin-bottom:15px;
      color:#8a6a53;
    }

    .about{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(320px, 1fr));
      gap:50px;
      align-items:center;
    }

    .about img{
      width:100%;
      border-radius:20px;
      box-shadow:0 10px 25px rgba(0,0,0,0.15);
    }

    .about-text h2{
      font-size:42px;
      margin-bottom:20px;
      color:#5d4c42;
    }

    .testimonials{
      display:grid;
      grid-template-columns:repeat(auto-fit, minmax(280px, 1fr));
      gap:30px;
    }

    .testimonial{
      background:#fff;
      padding:30px;
      border-radius:18px;
      box-shadow:0 5px 20px rgba(0,0,0,0.08);
    }

    .testimonial h4{
      margin-top:20px;
      color:#8a6a53;
    }

    .booking{
      background:#fff;
      border-radius:20px;
      padding:50px;
      max-width:800px;
      margin:auto;
      box-shadow:0 10px 25px rgba(0,0,0,0.08);
    }

    form{
      display:grid;
      gap:20px;
    }

    input, textarea{
      width:100%;
      padding:15px;
      border:1px solid #ddd;
      border-radius:12px;
      font-size:16px;
      outline:none;
    }

    textarea{
      resize:none;
      height:140px;
    }

    button{
      border:none;
      cursor:pointer;
      font-size:16px;
    }

    footer{
      background:#2c2c2c;
      color:#fff;
      text-align:center;
      padding:30px 20px;
      margin-top:60px;
    }

    @media(max-width:768px){
      .hero-content h1{
        font-size:42px;
      }

      nav{
        flex-direction:column;
        gap:15px;
      }

      nav ul{
        gap:15px;
      }
    }
  </style>
</head>

<body>

  <header>
    <nav>
      <div class="logo">Serenity <span>Spa</span></div>

      <ul>
        <li><a href="#services">Services</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#testimonials">Reviews</a></li>
        <li><a href="#booking">Book Now</a></li>
      </ul>
    </nav>

    <div class="hero">
      <div class="hero-content">
        <h1>Relax. Refresh. Rejuvenate.</h1>
        <p>
          Experience luxury wellness treatments and calming massage therapy
          designed to restore balance to your mind and body.
        </p>

        <a href="#booking" class="btn">Book Appointment</a>
      </div>
    </div>
  </header>

  <section id="services">
    <div class="section-title">
      <h2>Our Services</h2>
      <p>Premium spa treatments tailored for your relaxation.</p>
    </div>

    <div class="services">
      <div class="service-card">
        <h3>Swedish Massage</h3>
        <p>
          Gentle full-body massage designed to reduce stress and improve circulation.
        </p>
      </div>

      <div class="service-card">
        <h3>Deep Tissue Massage</h3>
        <p>
          Focused therapy that relieves muscle tension and chronic pain.
        </p>
      </div>

      <div class="service-card">
        <h3>Hot Stone Therapy</h3>
        <p>
          Smooth heated stones relax muscles and promote deep relaxation.
        </p>
      </div>

      <div class="service-card">
        <h3>Aromatherapy</h3>
        <p>
          Essential oils combined with massage to calm the body and mind.
        </p>
      </div>
    </div>
  </section>

  <section id="about">
    <div class="about">
      <img src="https://images.unsplash.com/photo-1515377905703-c4788e51af15?q=80&w=1200&auto=format&fit=crop" alt="Spa">

      <div class="about-text">
        <h2>About Serenity Massage Spa</h2>

        <p>
          At Serenity Massage Spa, we believe wellness begins with relaxation.
          Our certified therapists provide personalized treatments in a peaceful,
          luxurious environment designed to help you recharge and heal.
        </p>

        <br>

        <p>
          Whether you seek stress relief, pain recovery, or a rejuvenating spa day,
          our team is dedicated to delivering a calming and unforgettable experience.
        </p>
      </div>
    </div>
  </section>

  <section id="testimonials">
    <div class="section-title">
      <h2>Client Testimonials</h2>
      <p>What our guests say about us.</p>
    </div>

    <div class="testimonials">
      <div class="testimonial">
        <p>
          “Absolutely the best massage experience I’ve ever had.
          The atmosphere was peaceful and the staff were amazing.”
        </p>

        <h4>— Sarah M.</h4>
      </div>

      <div class="testimonial">
        <p>
          “Professional therapists and beautiful ambiance.
          I left feeling completely refreshed and relaxed.”
        </p>

        <h4>— David R.</h4>
      </div>

      <div class="testimonial">
        <p>
          “A luxury spa experience from start to finish.
          Highly recommended for stress relief.”
        </p>

        <h4>— Emily T.</h4>
      </div>
    </div>
  </section>

  <section id="booking">
    <div class="section-title">
      <h2>Book an Appointment</h2>
      <p>Schedule your relaxing spa session today.</p>
    </div>

    <div class="booking">
      <form>
        <input type="text" placeholder="Full Name" required>
        <input type="email" placeholder="Email Address" required>
        <input type="tel" placeholder="Phone Number" required>

        <textarea placeholder="Preferred service and booking details"></textarea>

        <button class="btn" type="submit">Submit Booking</button>
      </form>
    </div>
  </section>

  <footer>
    <p>© 2026 Serenity Massage Spa — All Rights Reserved</p>
  </footer>

</body>
</html>