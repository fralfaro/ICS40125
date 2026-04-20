# Perfiles Profesores

<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
:root {
  --navy: #0f1e35;
  --navy-mid: #162844;
  --gold: #c9a84c;
  --gold-light: #e8c87a;
  --cream-dark: #ede6d6;
  --text: #1a2a40;
  --white: #ffffff;
  --card-bg: #ffffff;
  --border: rgba(201,168,76,0.25);
}

.profiles-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
  margin: 1.5rem 0 2rem;
  align-items: stretch;
}

.pcard {
  background: var(--card-bg);
  border-radius: 14px;
  border: 1px solid var(--border);
  overflow: hidden;
  display: flex;
  flex-direction: column;
  box-shadow: 0 4px 20px rgba(15,30,53,0.08);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  opacity: 0;
  animation: fadeUp 0.5s ease forwards;
  font-family: 'DM Sans', sans-serif;
}
.pcard:nth-child(1) { animation-delay: 0.08s; }
.pcard:nth-child(2) { animation-delay: 0.18s; }
.pcard:nth-child(3) { animation-delay: 0.28s; }
.pcard:hover {
  transform: translateY(-5px);
  box-shadow: 0 14px 40px rgba(15,30,53,0.14);
}

.pcard-top {
  background: linear-gradient(145deg, var(--navy) 0%, var(--navy-mid) 100%);
  padding: 1.6rem 1.25rem 0;
  text-align: center;
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.pcard-top::after {
  content: '';
  position: absolute;
  bottom: -1px; left: 0; right: 0;
  height: 26px;
  background: var(--card-bg);
  clip-path: ellipse(55% 100% at 50% 100%);
}

.pavatar-wrap {
  position: relative;
  display: inline-block;
}
.pavatar-wrap::before {
  content: '';
  position: absolute;
  inset: -4px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--gold), var(--gold-light), var(--gold));
  z-index: 0;
}
.pavatar {
  width: 88px; height: 88px;
  border-radius: 50%;
  object-fit: cover;
  position: relative; z-index: 1;
  border: 3px solid var(--navy);
  display: block;
}
.pavatar-placeholder {
  width: 88px; height: 88px;
  border-radius: 50%;
  background: linear-gradient(135deg, #2a3f5f, #1a2d45);
  display: flex; align-items: center; justify-content: center;
  font-family: 'DM Serif Display', serif;
  font-size: 1.8rem;
  color: var(--gold-light);
  position: relative; z-index: 1;
  border: 3px solid var(--navy);
}

.pcard-namebox {
  height: 54px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 0.7rem;
  padding-bottom: 1.1rem;
  position: relative; z-index: 1;
  width: 100%;
}
.pcard-name {
  font-family: 'DM Serif Display', serif;
  font-size: 1.05rem;
  color: var(--white);
  line-height: 1.25;
  margin: 0;
  text-align: center;
}

.pcard-body {
  padding: 1.4rem 1.2rem 1rem;
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}
.pinfo {
  display: flex;
  align-items: flex-start;
  gap: 0.55rem;
  font-size: 0.81rem;
  color: var(--text);
  line-height: 1.4;
}
.pinfo-icon { font-size: 0.9rem; flex-shrink: 0; margin-top: 0.1rem; }

.pcard-footer {
  padding: 0.8rem 1.2rem 1.2rem;
  border-top: 1px solid var(--cream-dark);
  margin-top: auto;
}
.plink {
  display: inline-flex; align-items: center; gap: 0.35rem;
  font-size: 0.74rem; font-weight: 600; letter-spacing: 0.04em;
  text-decoration: none;
  padding: 0.38rem 0.85rem;
  border-radius: 6px;
  background: #bedfff;
  color: #ffffff;
  transition: background 0.2s ease;
}
.plink:hover { background: #0854a0; }

@keyframes fadeUp {
  from { opacity: 0; transform: translateY(20px); }
  to   { opacity: 1; transform: translateY(0); }
}

@media (max-width: 700px) {
  .profiles-grid { grid-template-columns: 1fr; }
}
</style>

<div class="profiles-grid">

  <!-- Sebastián Azócar -->
  <div class="pcard">
    <div class="pcard-top">
      <div class="pavatar-wrap">
        <img src="images/perfil_seba.png" alt="Sebastián Azócar" class="pavatar"
             onerror="this.outerHTML='<div class=&quot;pavatar-placeholder&quot;>SA</div>'">
      </div>
      <div class="pcard-namebox">
        <h3 class="pcard-name">Sebastián<br>Azócar</h3>
      </div>
    </div>
    <div class="pcard-body">
      <div class="pinfo"><span class="pinfo-icon">👨‍🎓</span><span>Ingeniero Matemático y Magíster en Ciencia de Datos</span></div>
    </div>
    <div class="pcard-footer">
      <a href="https://www.linkedin.com/in/sebasti%C3%A1n-az%C3%B3car/" target="_blank" class="plink">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
        LinkedIn
      </a>
    </div>
  </div>

  <!-- Fernando Díaz -->
  <div class="pcard">
    <div class="pcard-top">
      <div class="pavatar-wrap">
        <img src="images/perfil_fernando.png" alt="Fernando Díaz" class="pavatar"
             onerror="this.outerHTML='<div class=&quot;pavatar-placeholder&quot;>FD</div>'">
      </div>
      <div class="pcard-namebox">
        <h3 class="pcard-name">Fernando<br>Díaz H., PhD</h3>
      </div>
    </div>
    <div class="pcard-body">
      <div class="pinfo"><span class="pinfo-icon">🎓</span><span>Ph.D. Finanzas (Purdue) · MSc Finanzas y Economía (LSE) · MA Economía (PUC)</span></div>
    </div>
    <div class="pcard-footer">
      <a href="https://www.linkedin.com/in/frdiazh/" target="_blank" class="plink">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
        LinkedIn
      </a>
    </div>
  </div>

  <!-- Francisco Alfaro -->
  <div class="pcard">
    <div class="pcard-top">
      <div class="pavatar-wrap">
        <img src="images/perfil_francisco.png" alt="Francisco Alfaro" class="pavatar"
             onerror="this.outerHTML='<div class=&quot;pavatar-placeholder&quot;>FA</div>'">
      </div>
      <div class="pcard-namebox">
        <h3 class="pcard-name">Francisco<br>Alfaro M.</h3>
      </div>
    </div>
    <div class="pcard-body">
      <div class="pinfo"><span class="pinfo-icon">👨‍🎓</span><span>Ingeniero Matemático · Doctorado en Ingeniería Electrónica (UTFSM)</span></div>
    </div>
    <div class="pcard-footer">
      <a href="https://www.linkedin.com/in/faam/" target="_blank" class="plink">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="currentColor"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
        LinkedIn
      </a>
    </div>
  </div>

</div>

> 💡 Los tres profesionales colaboran en el curso de **Ciencia de Datos aplicado a la Gestión y Negocios** en la Universidad Técnica Federico Santa María.