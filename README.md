<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>School & Friends - Mantavya, Priyank & Team</title>
  <meta name="description" content="Website of Mantavya, Priyank & Friends - School Projects and Fun">
  <style>
    :root{--accent:#2563eb;--bg:#f8fafc;--card:#ffffff;--muted:#6b7280}
    *{box-sizing:border-box}
    body{font-family:Inter, system-ui, Arial, Helvetica, sans-serif;margin:0;background:var(--bg);color:#111}
    header{background:linear-gradient(90deg,var(--accent),#4f46e5);color:white;padding:14px 20px}
    .container{max-width:1000px;margin:0 auto;padding:20px}
    nav{display:flex;align-items:center;justify-content:space-between}
    .brand{font-weight:700;letter-spacing:0.4px}
    .navlinks{display:flex;gap:14px}
    .navlinks a{color:rgba(255,255,255,0.95);text-decoration:none;font-weight:600}
    .mobile-toggle{display:none;background:transparent;border:0;color:white;font-size:20px}.hero{display:grid;grid-template-columns:1fr 320px;gap:20px;align-items:center;margin-top:28px}
.card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(15,23,42,0.06)}
h1{margin:0 0 8px;font-size:28px}
p.lead{color:var(--muted);margin:0}

.quick-links{display:flex;gap:10px;margin-top:14px}
.btn{display:inline-block;padding:10px 14px;border-radius:8px;text-decoration:none;font-weight:700;cursor:pointer}
.btn-primary{background:var(--accent);color:white;border:0}
.btn-ghost{background:transparent;border:2px solid rgba(37,99,235,0.12);color:var(--accent)}

.features{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:18px}
.feature h3{margin:0 0 8px}
.gallery{display:grid;grid-template-columns:repeat(4,1fr);gap:8px;margin-top:18px}
.gallery img{width:100%;height:100px;object-fit:cover;border-radius:8px}

.members{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:16px;margin-top:18px}
.member{background:var(--card);padding:12px;border-radius:10px;box-shadow:0 4px 10px rgba(0,0,0,0.05);text-align:center}
.member img{width:80px;height:80px;border-radius:50%;object-fit:cover;margin-bottom:6px}

#guestbookEntries{margin-top:10px}
.entry{background:#eef2ff;padding:10px;border-radius:8px;margin-bottom:8px}

footer{padding:20px;text-align:center;color:var(--muted);margin-top:28px}

@media (max-width:900px){
  .hero{grid-template-columns:1fr}
  .features{grid-template-columns:repeat(2,1fr)}
  .gallery{grid-template-columns:repeat(2,1fr)}
}
@media (max-width:600px){
  .navlinks{display:none}
  .mobile-toggle{display:block}
  .features{grid-template-columns:1fr}
  .gallery img{height:120px}
}

  </style>
</head>
<body>
  <header>
    <div class="container">
      <nav>
        <div class="brand">School & Friends - Mantavya & Priyank</div>
        <div class="navlinks">
          <a href="#home">Home</a>
          <a href="#about">About</a>
          <a href="#members">Members</a>
          <a href="#projects">Projects</a>
          <a href="#gallery">Gallery</a>
          <a href="#guestbook">Guestbook</a>
          <a href="#contact">Contact</a>
        </div>
        <button class="mobile-toggle" aria-label="Menu" onclick="toggleMenu()">☰</button>
      </nav>
    </div>
  </header>  <main class="container">
    <section id="home" class="hero">
      <div class="card">
        <h1>Welcome to Our School & Friends Website</h1>
        <p class="lead">Made by <strong>Mantavya</strong>, <strong>Priyank</strong>, and their awesome classmates — a fun space to share memories, projects, and school life!</p>
        <div class="quick-links">
          <a class="btn btn-primary" href="#projects">See Projects</a>
          <a class="btn btn-ghost" href="#guestbook">Sign Guestbook</a>
        </div>
      </div><aside>
    <div class="card">
      <h3>Quick Contact</h3>
      <form id="contactForm" onsubmit="submitContact(event)">
        <label>Name</label>
        <input id="name" required style="width:100%;padding:8px;border-radius:6px;border:1px solid #e6e6e6">
        <label>Message</label>
        <textarea id="message" required style="width:100%;padding:8px;border-radius:6px;border:1px solid #e6e6e6"></textarea>
        <button class="btn btn-primary" style="width:100%;margin-top:10px">Send</button>
      </form>
    </div>
  </aside>
</section>

<section id="about" style="margin-top:22px">
  <div class="card">
    <h2>About Our School Group</h2>
    <p class="lead">We are a creative bunch of friends who love coding, drawing, and having fun while learning. This site is a collection of our school memories and achievements.</p>
  </div>
</section>

<section id="members" style="margin-top:22px">
  <div class="card">
    <h2>Team Members</h2>
    <div class="members">
      <div class="member"><img src="https://via.placeholder.com/100?text=M" alt="Mantavya"><h4>Mantavya</h4><p class="muted">Leader & Coder</p></div>
      <div class="member"><img src="https://via.placeholder.com/100?text=P" alt="Priyank"><h4>Priyank</h4><p class="muted">Designer & Organizer</p></div>
      <div class="member"><img src="https://via.placeholder.com/100?text=R" alt="Rohan"><h4>Rohan</h4><p class="muted">Photographer</p></div>
      <div class="member"><img src="https://via.placeholder.com/100?text=A" alt="Aarav"><h4>Aarav</h4><p class="muted">Project Researcher</p></div>
    </div>
  </div>
</section>

<section id="projects" style="margin-top:22px">
  <div class="card">
    <h2>Projects & Assignments</h2>
    <div style="display:grid;grid-template-columns:repeat(2,1fr);gap:12px;margin-top:12px">
      <div class="card">
        <h3>Science Fair</h3>
        <p class="muted">Our experiment on renewable energy created by Mantavya and Priyank.</p>
      </div>
      <div class="card">
        <h3>Art Collage</h3>
        <p class="muted">A creative collage made by our art group featuring school memories.</p>
      </div>
    </div>
  </div>
</section>

<section id="gallery" style="margin-top:22px">
  <div class="card">
    <h2>Gallery</h2>
    <div class="gallery" id="galleryGrid">
      <img src="https://via.placeholder.com/400x300?text=Science+Fair" alt="Science Fair">
      <img src="https://via.placeholder.com/400x300?text=Art+Day" alt="Art Day">
      <img src="https://via.placeholder.com/400x300?text=Sports+Event" alt="Sports Event">
      <img src="https://via.placeholder.com/400x300?text=Class+Trip" alt="Class Trip">
    </div>
  </div>
</section>

<section id="guestbook" style="margin-top:22px">
  <div class="card">
    <h2>Guestbook</h2>
    <p class="lead">Leave a message for Mantavya, Priyank, and the team!</p>
    <form id="guestForm" onsubmit="addEntry(event)">
      <input id="guestName" placeholder="Your name" required style="width:100%;padding:8px;border-radius:6px;border:1px solid #ddd;margin-top:8px">
      <textarea id="guestMessage" placeholder="Write a short message..." required style="width:100%;padding:8px;border-radius:6px;border:1px solid #ddd;margin-top:8px"></textarea>
      <button class="btn btn-primary" style="margin-top:10px">Post Message</button>
    </form>
    <div id="guestbookEntries"></div>
  </div>
</section>

<section id="contact" style="margin-top:22px">
  <div class="card">
    <h2>Contact & How to Publish</h2>
    <ol>
      <li>Save this file as <code>index.html</code>.</li>
      <li>Upload it to your hosting site or GitHub Pages.</li>
      <li>Replace images and member names with your real ones.</li>
    </ol>
  </div>
</section>

<footer>
  © <span id="year"></span> School & Friends — Mantavya, Priyank & Team
</footer>

  </main>  <script>
    document.getElementById('year').textContent = new Date().getFullYear();

    function toggleMenu(){
      const nav = document.querySelector('.navlinks');
      if(!nav) return;
      nav.style.display = nav.style.display === 'flex' ? 'none' : 'flex';
      nav.style.flexDirection = 'column';
      nav.style.background = 'rgba(255,255,255,0.06)';
      nav.style.position = 'absolute';
      nav.style.right = '20px';
      nav.style.top = '60px';
      nav.style.padding = '10px';
      nav.style.borderRadius = '8px';
    }

    // Simple guestbook using localStorage
    function addEntry(e){
      e.preventDefault();
      const name = document.getElementById('guestName').value.trim();
      const msg = document.getElementById('guestMessage').value.trim();
      if(!name || !msg) return;
      const entry = {name, msg, date: new Date().toLocaleString()};
      const entries = JSON.parse(localStorage.getItem('guestbook') || '[]');
      entries.unshift(entry);
      localStorage.setItem('guestbook', JSON.stringify(entries));
      document.getElementById('guestForm').reset();
      renderEntries();
    }

    function renderEntries(){
      const list = document.getElementById('guestbookEntries');
      const entries = JSON.parse(localStorage.getItem('guestbook') || '[]');
      list.innerHTML = entries.map(e => `<div class='entry'><strong>${e.name}</strong> <small>${e.date}</small><p>${e.msg}</p></div>`).join('');
    }

    renderEntries();

    function submitContact(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const msg = document.getElementById('message').value.trim();
      if(!name || !msg) return alert('Please fill both fields');
      const mailto = 'mailto:schoolfriends@example.com'
        + '?subject=' + encodeURIComponent('Message from ' + name)
        + '&body=' + encodeURIComponent(msg);
      window.location.href = mailto;
    }
  </script></body>
</html>
