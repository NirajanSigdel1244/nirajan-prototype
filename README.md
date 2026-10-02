<!DOCTYPE html>
<html lang="en-AU">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Riverside Community Clinic – Book a visit</title>
<meta name="description" content="Book a consultation, vaccination or telehealth appointment at Riverside Community Clinic.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Atkinson+Hyperlegible:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
<style>
:root{
  --paper:#FFFFFF; --ink:#15262E; --ink-soft:#3D525C; --river:#0A5770; --river-deep:#073F52;
  --mist:#E8F1F3; --line:#8FA7B0; --reed:#256B39; --reed-bg:#E6F2E8; --alert:#A4221B; --alert-bg:#FBEAE8;
  --focus:#FFBF47; --on-river:#FFFFFF;
  --font:"Atkinson Hyperlegible", Verdana, "Segoe UI", Arial, sans-serif;
  box-sizing:border-box;
  padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme:dark){
  :root:not([data-theme="light"]){
    --paper:#0F1E24; --ink:#EEF4F6; --ink-soft:#B9CBD1; --river:#7FC6DC; --river-deep:#A9DCEB;
    --mist:#18303A; --line:#5D7C87; --reed:#86D19A; --reed-bg:#173226; --alert:#FF9C93; --alert-bg:#3A1C1A;
    --on-river:#0F1E24;
  }
}
:root[data-theme="dark"]{
  --paper:#0F1E24; --ink:#EEF4F6; --ink-soft:#B9CBD1; --river:#7FC6DC; --river-deep:#A9DCEB;
  --mist:#18303A; --line:#5D7C87; --reed:#86D19A; --reed-bg:#173226; --alert:#FF9C93; --alert-bg:#3A1C1A;
  --on-river:#0F1E24;
}

:root[data-contrast="high"]{
  --paper:#000; --ink:#FFF; --ink-soft:#FFF; --river:#FFE600; --river-deep:#FFE600; --mist:#000;
  --line:#FFF; --reed:#7CFF8A; --reed-bg:#000; --alert:#FF8A80; --alert-bg:#000; --focus:#00E5FF; --on-river:#000;
}
:root[data-text="lg"]{font-size:118%}
:root[data-text="xl"]{font-size:136%}
*,*::before,*::after{box-sizing:inherit}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--paper);color:var(--ink);font-family:var(--font);font-size:1.125rem;line-height:1.6}
img,svg{max-width:100%}
a{color:var(--river)}
a:hover{text-decoration-thickness:3px}
h1,h2,h3{line-height:1.25;margin:0 0 .5em}
h1{font-size:2.1rem}
h2{font-size:1.5rem}
h3{font-size:1.2rem}
p{margin:0 0 1em;max-width:65ch}
:focus-visible{outline:4px solid var(--focus);outline-offset:2px;box-shadow:0 0 0 7px var(--ink)}
@media (prefers-reduced-motion:reduce){*{transition:none!important;animation:none!important;scroll-behavior:auto!important}}
.visually-hidden{position:absolute!important;width:1px;height:1px;overflow:hidden;clip:rect(0 0 0 0);white-space:nowrap}
.skip{position:absolute;left:1rem;top:-4rem;background:var(--focus);color:#000;padding:.75rem 1rem;font-weight:700;z-index:10}
.skip:focus{top:1rem}
.wrap{max-width:72rem;margin:0 auto;padding:0 1.25rem}


.utility{background:var(--river-deep);color:var(--on-river);font-size:1rem}
.utility .wrap{display:flex;flex-wrap:wrap;gap:.5rem 1.5rem;align-items:center;justify-content:space-between;padding-block:.5rem}
.utility a{color:var(--on-river);font-weight:700}
.tools{display:flex;flex-wrap:wrap;gap:.5rem;align-items:center}
.tools span{margin-right:.25rem}
.tool{font:inherit;font-size:.95rem;background:transparent;color:var(--on-river);border:2px solid var(--on-river);border-radius:6px;padding:.2rem .6rem;cursor:pointer;min-height:2.25rem}
.tool[aria-pressed="true"]{background:var(--on-river);color:var(--river-deep)}


header.site{border-bottom:1px solid var(--line)}
header.site .wrap{display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;gap:1rem;padding-block:1rem}
.brand{display:flex;align-items:center;gap:.75rem;color:var(--ink);text-decoration:none}
.brand strong{display:block;font-size:1.35rem;line-height:1.1}
.brand small{display:block;color:var(--ink-soft);font-size:.95rem}
nav ul{list-style:none;margin:0;padding:0;display:flex;flex-wrap:wrap;gap:.25rem}
nav a{display:inline-block;padding:.6rem .85rem;color:var(--ink);text-decoration:none;font-weight:700;border-bottom:4px solid transparent}
nav a:hover{border-bottom-color:var(--line)}
nav a[aria-current="page"]{border-bottom-color:var(--river);color:var(--river)}
.who{font-size:1rem;color:var(--ink-soft)}


.river{display:block;width:100%;height:28px;color:var(--river)}

main{padding:2rem 0 4rem}
.view[hidden]{display:none}


.hero{display:grid;grid-template-columns:1.2fr .8fr;gap:2.5rem;align-items:start;padding-bottom:1rem}
.hero h1{font-size:clamp(2rem,4.5vw,3rem);max-width:16ch}
.lede{font-size:1.25rem;color:var(--ink-soft)}
.search-big{display:flex;flex-wrap:wrap;gap:.75rem;margin-top:1.5rem;max-width:40rem}
.search-big input{flex:1 1 16rem}
.phone-card{background:var(--mist);border-left:6px solid var(--river);padding:1.25rem 1.5rem}
.phone-card p:last-child{margin:0}
.big-phone{font-size:1.6rem;font-weight:700}

.services{display:grid;grid-template-columns:repeat(3,1fr);gap:0;margin:2.5rem 0;border-top:2px solid var(--ink)}
.service{padding:1.25rem 1.5rem 1.5rem 0;border-right:1px solid var(--line)}
.service + .service{padding-left:1.5rem}
.service:last-child{border-right:0}
.service svg{width:44px;height:44px;color:var(--river)}
.service p{color:var(--ink-soft)}


.form{max-width:40rem}
.field{margin:0 0 1.5rem}
label,.label{display:block;font-weight:700;margin-bottom:.25rem}
.hint{display:block;color:var(--ink-soft);font-size:1rem;margin:-.1rem 0 .4rem}
input[type=text],input[type=email],input[type=tel],input[type=password],input[type=number],select{
  font:inherit;width:100%;padding:.65rem .75rem;border:2px solid var(--ink);border-radius:4px;background:var(--paper);color:var(--ink);min-height:3rem}
select{appearance:auto}
.w-short{max-width:8rem}.w-mid{max-width:18rem}
.dob{display:flex;gap:1rem;flex-wrap:wrap}
.dob div{display:flex;flex-direction:column}
.dob label{font-weight:400}
fieldset{border:0;margin:0 0 1.5rem;padding:0;min-width:0}
legend{font-weight:700;font-size:1.2rem;margin-bottom:.5rem;padding:0}
.check,.radio{display:flex;gap:.75rem;align-items:flex-start;margin:.5rem 0}
.check input,.radio input{width:1.6rem;height:1.6rem;margin:.1rem 0 0;flex:none;accent-color:var(--river)}
.check label,.radio label{font-weight:400;margin:0}
.field.has-error{border-left:5px solid var(--alert);padding-left:1rem}
.field.has-error input,.field.has-error select{border-color:var(--alert)}
.err{display:block;color:var(--alert);font-weight:700;margin:.1rem 0 .4rem}
.err:empty{display:none}
.pw{display:flex;gap:.5rem}
.pw input{flex:1}

.btn{font:inherit;font-weight:700;cursor:pointer;border-radius:6px;padding:.75rem 1.4rem;min-height:3rem;border:2px solid var(--river);background:var(--river);color:var(--on-river)}
.btn:hover{background:var(--river-deep);border-color:var(--river-deep)}
.btn.secondary{background:transparent;color:var(--river)}
.btn.secondary:hover{background:var(--mist)}
.btn.small{padding:.4rem .9rem;min-height:2.5rem;font-size:1rem}
.btn-row{display:flex;flex-wrap:wrap;gap:1rem;align-items:center;margin-top:2rem}
.linkbtn{font:inherit;background:none;border:0;color:var(--river);text-decoration:underline;cursor:pointer;padding:.25rem}

.error-summary{border:4px solid var(--alert);background:var(--alert-bg);padding:1rem 1.25rem;margin-bottom:2rem}
.error-summary ul{margin:.5rem 0 0;padding-left:1.25rem}
.error-summary a{color:var(--alert);font-weight:700}
.notice{background:var(--mist);border-left:6px solid var(--river);padding:1rem 1.25rem;margin:0 0 1.5rem}
.notice.ok{background:var(--reed-bg);border-color:var(--reed)}
.notice p:last-child{margin:0}
.lock{display:flex;gap:.6rem;align-items:flex-start}
.lock svg{flex:none;width:24px;height:24px;color:var(--reed);margin-top:.15rem}


.steps{list-style:none;padding:0;margin:0 0 2rem;display:flex;flex-wrap:wrap;gap:.25rem 0;counter-reset:s}
.steps li{counter-increment:s;display:flex;align-items:center;gap:.5rem;padding:.4rem .9rem .4rem 0;color:var(--ink-soft);font-size:1rem}
.steps li::before{content:counter(s);display:grid;place-items:center;width:2rem;height:2rem;border-radius:50%;border:2px solid var(--line);font-weight:700}
.steps li[aria-current="step"]{color:var(--ink);font-weight:700}
.steps li[aria-current="step"]::before{background:var(--river);border-color:var(--river);color:var(--on-river)}
.steps li.done::before{content:"✓";border-color:var(--reed);color:var(--reed)}


.rules{list-style:none;padding:0;margin:.5rem 0 0;font-size:1rem}
.rules li{display:flex;gap:.5rem;align-items:center}
.rules li::before{content:"○";font-weight:700;width:1.2rem;color:var(--ink-soft)}
.rules li.met{color:var(--reed)}
.rules li.met::before{content:"✓";color:var(--reed)}


.layout-find{display:grid;grid-template-columns:18rem 1fr;gap:2.5rem;align-items:start}
.filters{background:var(--mist);padding:1.25rem;border-radius:6px}
.filters .field{margin-bottom:1.1rem}
.results{list-style:none;margin:0;padding:0;border-top:2px solid var(--ink)}
.doc{display:grid;grid-template-columns:72px 1fr auto;gap:1.25rem;align-items:start;padding:1.25rem 0;border-bottom:1px solid var(--line)}
.doc h3{margin-bottom:.15rem}
.doc p{margin:.15rem 0;color:var(--ink-soft)}
.tags{display:flex;flex-wrap:wrap;gap:.4rem;margin:.5rem 0 0;padding:0;list-style:none}
.tags li{border:1px solid var(--line);border-radius:999px;padding:.05rem .65rem;font-size:.95rem}
.avatar{width:72px;height:72px}
.count{font-weight:700;margin:0 0 .75rem}


.layout-book{display:grid;grid-template-columns:1fr 20rem;gap:2.5rem;align-items:start}
.times{display:flex;flex-wrap:wrap;gap:.5rem}
.times .radio{margin:0}
.chip{position:relative}
.chip input{position:absolute;opacity:0;width:100%;height:100%;margin:0;cursor:pointer}
.chip label{display:block;border:2px solid var(--ink);border-radius:6px;padding:.5rem .9rem;font-weight:700;cursor:pointer}
.chip input:checked + label{background:var(--river);border-color:var(--river);color:var(--on-river)}
.chip input:focus-visible + label{outline:4px solid var(--focus);outline-offset:2px}
.qty{display:flex;align-items:center;gap:.5rem}
.qty input{width:5rem;text-align:center}
.summary{border:2px solid var(--ink);border-radius:6px;padding:1.25rem;position:sticky;top:calc(1rem + env(safe-area-inset-top,0px))}
.summary dl{display:grid;grid-template-columns:1fr auto;gap:.35rem 0;margin:0}
.summary dd{padding-left:1rem}
.summary dt{color:var(--ink-soft)}
.summary dd{margin:0;text-align:right;font-weight:700}
.summary .total{border-top:2px solid var(--ink);padding-top:.5rem;margin-top:.25rem;font-size:1.25rem}
.disc{color:var(--reed)}

.review{display:grid;grid-template-columns:auto 1fr auto;gap:.4rem 1.25rem;margin:0 0 1.5rem;border-top:1px solid var(--line);padding-top:.75rem}
.review dt{font-weight:700}
.review dd{margin:0}

footer{border-top:1px solid var(--line);padding:2rem 0;font-size:1rem;color:var(--ink-soft)}
footer .wrap{display:flex;flex-wrap:wrap;justify-content:space-between;gap:1rem}

@media (max-width:60rem){
  .hero,.layout-find,.layout-book{grid-template-columns:1fr}
  .summary{position:static}
}
@media (max-width:40rem){
  .services{grid-template-columns:1fr}
  .service,.service + .service{padding:1.25rem 0;border-right:0;border-bottom:1px solid var(--line)}
  .doc{grid-template-columns:56px 1fr}
  .doc .btn{grid-column:1 / -1}
  .avatar{width:56px;height:56px}
  .review{grid-template-columns:1fr auto}
  .review dd:not(.chg){grid-column:1 / -1}
}
</style>
</head>
<body>
<a class="skip" href="#main">Skip to main content</a>

<div class="utility">
  <div class="wrap">
    <p style="margin:0">Prefer to book by phone? <a href="tel:+61255501234">(02) 5550 1234</a>, weekdays 8am to 6pm</p>
    <div class="tools" role="group" aria-label="Display settings">
      <span>Text size</span>
      <button class="tool" type="button" data-size="md" aria-pressed="true" aria-label="Standard text size">A</button>
      <button class="tool" type="button" data-size="lg" aria-pressed="false" aria-label="Large text size">A+</button>
      <button class="tool" type="button" data-size="xl" aria-pressed="false" aria-label="Extra large text size">A++</button>
      <button class="tool" type="button" id="contrastBtn" aria-pressed="false">High contrast</button>
    </div>
  </div>
</div>

<header class="site">
  <div class="wrap">
    <a class="brand" href="#home">
      <svg width="52" height="52" viewBox="0 0 52 52" role="img" aria-label="Riverside Community Clinic logo">
        <rect x="2" y="2" width="48" height="48" rx="10" fill="var(--river)"/>
        <path d="M22 11h8v9h9v8h-9v4h-8v-4h-9v-8h9z" fill="var(--on-river)"/>
        <path d="M8 40c4-3 8-3 12 0s8 3 12 0 8-3 12 0" stroke="var(--on-river)" stroke-width="3" fill="none" stroke-linecap="round"/>
      </svg>
      <span><strong>Riverside Community Clinic</strong><small>General care for every age</small></span>
    </a>
    <nav aria-label="Main">
      <ul>
        <li><a href="#home" data-nav="home">Home</a></li>
        <li><a href="#find" data-nav="find">Find a doctor</a></li>
        <li><a href="#register" data-nav="register">Register</a></li>
        <li><a href="#login" data-nav="login" id="navLogin">Log in</a></li>
      </ul>
    </nav>
  </div>
  <svg class="river" viewBox="0 0 1200 28" preserveAspectRatio="none" aria-hidden="true" focusable="false">
    <path d="M0 14 C100 2 200 26 300 14 S500 2 600 14 800 26 900 14 1100 2 1200 14" fill="none" stroke="currentColor" stroke-width="3"/>
  </svg>
</header>

<main id="main" tabindex="-1">
  <div class="wrap">
    <div id="announcer" class="visually-hidden" aria-live="polite"></div>

  
    <section class="view" id="view-home" aria-labelledby="h-home">
      <div class="hero">
        <div>
          <h1 id="h-home" tabindex="-1">Book a visit with a Riverside doctor</h1>
          <p class="lede">See a GP in the clinic, get a vaccination, or talk to a doctor by video from home.</p>
          <form class="search-big" role="search" id="homeSearch" aria-label="Search doctors and services">
            <label for="q" class="visually-hidden">Search by doctor, specialty or service</label>
            <input type="text" id="q" name="q" placeholder="For example: flu vaccine, Dr Hart, children" autocomplete="off">
            <button class="btn" type="submit">Search</button>
          </form>
        </div>
        <aside class="phone-card" aria-label="Help with booking">
          <h2>New to Riverside?</h2>
          <p>Create an account once, then book any time. There is a one-off $10 joining fee.</p>
          <p><a href="#register" class="btn">Register as a new patient</a></p>
          <p>Already a patient? <a href="#login">Log in</a></p>
        </aside>
      </div>

      <h2 class="visually-hidden">Our services</h2>
      <div class="services">
        <div class="service">
          <svg viewBox="0 0 44 44" role="img" aria-label="Stethoscope icon"><path d="M12 6v12a8 8 0 0 0 16 0V6M20 26v6a6 6 0 0 0 12 0v-4" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round"/><circle cx="32" cy="25" r="3.5" fill="none" stroke="currentColor" stroke-width="3"/></svg>
          <h3>General consultation</h3>
          <p>Face-to-face appointments for check-ups, ongoing conditions and referrals.</p>
          <a href="#find" data-service="consultation">Find a consultation</a>
        </div>
        <div class="service">
          <svg viewBox="0 0 44 44" role="img" aria-label="Vaccine syringe icon"><path d="M30 6l8 8M34 10L16 28l-6 0 0-6L28 4M22 16l6 6M10 34l-4 4" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"/></svg>
          <h3>Vaccination</h3>
          <p>Flu, COVID-19, travel and childhood vaccines with a nurse or GP.</p>
          <a href="#find" data-service="vaccination">Find a vaccination</a>
        </div>
        <div class="service">
          <svg viewBox="0 0 44 44" role="img" aria-label="Video call icon"><rect x="4" y="11" width="26" height="22" rx="3" fill="none" stroke="currentColor" stroke-width="3"/><path d="M30 19l10-6v18l-10-6" fill="none" stroke="currentColor" stroke-width="3" stroke-linejoin="round"/></svg>
          <h3>Telehealth</h3>
          <p>Video or phone appointments. Book 4 or more sessions and get 10% off.</p>
          <a href="#find" data-service="telehealth">Find a telehealth session</a>
        </div>
      </div>
    </section>

   
    <section class="view" id="view-find" aria-labelledby="h-find">
      <h1 id="h-find" tabindex="-1">Find a doctor</h1>
      <p>Search by name, or narrow the list by service, specialty and day. Results update as you choose.</p>
      <div class="layout-find">
        <form class="filters" id="filters" role="search" aria-label="Filter doctors">
          <h2 style="font-size:1.2rem">Filter results</h2>
          <div class="field">
            <label for="fq">Search</label>
            <input type="text" id="fq" placeholder="Name or keyword">
          </div>
          <div class="field">
            <label for="fservice">Service</label>
            <select id="fservice">
              <option value="">Any service</option>
              <option value="consultation">General consultation</option>
              <option value="vaccination">Vaccination</option>
              <option value="telehealth">Telehealth</option>
            </select>
          </div>
          <div class="field">
            <label for="fspec">Specialty</label>
            <select id="fspec"><option value="">Any specialty</option></select>
          </div>
          <div class="field">
            <label for="fdate">Day</label>
            <select id="fdate"><option value="">Any day</option></select>
          </div>
          <button type="reset" class="btn secondary small">Clear filters</button>
        </form>
        <div>
          <p class="count" id="count" aria-live="polite"></p>
          <ul class="results" id="results"></ul>
        </div>
      </div>
    </section>

   
    <section class="view" id="view-book" aria-labelledby="h-book">
      <p><a href="#find">Back to doctors</a></p>
      <h1 id="h-book" tabindex="-1">Book with <span id="bookDoc"></span></h1>
      <div class="layout-book">
        <form id="bookForm" class="form" novalidate>
          <div id="bookErrors"></div>
          <fieldset class="field" id="f-bservice">
            <legend>Type of appointment</legend>
            <span class="err" id="e-bservice"></span>
            <div id="bservices"></div>
          </fieldset>
          <div class="field" id="f-bdate">
            <label for="bdate">Day</label>
            <span class="err" id="e-bdate"></span>
            <select id="bdate" class="w-mid" aria-describedby="e-bdate"></select>
          </div>
          <fieldset class="field" id="f-btime">
            <legend>Time</legend>
            <span class="err" id="e-btime"></span>
            <div class="times" id="btimes"></div>
          </fieldset>
          <div class="field" id="f-sessions" hidden>
            <label for="sessions">Number of telehealth sessions</label>
            <span class="hint" id="h-sessions">Weekly sessions starting on the day you chose. More than 3 sessions gets 10% off the total.</span>
            <div class="qty">
              <button type="button" class="btn secondary small" id="minus" aria-label="One fewer session">−</button>
              <input type="number" id="sessions" min="1" max="8" value="1" inputmode="numeric" aria-describedby="h-sessions">
              <button type="button" class="btn secondary small" id="plus" aria-label="One more session">+</button>
            </div>
          </div>
          <div class="btn-row"><button class="btn" type="submit">Confirm booking</button></div>
        </form>
        <aside class="summary" aria-labelledby="h-sum">
          <h2 id="h-sum" style="font-size:1.2rem">Your booking</h2>
          <dl id="sumList"></dl>
          <p class="hint" style="margin-top:1rem">Prototype prices. You pay at your appointment.</p>
        </aside>
      </div>
    </section>

   
    <section class="view" id="view-register" aria-labelledby="h-register">
      <h1 id="h-register" tabindex="-1">Register as a new patient</h1>
      <p>This takes about 5 minutes. You can go back and change anything before you pay.</p>
      <ol class="steps" id="steps" aria-label="Registration progress">
        <li>About you</li><li>Contacts</li><li>Account security</li><li>Joining fee</li><li>Consent and review</li>
      </ol>
      <form id="regForm" class="form" novalidate>
        <div id="regErrors"></div>

        <div class="step" data-step="0">
          <h2>About you</h2>
          <div class="field" id="f-fname">
            <label for="fname">First name</label>
            <span class="err" id="e-fname"></span>
            <input type="text" id="fname" autocomplete="given-name" aria-describedby="e-fname">
          </div>
          <div class="field" id="f-lname">
            <label for="lname">Last name</label>
            <span class="err" id="e-lname"></span>
            <input type="text" id="lname" autocomplete="family-name" aria-describedby="e-lname">
          </div>
          <fieldset class="field" id="f-dob" aria-describedby="h-dob e-dob">
            <legend>Date of birth</legend>
            <span class="hint" id="h-dob">For example, 27 3 1951. We use this to work out your age and match you to the right care.</span>
            <span class="err" id="e-dob"></span>
            <div class="dob">
              <div><label for="dd">Day</label><input type="text" id="dd" class="w-short" inputmode="numeric" maxlength="2" autocomplete="bday-day"></div>
              <div><label for="mm">Month</label><input type="text" id="mm" class="w-short" inputmode="numeric" maxlength="2" autocomplete="bday-month"></div>
              <div><label for="yy">Year</label><input type="text" id="yy" class="w-short" inputmode="numeric" maxlength="4" autocomplete="bday-year"></div>
            </div>
            <p id="age" aria-live="polite" style="margin:.75rem 0 0;font-weight:700"></p>
          </fieldset>
        </div>

        <div class="step" data-step="1">
          <h2>How we can reach you</h2>
          <div class="field" id="f-email">
            <label for="email">Email address</label>
            <span class="hint" id="h-email">You will use this to log in.</span>
            <span class="err" id="e-email"></span>
            <input type="email" id="email" autocomplete="email" spellcheck="false" aria-describedby="h-email e-email">
          </div>
          <div class="field" id="f-mobile">
            <label for="mobile">Mobile number</label>
            <span class="hint" id="h-mobile">For example, 0412 345 678</span>
            <span class="err" id="e-mobile"></span>
            <input type="tel" id="mobile" autocomplete="tel" class="w-mid" aria-describedby="h-mobile e-mobile">
          </div>
          <fieldset class="field">
            <legend>Emergency contact</legend>
            <p class="hint">Someone we can call if you become unwell during a visit.</p>
            <div class="field" id="f-ecname">
              <label for="ecname">Full name</label>
              <span class="err" id="e-ecname"></span>
              <input type="text" id="ecname" autocomplete="off" aria-describedby="e-ecname">
            </div>
            <div class="field" id="f-ecrel">
              <label for="ecrel">Relationship to you</label>
              <span class="err" id="e-ecrel"></span>
              <select id="ecrel" class="w-mid" aria-describedby="e-ecrel">
                <option value="">Choose one</option><option>Partner or spouse</option><option>Parent</option><option>Son or daughter</option><option>Other family member</option><option>Carer</option><option>Friend</option>
              </select>
            </div>
            <div class="field" id="f-ecphone">
              <label for="ecphone">Phone number</label>
              <span class="err" id="e-ecphone"></span>
              <input type="tel" id="ecphone" autocomplete="off" class="w-mid" aria-describedby="e-ecphone">
            </div>
          </fieldset>
        </div>

        <div class="step" data-step="2">
          <h2>Account security</h2>
          <div class="field" id="f-pw">
            <label for="pw">Create a password</label>
            <span class="hint" id="h-pw">A short sentence you will remember works well, like "river walk on sunday 9".</span>
            <span class="err" id="e-pw"></span>
            <div class="pw">
              <input type="password" id="pw" autocomplete="new-password" aria-describedby="h-pw rules e-pw">
              <button type="button" class="btn secondary small" data-toggle="pw" aria-controls="pw" aria-pressed="false">Show</button>
            </div>
            <ul class="rules" id="rules" aria-label="Password requirements">
              <li data-rule="len">At least 10 characters</li>
              <li data-rule="mix">Contains a letter and a number</li>
              <li data-rule="email">Is not your email address</li>
            </ul>
          </div>
          <div class="field" id="f-pw2">
            <label for="pw2">Type the password again</label>
            <span class="err" id="e-pw2"></span>
            <div class="pw">
              <input type="password" id="pw2" autocomplete="new-password" aria-describedby="e-pw2">
              <button type="button" class="btn secondary small" data-toggle="pw2" aria-controls="pw2" aria-pressed="false">Show</button>
            </div>
          </div>
          <fieldset class="field">
            <legend>Security questions</legend>
            <p class="hint">If you forget your password, we ask these before letting you reset it. Choose answers only you would know.</p>
            <div class="field" id="f-sq1">
              <label for="sq1">Question 1</label>
              <span class="err" id="e-sq1"></span>
              <select id="sq1" aria-describedby="e-sq1"></select>
            </div>
            <div class="field" id="f-sa1">
              <label for="sa1">Answer 1</label>
              <span class="err" id="e-sa1"></span>
              <input type="text" id="sa1" autocomplete="off" aria-describedby="e-sa1">
            </div>
            <div class="field" id="f-sq2">
              <label for="sq2">Question 2</label>
              <span class="err" id="e-sq2"></span>
              <select id="sq2" aria-describedby="e-sq2"></select>
            </div>
            <div class="field" id="f-sa2">
              <label for="sa2">Answer 2</label>
              <span class="err" id="e-sa2"></span>
              <input type="text" id="sa2" autocomplete="off" aria-describedby="e-sa2">
            </div>
          </fieldset>
        </div>

        <div class="step" data-step="3">
          <h2>Pay the $10 joining fee</h2>
          <div class="notice">
            <p>This is a one-off fee to set up your patient record. It is not a subscription and you will not be charged again.</p>
          </div>
          <div class="field" id="f-cname">
            <label for="cname">Name on card</label>
            <span class="err" id="e-cname"></span>
            <input type="text" id="cname" autocomplete="cc-name" aria-describedby="e-cname">
          </div>
          <div class="field" id="f-cnum">
            <label for="cnum">Card number</label>
            <span class="hint" id="h-cnum">The 16 digits on the front of your card. Try 4242 4242 4242 4242 in this prototype.</span>
            <span class="err" id="e-cnum"></span>
            <input type="text" id="cnum" inputmode="numeric" autocomplete="cc-number" maxlength="23" class="w-mid" aria-describedby="h-cnum e-cnum">
          </div>
          <div class="field" id="f-cexp">
            <label for="cexp">Expiry date</label>
            <span class="hint" id="h-cexp">MM/YY, for example 08/28</span>
            <span class="err" id="e-cexp"></span>
            <input type="text" id="cexp" inputmode="numeric" autocomplete="cc-exp" maxlength="5" class="w-short" aria-describedby="h-cexp e-cexp">
          </div>
          <div class="field" id="f-ccvc">
            <label for="ccvc">Security code</label>
            <span class="hint" id="h-ccvc">The last 3 digits on the back of your card</span>
            <span class="err" id="e-ccvc"></span>
            <input type="password" id="ccvc" inputmode="numeric" autocomplete="cc-csc" maxlength="4" class="w-short" aria-describedby="h-ccvc e-ccvc">
          </div>
          <div class="lock">
            <svg viewBox="0 0 24 24" role="img" aria-label="Padlock icon"><rect x="4" y="10" width="16" height="11" rx="2" fill="none" stroke="currentColor" stroke-width="2"/><path d="M8 10V7a4 4 0 0 1 8 0v3" fill="none" stroke="currentColor" stroke-width="2"/></svg>
            <p>Your card is processed over an encrypted connection by our payment provider. Riverside never stores your full card number or security code.</p>
          </div>
        </div>

        <div class="step" data-step="4">
          <h2>Consent and review</h2>
          <h3>Check your details</h3>
          <dl class="review" id="review"></dl>
          <fieldset class="field" id="f-consent">
            <legend>Storing your health record</legend>
            <p>We keep your details in an encrypted record that only Riverside clinical staff can open. We use them to provide your care and never sell or share them for marketing. You can ask to see, correct or delete your record at any time. <a href="#privacy">Read the full privacy notice</a>.</p>
            <span class="err" id="e-consent"></span>
            <div class="check">
              <input type="checkbox" id="consent" aria-describedby="e-consent">
              <label for="consent">I agree to Riverside Community Clinic storing my details securely to provide my care (required)</label>
            </div>
          </fieldset>
          <fieldset class="field">
            <legend>Optional messages</legend>
            <p class="hint">Leave these unticked if you do not want them. You can change this later in your account.</p>
            <div class="check">
              <input type="checkbox" id="optTips">
              <label for="optTips">Send me monthly health tips by email</label>
            </div>
            <div class="check">
              <input type="checkbox" id="optRem">
              <label for="optRem">Send me appointment reminders by text message</label>
            </div>
          </fieldset>
        </div>

        <div class="btn-row">
          <button type="button" class="btn secondary" id="regBack" hidden>Back</button>
          <button type="submit" class="btn" id="regNext">Continue</button>
        </div>
      </form>
    </section>

    
    <section class="view" id="view-login" aria-labelledby="h-login">
      <h1 id="h-login" tabindex="-1">Log in</h1>
      <p>Not registered yet? <a href="#register">Register as a new patient</a></p>
      <form id="loginForm" class="form" novalidate>
        <div id="loginErrors"></div>
        <div class="field" id="f-lemail">
          <label for="lemail">Email address</label>
          <span class="err" id="e-lemail"></span>
          <input type="email" id="lemail" autocomplete="username" spellcheck="false" aria-describedby="e-lemail">
        </div>
        <div class="field" id="f-lpw">
          <label for="lpw">Password</label>
          <span class="err" id="e-lpw"></span>
          <div class="pw">
            <input type="password" id="lpw" autocomplete="current-password" aria-describedby="e-lpw">
            <button type="button" class="btn secondary small" data-toggle="lpw" aria-controls="lpw" aria-pressed="false">Show</button>
          </div>
        </div>
        <div class="btn-row">
          <button class="btn" type="submit">Log in</button>
          <button class="linkbtn" type="button" id="forgotBtn" aria-expanded="false" aria-controls="forgot">Forgot your password?</button>
        </div>
      </form>
      <div id="forgot" class="form" hidden style="margin-top:2rem">
        <h2>Reset your password</h2>
        <p>Enter your email and answer one of your security questions. We will then send a reset link to your email.</p>
        <form id="forgotForm" novalidate>
          <div class="field" id="f-femail">
            <label for="femail">Email address</label>
            <span class="err" id="e-femail"></span>
            <input type="email" id="femail" autocomplete="username" aria-describedby="e-femail">
          </div>
          <div class="field" id="f-fans">
            <label for="fans">Security question: What was the name of your first school?</label>
            <span class="hint">This is one of the two questions you chose when you registered.</span>
            <span class="err" id="e-fans"></span>
            <input type="text" id="fans" autocomplete="off" aria-describedby="e-fans">
          </div>
          <button class="btn" type="submit">Send reset link</button>
        </form>
        <div id="forgotDone" role="status"></div>
      </div>
    </section>

    
    <section class="view" id="view-done" aria-labelledby="h-done">
      <div class="notice ok" style="max-width:40rem">
        <h1 id="h-done" tabindex="-1"></h1>
        <div id="doneBody"></div>
      </div>
      <div class="btn-row"><a class="btn" href="#find">Find a doctor</a><a class="btn secondary" href="#home">Go to home page</a></div>
    </section>

   
    <section class="view" id="view-privacy" aria-labelledby="h-privacy">
      <h1 id="h-privacy" tabindex="-1">Privacy notice</h1>
      <div class="form">
        <h2>What we collect</h2>
        <p>Your name, date of birth, contact details, emergency contact, appointment history and the answers to your security questions. We collect only what we need to provide your care.</p>
        <h2>How we protect it</h2>
        <p>Records are encrypted in storage and in transit. Passwords and security answers are stored as one-way hashes, so staff cannot read them. Card payments go straight to our payment provider; we keep only the last 4 digits as a receipt.</p>
        <h2>Your choices</h2>
        <p>Health tips and reminders are off unless you turn them on. You can ask to see, correct or delete your information by calling (02) 5550 1234. We handle your information under the Australian Privacy Principles.</p>
        <p><a href="#register">Back to registration</a></p>
      </div>
    </section>
  </div>
</main>

<footer>
  <div class="wrap">
    <p style="margin:0">Riverside Community Clinic. In an emergency, call 000.</p>
    <p style="margin:0"><a href="#privacy">Privacy notice</a>. Prototype only: nothing you enter is sent or stored.</p>
  </div>
</footer>

<script>
(function(){
  "use strict";
  const $ = s => document.querySelector(s);
  const $$ = s => Array.from(document.querySelectorAll(s));
  const announce = msg => { const a=$('#announcer'); a.textContent=''; setTimeout(()=>a.textContent=msg,50); };


  $$('.tool[data-size]').forEach(b=>b.addEventListener('click',()=>{
    $$('.tool[data-size]').forEach(x=>x.setAttribute('aria-pressed','false'));
    b.setAttribute('aria-pressed','true');
    document.documentElement.dataset.text=b.dataset.size;
  }));
  $('#contrastBtn').addEventListener('click',e=>{
    const on=e.currentTarget.getAttribute('aria-pressed')!=='true';
    e.currentTarget.setAttribute('aria-pressed',String(on));
    if(on) document.documentElement.dataset.contrast='high'; else delete document.documentElement.dataset.contrast;
  });


  $$('[data-toggle]').forEach(b=>b.addEventListener('click',()=>{
    const i=document.getElementById(b.dataset.toggle);
    const show=i.type==='password';
    i.type=show?'text':'password';
    b.textContent=show?'Hide':'Show';
    b.setAttribute('aria-pressed',String(show));
  }));

 
  const DAY = 864e5;
  const today = new Date(); today.setHours(0,0,0,0);
  const days = Array.from({length:14},(_,i)=>new Date(today.getTime()+(i+1)*DAY)).filter(d=>d.getDay()!==0);
  const fmt = d => d.toLocaleDateString('en-AU',{weekday:'long',day:'numeric',month:'long'});
  const iso = d => d.toISOString().slice(0,10);
  const SERVICE = {consultation:'General consultation',vaccination:'Vaccination',telehealth:'Telehealth'};
  const KEYWORDS = {consultation:'gp check-up checkup appointment in person',vaccination:'vaccine jab shot flu covid immunisation immunization travel',telehealth:'video phone online call remote'};
  const PRICE = {consultation:75,vaccination:25,telehealth:55};
  const pick = (arr,idx) => idx.map(i=>arr[i]).filter(Boolean);
  const doctors = [
    {id:'hart',name:'Dr Amelia Hart',spec:'General practice',services:['consultation','telehealth'],langs:'English, Auslan',days:pick(days,[0,2,4,6,8,10]),times:['9:00 am','10:30 am','2:00 pm']},
    {id:'nguyen',name:'Dr Minh Nguyen',spec:"Children's health",services:['consultation','vaccination'],langs:'English, Vietnamese',days:pick(days,[1,2,5,7,9]),times:['8:30 am','11:00 am','3:30 pm']},
    {id:'okafor',name:'Dr Grace Okafor',spec:"Older people's health",services:['consultation','telehealth'],langs:'English',days:pick(days,[0,1,3,5,9,11]),times:['10:00 am','1:00 pm','4:00 pm']},
    {id:'patel',name:'Nurse Ravi Patel',spec:'Immunisation',services:['vaccination'],langs:'English, Hindi, Gujarati',days:pick(days,[0,1,2,3,4,5,6]),times:['9:15 am','12:00 pm','2:45 pm']},
    {id:'russo',name:'Dr Lucia Russo',spec:'Mental health',services:['telehealth'],langs:'English, Italian',days:pick(days,[1,3,6,8,10]),times:['9:00 am','12:30 pm','5:00 pm']},
    {id:'walker',name:'Dr Tom Walker',spec:'General practice',services:['consultation','vaccination','telehealth'],langs:'English',days:pick(days,[2,4,7,9,11]),times:['8:00 am','11:30 am','3:00 pm']}
  ];
  const initials = n => n.replace(/^(Dr|Nurse)\s+/,'').split(' ').map(p=>p[0]).join('');
  const avatar = d => `<svg class="avatar" viewBox="0 0 72 72" role="img" aria-label="Placeholder portrait of ${d.name}"><circle cx="36" cy="36" r="34" fill="var(--mist)" stroke="var(--river)" stroke-width="3"/><text x="36" y="44" text-anchor="middle" font-family="inherit" font-size="22" font-weight="700" fill="var(--river)">${initials(d.name)}</text></svg>`;


  const titles = {home:'Book a visit',find:'Find a doctor',book:'Book an appointment',register:'Register',login:'Log in',done:'Confirmation',privacy:'Privacy notice'};
  function show(view, focus=true){
    if(!titles[view]) view='home';
    $$('.view').forEach(v=>v.hidden = v.id!=='view-'+view);
    $$('[data-nav]').forEach(a=>a.dataset.nav===view?a.setAttribute('aria-current','page'):a.removeAttribute('aria-current'));
    document.title = titles[view]+' – Riverside Community Clinic';
    if(focus){ const h=$('#view-'+view+' h1'); h && h.focus(); }
    if(view==='find') renderResults();
  }
  function navigate(view){
    show(view);
    try{ history.pushState({view},'', '#'+view); }catch(err){ /* embedded viewers may block URL changes; the view still switches */ }
    window.scrollTo(0,0);
  }
 
  document.addEventListener('click',e=>{
    const a=e.target.closest('a[href^="#"]');
    if(!a || a.hasAttribute('data-focus')) return;
    const view=a.getAttribute('href').slice(1);
    if(!titles[view]) return; // e.g. skip link to #main keeps default behaviour
    e.preventDefault();
    navigate(view);
  });
  window.addEventListener('popstate',e=>show((e.state&&e.state.view)||location.hash.slice(1)||'home'));
  window.addEventListener('hashchange',()=>show(location.hash.slice(1)));
  $$('[data-service]').forEach(a=>a.addEventListener('click',()=>{ $('#fservice').value=a.dataset.service; }));


  [...new Set(doctors.map(d=>d.spec))].sort().forEach(s=>$('#fspec').add(new Option(s,s)));
  days.forEach(d=>$('#fdate').add(new Option(fmt(d),iso(d))));
  $('#homeSearch').addEventListener('submit',e=>{ e.preventDefault(); $('#fq').value=$('#q').value.trim(); navigate('find'); });
  ['input','change'].forEach(ev=>$('#filters').addEventListener(ev,renderResults));
  $('#filters').addEventListener('reset',()=>setTimeout(renderResults,0));

  let lastKey=null;
  function renderResults(){
    const q=$('#fq').value.trim().toLowerCase(), sv=$('#fservice').value, sp=$('#fspec').value, dt=$('#fdate').value;
    const key=[q,sv,sp,dt].join('|'); if(key===lastKey) return; lastKey=key; // don't rebuild the list unless filters changed
    const list=doctors.filter(d=>{
      const text=(d.name+' '+d.spec+' '+d.services.map(s=>SERVICE[s]+' '+KEYWORDS[s]).join(' ')+' '+d.langs).toLowerCase();
      const words=q.split(/\s+/).filter(Boolean).map(w=>w.replace(/s$/,''));
      return words.every(w=>text.includes(w)) && (!sv||d.services.includes(sv)) && (!sp||d.spec===sp) && (!dt||d.days.some(x=>iso(x)===dt));
    });
    $('#count').textContent = list.length ? `${list.length} ${list.length===1?'doctor':'doctors'} found` : 'No doctors match these filters. Try choosing "Any day" or clearing the search.';
    $('#results').innerHTML = list.map(d=>`<li class="doc">${avatar(d)}<div><h3>${d.name}</h3><p>${d.spec}. Speaks ${d.langs}.</p><p>Next available: ${fmt(d.days[0])}</p><ul class="tags" aria-label="Services offered">${d.services.map(s=>`<li>${SERVICE[s]}</li>`).join('')}</ul></div><button class="btn small" type="button" data-book="${d.id}">Book<span class="visually-hidden"> with ${d.name}</span></button></li>`).join('');
  }
  $('#results').addEventListener('click',e=>{ const b=e.target.closest('[data-book]'); if(b) openBooking(b.dataset.book); });

  
  let current=null, user=null, pending=false;
  function openBooking(id){
    current=doctors.find(d=>d.id===id);
    $('#bookDoc').textContent=current.name;
    const pre=$('#fservice').value;
    $('#bservices').innerHTML=current.services.map((s,i)=>`<div class="radio"><input type="radio" name="bservice" id="bs-${s}" value="${s}" ${(pre?s===pre:i===0)?'checked':''}><label for="bs-${s}">${SERVICE[s]} ($${PRICE[s]}${s==='telehealth'?' per session':''})</label></div>`).join('');
    $('#bdate').innerHTML=current.days.map(d=>`<option value="${iso(d)}">${fmt(d)}</option>`).join('');
    const fd=$('#fdate').value; if(fd && current.days.some(d=>iso(d)===fd)) $('#bdate').value=fd;
    $('#btimes').innerHTML=current.times.map((t,i)=>`<div class="chip"><input type="radio" name="btime" id="bt-${i}" value="${t}"><label for="bt-${i}">${t}</label></div>`).join('');
    $('#sessions').value=1; clearErrors('#bookForm','#bookErrors');
    navigate('book'); updateSummary();
  }
  function updateSummary(){
    if(!current) return;
    const s=($('input[name=bservice]:checked')||{}).value;
    const tele=s==='telehealth';
    $('#f-sessions').hidden=!tele;
    let n=Math.min(8,Math.max(1,parseInt($('#sessions').value,10)||1));
    const sessions=tele?n:1, base=s?PRICE[s]*sessions:0, disc=tele&&sessions>3?base*0.1:0;
    const t=($('input[name=btime]:checked')||{}).value;
    const d=$('#bdate').selectedOptions[0];
    $('#sumList').innerHTML=`<dt>Doctor</dt><dd>${current.name}</dd><dt>Service</dt><dd>${s?SERVICE[s]:'Not chosen'}</dd><dt>Day</dt><dd>${d?d.text:''}</dd><dt>Time</dt><dd>${t||'Not chosen'}</dd>${tele?`<dt>Sessions</dt><dd>${sessions} × $${PRICE.telehealth}</dd>`:''}${disc?`<dt class="disc">Discount (10%)</dt><dd class="disc">−$${disc.toFixed(2)}</dd>`:''}<dt class="total">Total</dt><dd class="total">$${(base-disc).toFixed(2)}</dd>`;
    return {s,t,sessions,total:base-disc,disc,day:d?d.text:''};
  }
  $('#bookForm').addEventListener('change',updateSummary);
  $('#sessions').addEventListener('input',updateSummary);
  const step=k=>{ const i=$('#sessions'); i.value=Math.min(8,Math.max(1,(parseInt(i.value,10)||1)+k)); updateSummary(); announce(i.value+' sessions'+(i.value>3?', 10% discount applied':'')); };
  $('#plus').addEventListener('click',()=>step(1));
  $('#minus').addEventListener('click',()=>step(-1));
  $('#bookForm').addEventListener('submit',e=>{
    e.preventDefault();
    const sm=updateSummary(), errs=[];
    if(!sm.s) errs.push(['bservice','Choose a type of appointment','bs-'+current.services[0]]);
    if(!sm.t) errs.push(['btime','Choose a time for your appointment','bt-0']);
    if(showErrors('#bookForm','#bookErrors',errs)) return;
    if(!user){
      pending=true;
      $('#bookErrors').innerHTML='<div class="notice" role="alert" tabindex="-1"><h2 style="font-size:1.25rem">Log in to confirm this booking</h2><p>Your choices are saved on this page. <a href="#login">Log in</a> if you are already a patient, or <a href="#register">register as a new patient</a>, then come back to confirm.</p></div>';
      $('#bookErrors .notice').focus(); return;
    }
    pending=false;
    done('Appointment booked',`<p>${SERVICE[sm.s]} with ${current.name} on ${sm.day} at ${sm.t}${sm.sessions>1?`, then weekly for ${sm.sessions} sessions`:''}.</p><p>Total: $${sm.total.toFixed(2)}${sm.disc?` (includes $${sm.disc.toFixed(2)} telehealth discount)`:''}.</p><p>Booking reference: RCC-${Math.floor(100000+Math.random()*900000)}</p>`);
  });


  function clearErrors(form,box){
    $(box).innerHTML='';
    $$(form+' .has-error').forEach(f=>f.classList.remove('has-error'));
    $$(form+' .err').forEach(e=>e.textContent='');
    $$(form+' [aria-invalid]').forEach(i=>i.removeAttribute('aria-invalid'));
  }
 
  function showErrors(form,box,errs){
    clearErrors(form,box);
    if(!errs.length) return false;
    errs.forEach(([k,m,fid])=>{
      const f=document.getElementById('f-'+k); f&&f.classList.add('has-error');
      const e=document.getElementById('e-'+k); if(e) e.textContent='Error: '+m;
      const inp=document.getElementById(fid||k); inp&&inp.setAttribute('aria-invalid','true');
    });
    $(box).innerHTML=`<div class="error-summary" role="alert" tabindex="-1"><h2 style="font-size:1.25rem">There is a problem</h2><ul>${errs.map(([k,m,fid])=>`<li><a href="#${fid||k}" data-focus="${fid||k}">${m}</a></li>`).join('')}</ul></div>`;
    $(box+' .error-summary').focus();
    return true;
  }
  document.addEventListener('click',e=>{ const a=e.target.closest('[data-focus]'); if(a){ e.preventDefault(); const t=document.getElementById(a.dataset.focus); t&&t.focus(); }});


  const QS=['What was the name of your first school?','What is the name of the street you grew up on?','What was the name of your first pet?','What is your oldest sibling’s middle name?','In what town did your parents meet?'];
  ['sq1','sq2'].forEach((id,n)=>{ const s=$('#'+id); s.add(new Option('Choose a question','')); QS.forEach(q=>s.add(new Option(q,q))); });
  let st=0; const STEPS=$$('.step');
  const v=id=>$('#'+id).value.trim();
  const digits=s=>s.replace(/\D/g,'');
  const emailOk=s=>/^[^\s@]+@[^\s@]+\.[^\s@]{2,}$/.test(s);
  const phoneOk=s=>{const d=digits(s);return d.length>=8&&d.length<=12;};
  function dob(){
    const d=+v('dd'),m=+v('mm'),y=+v('yy');
    if(!d||!m||!y) return null;
    const dt=new Date(y,m-1,d);
    if(dt.getFullYear()!==y||dt.getMonth()!==m-1||dt.getDate()!==d) return 'bad';
    let age=today.getFullYear()-y; if(today<new Date(today.getFullYear(),m-1,d)) age--;
    return dt>today||age>120?'bad':age;
  }
  ['dd','mm','yy'].forEach(id=>$('#'+id).addEventListener('input',()=>{ const a=dob(); $('#age').textContent=typeof a==='number'?`Age: ${a}`:''; }));
  function luhn(n){let s=0,alt=false;for(let i=n.length-1;i>=0;i--){let x=+n[i];if(alt){x*=2;if(x>9)x-=9;}s+=x;alt=!alt;}return s%10===0;}
  $('#cnum').addEventListener('input',e=>{ const d=digits(e.target.value).slice(0,19); e.target.value=d.replace(/(.{4})/g,'$1 ').trim(); });
  $('#cexp').addEventListener('input',e=>{ const d=digits(e.target.value).slice(0,4); e.target.value=d.length>2?d.slice(0,2)+'/'+d.slice(2):d; });
  function pwRules(){
    const p=$('#pw').value, em=v('email').toLowerCase();
    const r={len:p.length>=10, mix:/[a-z]/i.test(p)&&/\d/.test(p), email:p.length>0&&p.toLowerCase()!==em};
    $$('#rules li').forEach(li=>li.classList.toggle('met',r[li.dataset.rule]));
    return r;
  }
  $('#pw').addEventListener('input',pwRules);

  function validate(n){
    const e=[];
    if(n===0){
      if(!v('fname')) e.push(['fname','Enter your first name']);
      if(!v('lname')) e.push(['lname','Enter your last name']);
      const a=dob();
      if(a===null) e.push(['dob','Enter your date of birth as day, month and year','dd']);
      else if(a==='bad') e.push(['dob','Date of birth must be a real date in the past','dd']);
    }
    if(n===1){
      if(!emailOk(v('email'))) e.push(['email','Enter an email address like name@example.com']);
      if(!phoneOk(v('mobile'))) e.push(['mobile','Enter a mobile number like 0412 345 678']);
      if(!v('ecname')) e.push(['ecname','Enter the name of your emergency contact']);
      if(!v('ecrel')) e.push(['ecrel','Choose how your emergency contact is related to you']);
      if(!phoneOk(v('ecphone'))) e.push(['ecphone','Enter a phone number for your emergency contact']);
    }
    if(n===2){
      const r=pwRules();
      if(!r.len||!r.mix||!r.email) e.push(['pw','Your password must meet all 3 requirements listed under it']);
      else if($('#pw').value!==$('#pw2').value) e.push(['pw2','The two passwords do not match']);
      if(!v('sq1')) e.push(['sq1','Choose your first security question']);
      if(!v('sa1')) e.push(['sa1','Answer your first security question']);
      if(!v('sq2')) e.push(['sq2','Choose your second security question']);
      else if(v('sq2')===v('sq1')) e.push(['sq2','Choose a different question from question 1']);
      if(!v('sa2')) e.push(['sa2','Answer your second security question']);
    }
    if(n===3){
      if(!v('cname')) e.push(['cname','Enter the name shown on your card']);
      const c=digits(v('cnum'));
      if(c.length<13||!luhn(c)) e.push(['cnum','Check the card number. It should be the long number on the front of your card']);
      const m=/^(\d{2})\/(\d{2})$/.exec(v('cexp'));
      if(!m||+m[1]<1||+m[1]>12) e.push(['cexp','Enter the expiry date as MM/YY']);
      else if(new Date(2000+ +m[2],+m[1],1)<=today) e.push(['cexp','This card has expired. Use a different card']);
      if(!/^\d{3,4}$/.test(v('ccvc'))) e.push(['ccvc','Enter the 3 or 4 digit security code']);
    }
    if(n===4){
      if(!$('#consent').checked) e.push(['consent','Tick the box to agree to us storing your details. We cannot create your record without it','consent']);
    }
    return e;
  }
  function goStep(n,quiet){
    st=n;
    STEPS.forEach((s,i)=>s.hidden=i!==n);
    $$('#steps li').forEach((li,i)=>{ li.classList.toggle('done',i<n); i===n?li.setAttribute('aria-current','step'):li.removeAttribute('aria-current'); });
    $('#regBack').hidden=n===0;
    $('#regNext').textContent=n===4?'Pay $10 and create account':'Continue';
    if(n===4) buildReview();
    clearErrors('#regForm','#regErrors');
    const h=STEPS[n].querySelector('h2'); h.setAttribute('tabindex','-1'); if(quiet) return; h.focus();
    announce(`Step ${n+1} of 5: ${h.textContent}`);
  }
  function buildReview(){
    const c=digits(v('cnum'));
    const rows=[['Name',v('fname')+' '+v('lname'),0],['Age',String(dob()),0],['Email',v('email'),1],['Mobile',v('mobile'),1],['Emergency contact',`${v('ecname')} (${v('ecrel')}), ${v('ecphone')}`,1],['Password','Set (hidden)',2],['Card','Ending in '+c.slice(-4)+', $10 joining fee',3]];
    $('#review').innerHTML=rows.map(([k,val,s])=>`<dt>${k}</dt><dd>${val.replace(/</g,'&lt;')}</dd><dd class="chg"><button type="button" class="linkbtn" data-goto="${s}">Change<span class="visually-hidden"> ${k.toLowerCase()}</span></button></dd>`).join('');
  }
  $('#review').addEventListener('click',e=>{ const b=e.target.closest('[data-goto]'); if(b) goStep(+b.dataset.goto); });
  $('#regBack').addEventListener('click',()=>goStep(st-1));
  $('#regForm').addEventListener('submit',e=>{
    e.preventDefault();
    if(showErrors('#regForm','#regErrors',validate(st))) return;
    if(st<4) return goStep(st+1);
    const opts=[$('#optTips').checked&&'monthly health tips by email',$('#optRem').checked&&'appointment reminders by text'].filter(Boolean);
    loggedIn(v('fname'));
    done('Your account is ready',`<p>Welcome to Riverside, ${v('fname').replace(/</g,'&lt;')}. We have taken the $10 joining fee from the card ending in ${digits(v('cnum')).slice(-4)} and emailed a receipt to ${v('email').replace(/</g,'&lt;')}.</p><p>${opts.length?'You chose to receive '+opts.join(' and ')+'.':'You chose not to receive health tips or reminders. You can turn them on later.'}</p>`);
    ['cnum','cexp','ccvc','pw','pw2'].forEach(id=>$('#'+id).value=''); 
  });


  let fails=0;
  $('#loginForm').addEventListener('submit',e=>{
    e.preventDefault();
    const errs=[];
    if(!emailOk(v('lemail'))) errs.push(['lemail','Enter the email address you registered with']);
    if(!$('#lpw').value) errs.push(['lpw','Enter your password']);
    if(!errs.length && $('#lpw').value.length<10){
      fails++;
      errs.push(['lpw', fails>=3?'For your security, log in is paused for 5 minutes. You can reset your password instead':'The email or password is not right. Check them and try again']);
    }
    if(showErrors('#loginForm','#loginErrors',errs)) return;
    fails=0; loggedIn(v('lemail').split('@')[0]); $('#lpw').value='';
    done('You are logged in', pending?'<p>Your booking is waiting for you to confirm it.</p>':'<p>Find a doctor to book your next visit.</p>');
  });
  $('#forgotBtn').addEventListener('click',e=>{
    const open=$('#forgot').hidden; $('#forgot').hidden=!open; e.currentTarget.setAttribute('aria-expanded',String(open));
    if(open) $('#femail').focus();
  });
  $('#forgotForm').addEventListener('submit',e=>{
    e.preventDefault();
    const errs=[]; if(!emailOk(v('femail'))) errs.push(['femail','Enter your email address']); if(!v('fans')) errs.push(['fans','Answer the security question']);
    $$('#forgotForm .err').forEach(x=>x.textContent=''); $$('#forgotForm .has-error').forEach(x=>x.classList.remove('has-error'));
    errs.forEach(([k,m])=>{ $('#f-'+k).classList.add('has-error'); $('#e-'+k).textContent='Error: '+m; });
    if(errs.length){ $('#'+errs[0][0]).focus(); return; }
    $('#forgotDone').innerHTML='<div class="notice ok" style="margin-top:1.5rem"><p>If the details match an account, we have sent a reset link to that email. The link works for 30 minutes.</p></div>';
  });
  function loggedIn(name){
    user=name;
    const a=$('#navLogin'); a.textContent='Log out'; a.href='#home';
    a.onclick=()=>{ user=null; a.textContent='Log in'; a.href='#login'; a.onclick=null; announce('You have logged out'); };
    announce('Logged in as '+name);
  }

  function done(title,html){ $('#h-done').textContent=title; $('#doneBody').innerHTML=html+(pending&&user&&title!=='Appointment booked'?'<p><a class="btn" href="#book">Go back to your booking</a></p>':''); if(pending&&user) clearErrors('#bookForm','#bookErrors'); navigate('done'); }

  goStep(0,true);
  let start='home'; try{ start=location.hash.slice(1)||'home'; }catch(err){}
  show(start, false);
})();
</script>
</body>
</html>
