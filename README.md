<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SHELDA vida solar — Venta, Instalación y Mantenimiento de Paneles Solares</title>
<meta name="description" content="SHELDA vida solar: 10 años de experiencia en venta, instalación y mantenimiento de sistemas fotovoltaicos. Cotiza gratis por teléfono, correo o WhatsApp.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;400;500;600;700;800&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>
<script>
tailwind.config = {
  theme: {
    extend: {
      colors: {
        ink: '#070B14',
        panel: '#0B1120',
        card: '#0D1424',
        sun: {
          300:'#FFD76A', 400:'#FFC233', 500:'#FFB020', 600:'#F59E0B', 700:'#E8820C'
        }
      },
      fontFamily: {
        display: ['Sora','sans-serif'],
        body: ['Inter','sans-serif']
      }
    }
  }
}
</script>
<style>
html {
  scroll-behavior: smooth;
  scroll-padding-top: 96px;
}
body {
  background: #070B14;
  color: #E7ECF5;
  font-family: 'Inter', sans-serif;
  overflow-x: hidden;
}
::selection { background: #FFB020; color: #070B14; }

/* Scrollbar */
::-webkit-scrollbar { width: 8px; }
::-webkit-scrollbar-track { background: #070B14; }
::-webkit-scrollbar-thumb { background: linear-gradient(#FFB020, #E8820C); border-radius: 8px; border: 2px solid #070B14; }

/* Custom cursor - simplified */
@media (pointer: fine) {
  * { cursor: none !important; }
}
.cursor-dot, .cursor-ring {
  position: fixed;
  top: 0; left: 0;
  pointer-events: none;
  z-index: 10001;
  border-radius: 50%;
  transform: translate(-50%, -50%);
  will-change: transform;
}
.cursor-dot {
  width: 6px; height: 6px;
  background: #FFB020;
}
.cursor-ring {
  width: 36px; height: 36px;
  border: 1.5px solid rgba(255,176,32,.5);
  transition: width .25s ease, height .25s ease, border-color .25s ease, background .25s ease;
}
.cursor-ring.hovered {
  width: 56px; height: 56px;
  border-color: rgba(255,176,32,.85);
  background: rgba(255,176,32,.06);
}
@media (pointer: coarse) {
  .cursor-dot, .cursor-ring { display: none; }
}

/* Gradient text */
.text-grad {
  background: linear-gradient(100deg, #FFE9B0 0%, #FFB020 45%, #FF8A00 100%);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}

/* Glass */
.glass {
  background: rgba(13,20,36,.55);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(255,255,255,.08);
}

/* Nav */
#nav {
  transition: background .3s ease, border-color .3s ease, backdrop-filter .3s ease;
  border-bottom: 1px solid transparent;
}
#nav.nav-scrolled {
  background: rgba(7,11,20,.85);
  backdrop-filter: blur(14px);
  -webkit-backdrop-filter: blur(14px);
  border-bottom: 1px solid rgba(255,255,255,.07);
}
.nav-link { position: relative; }
.nav-link::after {
  content: '';
  position: absolute;
  left: 0; bottom: -6px;
  width: 0; height: 2px;
  background: linear-gradient(90deg, #FFB020, #FF8A00);
  transition: width .3s ease;
  border-radius: 2px;
}
.nav-link:hover::after { width: 100%; }

/* Marquee */
.marquee-track {
  display: flex;
  width: max-content;
  animation: marquee 40s linear infinite;
}
.marquee-track:hover { animation-play-state: paused; }
@keyframes marquee { to { transform: translateX(-50%); } }

/* Rotating ring text */
@keyframes spin-slow { to { transform: rotate(360deg); } }
.animate-spin-slow {
  animation: spin-slow 35s linear infinite;
  transform-origin: center;
  will-change: transform;
}

/* Float - simplified */
@keyframes floaty {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-10px); }
}
.floaty { animation: floaty 7s ease-in-out infinite; will-change: transform; }
.floaty-2 { animation: floaty 8s ease-in-out infinite; animation-delay: 1.5s; will-change: transform; }

/* Preloader */
#preloader {
  position: fixed; inset: 0; z-index: 10000;
  background: #070B14;
  display: flex; flex-direction: column;
  align-items: center; justify-content: center; gap: 24px;
  transition: opacity .5s ease;
}
#preloader.fade-out { opacity: 0; pointer-events: none; }
@keyframes sunPulse {
  0%, 100% { transform: scale(1); filter: drop-shadow(0 0 10px rgba(255,176,32,.6)); }
  50% { transform: scale(1.08); filter: drop-shadow(0 0 24px rgba(255,176,32,.9)); }
}
.loader-sun { animation: sunPulse 1.8s ease-in-out infinite; }
.loader-bar {
  width: 180px; height: 3px;
  background: rgba(255,255,255,.1);
  border-radius: 99px; overflow: hidden;
}
.loader-bar-fill {
  width: 0%; height: 100%;
  background: linear-gradient(90deg, #FFB020, #FF8A00);
  border-radius: 99px;
  transition: width .4s ease;
}

/* Buttons */
.btn-sun {
  position: relative; overflow: hidden;
  background: linear-gradient(100deg, #FFB020, #FF8A00);
  color: #070B14; font-weight: 700;
  transition: transform .25s ease, box-shadow .25s ease;
  box-shadow: 0 8px 28px -8px rgba(255,150,20,.5);
}
.btn-sun:hover {
  transform: translateY(-2px);
  box-shadow: 0 12px 36px -8px rgba(255,150,20,.65);
}
.btn-sun::after {
  content: '';
  position: absolute; top: 0; left: -80%;
  width: 50%; height: 100%;
  background: linear-gradient(100deg, transparent, rgba(255,255,255,.4), transparent);
  transform: skewX(-20deg);
  transition: left .5s ease;
}
.btn-sun:hover::after { left: 130%; }

.btn-ghost {
  border: 1px solid rgba(255,255,255,.18);
  transition: border-color .25s ease, background .25s ease, transform .25s ease;
}
.btn-ghost:hover {
  border-color: rgba(255,176,32,.55);
  background: rgba(255,176,32,.05);
  transform: translateY(-2px);
}

/* Cards */
.service-card {
  position: relative;
  transition: transform .35s cubic-bezier(.2,.8,.2,1), border-color .35s ease;
  overflow: hidden;
}
.service-card::before {
  content: '';
  position: absolute; inset: 0;
  background: radial-gradient(500px circle at var(--mx,50%) var(--my,0%), rgba(255,176,32,.08), transparent 40%);
  opacity: 0;
  transition: opacity .3s ease;
  pointer-events: none;
}
.service-card:hover {
  transform: translateY(-6px);
  border-color: rgba(255,176,32,.4);
}
.service-card:hover::before { opacity: 1; }
.service-card .card-arrow {
  transition: transform .3s ease, background .3s ease, color .3s ease;
}
.service-card:hover .card-arrow {
  transform: translate(3px, -3px);
  background: #FFB020;
  color: #070B14;
}

.project-card img {
  transition: transform .6s cubic-bezier(.2,.8,.2,1), filter .4s ease;
}
.project-card:hover img {
  transform: scale(1.06);
  filter: brightness(1.05);
}
.project-card .proj-overlay {
  background: linear-gradient(to top, rgba(7,11,20,.92) 0%, rgba(7,11,20,.3) 55%, transparent 100%);
}

/* Range slider */
input[type=range] {
  -webkit-appearance: none; appearance: none;
  width: 100%; height: 6px;
  border-radius: 9999px;
  background: rgba(255,255,255,.1);
  outline: none;
}
input[type=range]::-webkit-slider-thumb {
  -webkit-appearance: none;
  width: 22px; height: 22px;
  border-radius: 50%;
  background: #FFB020;
  border: 4px solid #0B1120;
  box-shadow: 0 0 0 3px rgba(255,176,32,.3), 0 0 20px rgba(255,176,32,.6);
  cursor: pointer;
  transition: transform .2s ease;
}
input[type=range]::-webkit-slider-thumb:hover { transform: scale(1.12); }
input[type=range]::-moz-range-thumb {
  width: 22px; height: 22px;
  border-radius: 50%;
  background: #FFB020;
  border: 4px solid #0B1120;
  box-shadow: 0 0 0 3px rgba(255,176,32,.3), 0 0 20px rgba(255,176,32,.6);
  cursor: pointer;
}

/* FAQ */
.faq-item { transition: border-color .25s ease, background .25s ease; }
.faq-item.open { border-color: rgba(255,176,32,.35); background: rgba(255,176,32,.02); }
.faq-answer {
  max-height: 0; overflow: hidden;
  transition: max-height .4s cubic-bezier(.2,.8,.2,1);
}
.faq-item.open .faq-answer { max-height: 320px; }
.faq-icon { transition: transform .3s ease; }
.faq-item.open .faq-icon { transform: rotate(45deg); color: #FFB020; }

/* WhatsApp float */
@keyframes pulseRing {
  0% { transform: scale(1); opacity: .5; }
  100% { transform: scale(1.8); opacity: 0; }
}
.wa-pulse::before {
  content: '';
  position: absolute; inset: 0;
  border-radius: 50%;
  background: #25D366;
  animation: pulseRing 2.5s ease-out infinite;
  z-index: -1;
}
.wa-tooltip {
  opacity: 0; transform: translateX(6px);
  transition: opacity .25s ease, transform .25s ease;
  pointer-events: none;
}
.wa-wrap:hover .wa-tooltip { opacity: 1; transform: translateX(0); }

/* Timeline */
.step-line {
  position: absolute;
  top: 34px; left: calc(50% + 44px);
  width: calc(100% - 88px); height: 2px;
  background: linear-gradient(90deg, rgba(255,176,32,.5), rgba(255,176,32,.06));
}
@media (max-width: 1023px) { .step-line { display: none; } }

/* Toast */
#toast {
  position: fixed; bottom: 100px; left: 50%;
  transform: translate(-50%, 16px);
  opacity: 0;
  transition: opacity .3s ease, transform .3s ease;
  z-index: 10002; pointer-events: none;
}
#toast.show { opacity: 1; transform: translate(-50%, 0); }

/* Progress bar */
#progress {
  position: fixed; top: 0; left: 0;
  height: 3px; width: 0%;
  background: linear-gradient(90deg, #FFB020, #FF8A00);
  z-index: 9999;
  box-shadow: 0 0 10px rgba(255,176,32,.6);
  will-change: width;
}

/* Reveal - using CSS for performance */
.reveal {
  opacity: 0;
  transform: translateY(30px);
  transition: opacity .7s ease, transform .7s ease;
}
.reveal.revealed {
  opacity: 1;
  transform: translateY(0);
}

/* Section label */
.sec-label {
  display: inline-flex;
  align-items: center; gap: 12px;
}
.sec-label::before {
  content: '';
  display: block;
  width: 36px; height: 1px;
  background: linear-gradient(90deg, #FFB020, transparent);
}

/* Glow orbs */
.orb {
  position: absolute;
  border-radius: 50%;
  filter: blur(80px);
  pointer-events: none;
  opacity: .7;
}

/* Big outline text */
.outline-text {
  -webkit-text-stroke: 1px rgba(255,255,255,.06);
  color: transparent;
}

input, textarea, select { outline: none; }
input:focus, textarea:focus, select:focus {
  border-color: rgba(255,176,32,.55) !important;
  box-shadow: 0 0 0 3px rgba(255,176,32,.1);
}

/* Reduce motion preference */
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
  .reveal { opacity: 1; transform: none; }
}
</style>
</head>
<body class="font-body antialiased">

<!-- Cursor -->
<div class="cursor-dot" id="cursorDot"></div>
<div class="cursor-ring" id="cursorRing"></div>

<!-- Scroll progress -->
<div id="progress"></div>

<!-- Toast -->
<div id="toast" class="glass px-5 py-3 rounded-full text-sm font-medium flex items-center gap-2">
  <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
  <span id="toastMsg">Copiado al portapapeles</span>
</div>

<!-- ============ PRELOADER ============ -->
<div id="preloader">
  <svg class="loader-sun" width="56" height="56" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="1.8" stroke-linecap="round">
    <circle cx="12" cy="12" r="4.5" fill="#FFB020" stroke="none"/>
    <line x1="12" y1="1.5" x2="12" y2="4"/><line x1="12" y1="20" x2="12" y2="22.5"/>
    <line x1="1.5" y1="12" x2="4" y2="12"/><line x1="20" y1="12" x2="22.5" y2="12"/>
    <line x1="4.6" y1="4.6" x2="6.4" y2="6.4"/><line x1="17.6" y1="17.6" x2="19.4" y2="19.4"/>
    <line x1="4.6" y1="19.4" x2="6.4" y2="17.6"/><line x1="17.6" y1="6.4" x2="19.4" y2="4.6"/>
  </svg>
  <div class="font-display font-800 tracking-[0.35em] text-lg font-bold">SHELDA</div>
  <div class="text-[11px] tracking-[0.4em] text-white/40 uppercase">vida solar</div>
  <div class="loader-bar"><div class="loader-bar-fill" id="loaderFill"></div></div>
</div>

<!-- ============ NAVBAR ============ -->
<header id="nav" class="fixed top-0 left-0 w-full z-[100]">
  <div class="max-w-7xl mx-auto px-5 md:px-8 h-[84px] flex items-center justify-between">
    <a href="#inicio" class="flex items-center gap-3 group">
      <span class="relative flex items-center justify-center w-11 h-11 rounded-xl bg-gradient-to-br from-sun-400 to-sun-700 shadow-[0_0_22px_rgba(255,176,32,.4)]">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#070B14" stroke-width="2.2" stroke-linecap="round">
          <circle cx="12" cy="12" r="4" fill="#070B14" stroke="none"/>
          <line x1="12" y1="2" x2="12" y2="5"/><line x1="12" y1="19" x2="12" y2="22"/>
          <line x1="2" y1="12" x2="5" y2="12"/><line x1="19" y1="12" x2="22" y2="12"/>
          <line x1="4.9" y1="4.9" x2="7" y2="7"/><line x1="17" y1="17" x2="19.1" y2="19.1"/>
          <line x1="4.9" y1="19.1" x2="7" y2="17"/><line x1="17" y1="7" x2="19.1" y2="4.9"/>
        </svg>
      </span>
      <span class="leading-none">
        <span class="block font-display font-bold text-lg tracking-[0.18em]">SHELDA</span>
        <span class="block text-[10px] tracking-[0.42em] text-sun-500 uppercase">vida solar</span>
      </span>
    </a>

    <nav class="hidden lg:flex items-center gap-9 text-sm font-medium text-white/75">
      <a href="#nosotros" class="nav-link hover:text-white transition-colors">Nosotros</a>
      <a href="#servicios" class="nav-link hover:text-white transition-colors">Servicios</a>
      <a href="#calculadora" class="nav-link hover:text-white transition-colors">Calculadora</a>
      <a href="#proyectos" class="nav-link hover:text-white transition-colors">Proyectos</a>
      <a href="#contacto" class="nav-link hover:text-white transition-colors">Contacto</a>
    </nav>

    <div class="hidden lg:flex items-center gap-4">
      <a href="tel:+525584213690" class="flex items-center gap-2 text-sm text-white/75 hover:text-sun-400 transition-colors">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
        +52 (55) 8421 3690
      </a>
      <a href="https://wa.me/5215584213690?text=Hola%20SHELDA%2C%20quiero%20una%20cotizaci%C3%B3n%20gratuita%20de%20paneles%20solares." target="_blank" rel="noopener" class="btn-sun px-6 py-3 rounded-full text-sm">Cotizar gratis</a>
    </div>

    <!-- Hamburger -->
    <button id="menuBtn" class="lg:hidden w-11 h-11 flex flex-col items-center justify-center gap-[6px] rounded-xl border border-white/15">
      <span class="menu-line block w-5 h-[2px] bg-white transition-all duration-300"></span>
      <span class="menu-line block w-5 h-[2px] bg-white transition-all duration-300"></span>
      <span class="menu-line block w-5 h-[2px] bg-white transition-all duration-300"></span>
    </button>
  </div>
</header>

<!-- Mobile menu -->
<div id="mobileMenu" class="fixed inset-0 z-[99] bg-ink/95 backdrop-blur-xl flex-col items-center justify-center gap-8 hidden">
  <a href="#nosotros" class="mob-link font-display text-3xl font-semibold text-white/85 hover:text-sun-400 transition-colors">Nosotros</a>
  <a href="#servicios" class="mob-link font-display text-3xl font-semibold text-white/85 hover:text-sun-400 transition-colors">Servicios</a>
  <a href="#calculadora" class="mob-link font-display text-3xl font-semibold text-white/85 hover:text-sun-400 transition-colors">Calculadora</a>
  <a href="#proyectos" class="mob-link font-display text-3xl font-semibold text-white/85 hover:text-sun-400 transition-colors">Proyectos</a>
  <a href="#contacto" class="mob-link font-display text-3xl font-semibold text-white/85 hover:text-sun-400 transition-colors">Contacto</a>
  <a href="https://wa.me/5215584213690" target="_blank" rel="noopener" class="mob-link btn-sun px-8 py-4 rounded-full mt-4">Cotizar por WhatsApp</a>
</div>

<!-- ============ HERO ============ -->
<section id="inicio" class="relative min-h-screen flex items-center pt-[110px] pb-16 overflow-hidden">
  <div class="orb w-[450px] h-[450px] bg-sun-600/12 -top-32 -left-32"></div>
  <div class="orb w-[350px] h-[350px] bg-sun-500/08 bottom-0 right-0"></div>

  <!-- faint grid -->
  <div class="absolute inset-0 opacity-[0.04]" style="background-image:linear-gradient(rgba(255,255,255,.5) 1px,transparent 1px),linear-gradient(90deg,rgba(255,255,255,.5) 1px,transparent 1px);background-size:72px 72px;"></div>

  <div class="relative max-w-7xl mx-auto px-5 md:px-8 grid lg:grid-cols-2 gap-14 items-center w-full">
    <!-- Left -->
    <div>
      <div class="hero-anim inline-flex items-center gap-2 glass rounded-full px-4 py-2 text-xs font-medium tracking-wide text-sun-300 mb-7">
        <span class="w-2 h-2 rounded-full bg-sun-500 animate-pulse"></span>
        10 AÑOS LIDERANDO LA ENERGÍA SOLAR
      </div>

      <h1 class="hero-anim font-display font-extrabold text-[42px] leading-[1.05] sm:text-6xl xl:text-[72px] tracking-tight">
        Tu energía,<br>
        <span class="text-grad">el sol.</span>
      </h1>

      <p class="hero-anim mt-7 text-white/60 text-lg max-w-lg leading-relaxed">
        Diseñamos, instalamos y mantenemos sistemas fotovoltaicos de alto rendimiento para hogares y empresas. Reduce tu recibo de luz hasta un <span class="text-sun-400 font-semibold">95%</span> con los expertos del mercado.
      </p>

      <div class="hero-anim mt-9 flex flex-wrap items-center gap-4">
        <a href="#calculadora" class="btn-sun px-8 py-4 rounded-full text-sm flex items-center gap-2">
          Calcula tu ahorro
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><line x1="5" y1="12" x2="19" y2="12"/><polyline points="12 5 19 12 12 19"/></svg>
        </a>
        <a href="https://wa.me/5215584213690?text=Hola%20SHELDA%2C%20quiero%20una%20cotizaci%C3%B3n%20gratuita." target="_blank" rel="noopener" class="btn-ghost px-8 py-4 rounded-full text-sm font-semibold flex items-center gap-2">
          <svg width="17" height="17" viewBox="0 0 24 24" fill="#25D366"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
          WhatsApp directo
        </a>
      </div>

      <div class="hero-anim mt-10 flex flex-wrap items-center gap-x-8 gap-y-3 text-xs text-white/45">
        <span class="flex items-center gap-2"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>Garantía de 25 años</span>
        <span class="flex items-center gap-2"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>Equipos Tier 1</span>
        <span class="flex items-center gap-2"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>Instaladores certificados</span>
      </div>
    </div>

    <!-- Right: Sun visual -->
    <div class="hero-anim relative flex items-center justify-center">
      <div class="relative w-[300px] h-[300px] sm:w-[400px] sm:h-[400px] xl:w-[480px] xl:h-[480px]">
        <canvas id="sun-canvas" class="absolute inset-0"></canvas>

        <!-- rotating ring text -->
        <svg class="absolute animate-spin-slow" style="inset:-40px;" viewBox="0 0 200 200">
          <defs><path id="circlePath" d="M100,100 m-88,0 a88,88 0 1,1 176,0 a88,88 0 1,1 -176,0"/></defs>
          <text fill="rgba(255,255,255,.35)" font-size="8" letter-spacing="3.5" font-family="Sora,sans-serif" font-weight="600">
            <textPath href="#circlePath">ENERGÍA SOLAR • SHELDA VIDA SOLAR • VENTA • INSTALACIÓN • MANTENIMIENTO •</textPath>
          </text>
        </svg>

        <!-- floating cards -->
        <div class="floaty absolute -left-4 sm:-left-12 top-8 glass rounded-2xl px-5 py-4 shadow-2xl">
          <div class="font-display font-bold text-2xl text-sun-400">98%</div>
          <div class="text-[11px] text-white/55 tracking-wide">Clientes satisfechos</div>
        </div>
        <div class="floaty-2 absolute -right-2 sm:-right-8 bottom-10 glass rounded-2xl px-5 py-4 shadow-2xl">
          <div class="font-display font-bold text-2xl text-sun-400">+12 MW</div>
          <div class="text-[11px] text-white/55 tracking-wide">Potencia instalada</div>
        </div>
      </div>
    </div>
  </div>

  <!-- scroll indicator -->
  <div class="absolute bottom-7 left-1/2 -translate-x-1/2 flex flex-col items-center gap-2 text-white/35">
    <span class="text-[10px] tracking-[0.35em] uppercase">Desliza</span>
    <div class="w-[1px] h-10 bg-gradient-to-b from-sun-500 to-transparent"></div>
  </div>
</section>

<!-- ============ MARQUEE ============ -->
<div class="relative border-y border-white/8 bg-panel/60 py-5 overflow-hidden" style="border-color:rgba(255,255,255,.07)">
  <div class="marquee-track items-center">
    <div class="flex items-center gap-10 pr-10" id="marqueeA"></div>
    <div class="flex items-center gap-10 pr-10" id="marqueeB" aria-hidden="true"></div>
  </div>
</div>

<!-- ============ STATS ============ -->
<section class="relative py-20">
  <div class="max-w-7xl mx-auto px-5 md:px-8">
    <div class="grid grid-cols-2 lg:grid-cols-4 gap-6">
      <div class="reveal glass rounded-3xl p-8 text-center">
        <div class="font-display font-extrabold text-5xl text-grad"><span data-count="10">0</span>+</div>
        <div class="mt-2 text-sm text-white/55">Años de experiencia</div>
      </div>
      <div class="reveal glass rounded-3xl p-8 text-center" style="transition-delay:.1s">
        <div class="font-display font-extrabold text-5xl text-grad"><span data-count="850">0</span>+</div>
        <div class="mt-2 text-sm text-white/55">Instalaciones realizadas</div>
      </div>
      <div class="reveal glass rounded-3xl p-8 text-center" style="transition-delay:.2s">
        <div class="font-display font-extrabold text-5xl text-grad"><span data-count="12">0</span> MW</div>
        <div class="mt-2 text-sm text-white/55">Potencia instalada</div>
      </div>
      <div class="reveal glass rounded-3xl p-8 text-center" style="transition-delay:.3s">
        <div class="font-display font-extrabold text-5xl text-grad"><span data-count="98">0</span>%</div>
        <div class="mt-2 text-sm text-white/55">Clientes que nos recomiendan</div>
      </div>
    </div>
  </div>
</section>

<!-- ============ NOSOTROS ============ -->
<section id="nosotros" class="relative py-24 overflow-hidden">
  <div class="orb w-[400px] h-[400px] bg-sun-600/08 top-20 -right-48"></div>

  <div class="max-w-7xl mx-auto px-5 md:px-8 grid lg:grid-cols-2 gap-16 items-center">
    <!-- Images -->
    <div class="reveal relative">
      <div class="rounded-[28px] overflow-hidden border border-white/10 shadow-2xl">
        <img src="https://images.unsplash.com/photo-1509391366360-2e959784a276?q=80&w=1400&auto=format&fit=crop" alt="Planta de paneles solares al atardecer" class="w-full h-[440px] md:h-[520px] object-cover"/>
      </div>
      <div class="absolute -bottom-8 -right-4 md:-right-8 w-48 md:w-60 rounded-2xl overflow-hidden border-4 border-ink shadow-2xl hidden sm:block">
        <img src="https://images.unsplash.com/photo-1592833159155-c62df1b65634?q=80&w=800&auto=format&fit=crop" alt="Técnicos instalando paneles solares" class="w-full h-40 md:h-48 object-cover"/>
      </div>
      <!-- Badge 10 años -->
      <div class="absolute -top-6 -left-4 md:-left-8 w-28 h-28 md:w-32 md:h-32 rounded-full bg-gradient-to-br from-sun-400 to-sun-700 flex flex-col items-center justify-center text-ink shadow-[0_0_35px_rgba(255,176,32,.45)] floaty">
        <span class="font-display font-extrabold text-3xl md:text-4xl leading-none">10</span>
        <span class="text-[10px] font-bold tracking-widest uppercase mt-1">años de</span>
        <span class="text-[10px] font-bold tracking-widest uppercase">experiencia</span>
      </div>
    </div>

    <!-- Text -->
    <div>
      <span class="reveal sec-label text-sun-500 text-xs font-semibold tracking-[0.3em] uppercase">01 — Nosotros</span>
      <h2 class="reveal font-display font-bold text-4xl md:text-5xl mt-5 leading-tight">Una década convirtiendo sol en <span class="text-grad">ahorro real</span></h2>
      <p class="reveal mt-6 text-white/60 leading-relaxed">
        En <strong class="text-white">SHELDA vida solar</strong> no solo instalamos paneles: diseñamos independencia energética. Durante 10 años hemos sido el aliado de cientos de familias y empresas que decidieron tomar el control de su electricidad con sistemas fotovoltaicos de la más alta calidad.
      </p>
      <p class="reveal mt-4 text-white/60 leading-relaxed">
        Nuestro equipo de ingenieros certificados acompaña cada proyecto de principio a fin: desde el estudio de tu consumo hasta el monitoreo post-instalación. Por eso somos los mejores del mercado.
      </p>

      <ul class="reveal mt-8 space-y-4">
        <li class="flex items-start gap-3">
          <span class="mt-0.5 w-6 h-6 rounded-full bg-sun-500/15 border border-sun-500/40 flex items-center justify-center shrink-0"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg></span>
          <span class="text-white/75 text-sm">Ingenieros e instaladores con certificación vigente</span>
        </li>
        <li class="flex items-start gap-3">
          <span class="mt-0.5 w-6 h-6 rounded-full bg-sun-500/15 border border-sun-500/40 flex items-center justify-center shrink-0"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg></span>
          <span class="text-white/75 text-sm">Paneles e inversores Tier 1 con garantía de hasta 25 años</span>
        </li>
        <li class="flex items-start gap-3">
          <span class="mt-0.5 w-6 h-6 rounded-full bg-sun-500/15 border border-sun-500/40 flex items-center justify-center shrink-0"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg></span>
          <span class="text-white/75 text-sm">Trámites e interconexión ante CFE incluidos, sin complicaciones</span>
        </li>
        <li class="flex items-start gap-3">
          <span class="mt-0.5 w-6 h-6 rounded-full bg-sun-500/15 border border-sun-500/40 flex items-center justify-center shrink-0"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg></span>
          <span class="text-white/75 text-sm">Monitoreo, soporte y mantenimiento post-venta de por vida</span>
        </li>
      </ul>

      <a href="#contacto" class="reveal btn-ghost inline-flex items-center gap-2 mt-9 px-7 py-3.5 rounded-full text-sm font-semibold">
        Conoce cómo trabajamos
        <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><line x1="5" y1="12" x2="19" y2="12"/><polyline points="12 5 19 12 12 19"/></svg>
      </a>
    </div>
  </div>
</section>

<!-- ============ SERVICIOS ============ -->
<section id="servicios" class="relative py-24 bg-panel/40">
  <div class="max-w-7xl mx-auto px-5 md:px-8">
    <div class="max-w-2xl">
      <span class="reveal sec-label text-sun-500 text-xs font-semibold tracking-[0.3em] uppercase">02 — Servicios</span>
      <h2 class="reveal font-display font-bold text-4xl md:text-5xl mt-5 leading-tight">Soluciones solares <span class="text-grad">integrales</span></h2>
      <p class="reveal mt-5 text-white/55 leading-relaxed">Del primer rayo de sol al último tornillo: cubrimos todo el ciclo de vida de tu sistema fotovoltaico.</p>
    </div>

    <div class="grid md:grid-cols-3 gap-6 mt-14">
      <!-- Venta -->
      <div class="reveal service-card glass rounded-3xl p-8 border border-white/8">
        <div class="flex items-start justify-between">
          <span class="w-14 h-14 rounded-2xl bg-gradient-to-br from-sun-400/20 to-sun-700/20 border border-sun-500/30 flex items-center justify-center">
            <svg width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="4" width="18" height="14" rx="2"/><line x1="3" y1="9" x2="21" y2="9"/><line x1="3" y1="14" x2="21" y2="14"/><line x1="9" y1="4" x2="9" y2="18"/><line x1="15" y1="4" x2="15" y2="18"/><line x1="8" y1="21" x2="16" y2="21"/></svg>
          </span>
          <span class="card-arrow w-10 h-10 rounded-full border border-white/15 flex items-center justify-center text-white/60">
            <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"/><polyline points="7 7 17 7 17 17"/></svg>
          </span>
        </div>
        <div class="mt-7 text-xs font-bold tracking-[0.25em] text-white/30">01</div>
        <h3 class="font-display font-bold text-2xl mt-2">Venta de Sistemas</h3>
        <p class="mt-3 text-sm text-white/55 leading-relaxed">Equipos fotovoltaicos de última generación con las mejores marcas del mercado mundial, al precio correcto.</p>
        <ul class="mt-6 space-y-2.5 text-sm text-white/65">
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Paneles solares Tier 1 de alta eficiencia</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Inversores y microinversores inteligentes</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Baterías y sistemas de respaldo</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Estructuras y material eléctrico certificado</li>
        </ul>
      </div>

      <!-- Instalación -->
      <div class="reveal service-card glass rounded-3xl p-8 border border-white/8" style="transition-delay:.12s">
        <div class="flex items-start justify-between">
          <span class="w-14 h-14 rounded-2xl bg-gradient-to-br from-sun-400/20 to-sun-700/20 border border-sun-500/30 flex items-center justify-center">
            <svg width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"/></svg>
          </span>
          <span class="card-arrow w-10 h-10 rounded-full border border-white/15 flex items-center justify-center text-white/60">
            <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"/><polyline points="7 7 17 7 17 17"/></svg>
          </span>
        </div>
        <div class="mt-7 text-xs font-bold tracking-[0.25em] text-white/30">02</div>
        <h3 class="font-display font-bold text-2xl mt-2">Instalación Profesional</h3>
        <p class="mt-3 text-sm text-white/55 leading-relaxed">Montaje impecable por técnicos certificados, con ingeniería de precisión y entrega en tiempo récord.</p>
        <ul class="mt-6 space-y-2.5 text-sm text-white/65">
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Diseño e ingeniería a la medida de tu techo</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Instalación certificada en 3 a 5 días</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Trámites e interconexión ante CFE</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Puesta en marcha y capacitación de uso</li>
        </ul>
      </div>

      <!-- Mantenimiento -->
      <div class="reveal service-card glass rounded-3xl p-8 border border-white/8" style="transition-delay:.24s">
        <div class="flex items-start justify-between">
          <span class="w-14 h-14 rounded-2xl bg-gradient-to-br from-sun-400/20 to-sun-700/20 border border-sun-500/30 flex items-center justify-center">
            <svg width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"/></svg>
          </span>
          <span class="card-arrow w-10 h-10 rounded-full border border-white/15 flex items-center justify-center text-white/60">
            <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"/><polyline points="7 7 17 7 17 17"/></svg>
          </span>
        </div>
        <div class="mt-7 text-xs font-bold tracking-[0.25em] text-white/30">03</div>
        <h3 class="font-display font-bold text-2xl mt-2">Mantenimiento</h3>
        <p class="mt-3 text-sm text-white/55 leading-relaxed">Tu sistema siempre al 100%. Planes de mantenimiento preventivo y correctivo con monitoreo continuo.</p>
        <ul class="mt-6 space-y-2.5 text-sm text-white/65">
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Limpieza profesional de módulos</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Monitoreo de producción 24/7</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Termografía e inspección eléctrica</li>
          <li class="flex items-center gap-2.5"><span class="w-1.5 h-1.5 rounded-full bg-sun-500"></span>Planes anuales con atención prioritaria</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- ============ CALCULADORA ============ -->
<section id="calculadora" class="relative py-24 overflow-hidden">
  <div class="orb w-[450px] h-[450px] bg-sun-600/10 -bottom-32 -left-48"></div>

  <div class="max-w-7xl mx-auto px-5 md:px-8">
    <div class="text-center max-w-2xl mx-auto">
      <span class="reveal sec-label text-sun-500 text-xs font-semibold tracking-[0.3em] uppercase justify-center">03 — Calculadora solar</span>
      <h2 class="reveal font-display font-bold text-4xl md:text-5xl mt-5 leading-tight">Descubre cuánto puedes <span class="text-grad">ahorrar</span></h2>
      <p class="reveal mt-5 text-white/55">Mueve el control según tu pago mensual de luz y obtén una estimación instantánea de tu sistema ideal.</p>
    </div>

    <div class="reveal mt-14 glass rounded-[32px] p-8 md:p-12 border border-white/10 grid lg:grid-cols-2 gap-12">
      <!-- Controls -->
      <div>
        <div class="flex items-end justify-between mb-2">
          <label class="text-sm font-medium text-white/70">Tu pago mensual de electricidad</label>
        </div>
        <div class="font-display font-extrabold text-5xl md:text-6xl text-grad mb-8">$<span id="billLabel">3,000</span> <span class="text-lg text-white/40 font-medium">MXN/mes</span></div>

        <input type="range" id="billRange" min="500" max="20000" step="100" value="3000">

        <div class="flex justify-between text-xs text-white/35 mt-3">
          <span>$500</span><span>$20,000</span>
        </div>

        <div class="mt-10 p-5 rounded-2xl border border-sun-500/25" style="background:rgba(255,176,32,.06)">
          <div class="flex gap-3">
            <svg class="shrink-0 mt-0.5" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><line x1="12" y1="16" x2="12" y2="12"/><line x1="12" y1="8" x2="12.01" y2="8"/></svg>
            <p class="text-sm text-white/70 leading-relaxed" id="insightText">Recuperas tu inversión en aproximadamente <strong class="text-sun-400">4.0 años</strong> y disfrutas más de 20 años de energía prácticamente gratis.</p>
          </div>
        </div>
      </div>

      <a id="calcWhatsapp" href="#" target="_blank" rel="noopener" class="btn-sun mt-8 w-full py-4 rounded-full text-sm flex items-center justify-center gap-2">
        <svg width="17" height="17" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
        Quiero esta cotización exacta
      </a>

      <p class="text-[11px] text-white/35 mt-4 text-center">Estimación basada en tarifa promedio. La cotización formal es gratuita y sin compromiso.</p>

      <!-- Results -->
      <div class="grid grid-cols-2 gap-4 content-start">
        <div class="rounded-2xl border border-white/10 bg-white/[0.03] p-6">
          <div class="text-xs text-white/45 mb-2 flex items-center gap-2"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"/></svg>Sistema recomendado</div>
          <div class="font-display font-bold text-3xl"><span id="outKwp">7.3</span> <span class="text-base text-white/40">kWp</span></div>
        </div>
        <div class="rounded-2xl border border-white/10 bg-white/[0.03] p-6">
          <div class="text-xs text-white/45 mb-2 flex items-center gap-2"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="4" width="18" height="14" rx="2"/><line x1="3" y1="11" x2="21" y2="11"/><line x1="12" y1="4" x2="12" y2="18"/></svg>Paneles aprox.</div>
          <div class="font-display font-bold text-3xl"><span id="outPanels">14</span> <span class="text-base text-white/40">módulos</span></div>
        </div>
        <div class="rounded-2xl border border-white/10 bg-white/[0.03] p-6">
          <div class="text-xs text-white/45 mb-2 flex items-center gap-2"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="12" y1="1" x2="12" y2="23"/><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>Ahorro mensual</div>
          <div class="font-display font-bold text-3xl text-sun-400">$<span id="outMonthly">2,850</span></div>
        </div>
        <div class="rounded-2xl border border-white/10 bg-white/[0.03] p-6">
          <div class="text-xs text-white/45 mb-2 flex items-center gap-2"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="23 6 13.5 15.5 8.5 10.5 1 18"/><polyline points="17 6 23 6 23 12"/></svg>Ahorro en 25 años</div>
          <div class="font-display font-bold text-3xl text-sun-400">$<span id="outSave25">855,000</span></div>
        </div>
        <div class="col-span-2 rounded-2xl border border-sun-500/30 p-6" style="background:linear-gradient(120deg,rgba(255,176,32,.1),rgba(255,138,0,.04))">
          <div class="flex flex-wrap items-center justify-between gap-4">
            <div>
              <div class="text-xs text-white/50 mb-1">Retorno de inversión estimado</div>
              <div class="font-display font-extrabold text-4xl text-grad"><span id="outPayback">4.0</span> años</div>
            </div>
            <div class="flex-1 min-w-[180px]">
              <div class="h-2.5 rounded-full bg-white/10 overflow-hidden">
                <div id="paybackBar" class="h-full rounded-full bg-gradient-to-r from-sun-400 to-sun-700 transition-all duration-500" style="width:16%"></div>
              </div>
              <div class="flex justify-between text-[10px] text-white/35 mt-2"><span>Inversión recuperada</span><span>Vida útil: 25+ años</span></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ PROCESO ============ -->
<section id="proceso" class="relative py-24 bg-panel/40">
  <div class="max-w-7xl mx-auto px-5 md:px-8">
    <div class="text-center max-w-2xl mx-auto">
      <span class="reveal sec-label text-sun-500 text-xs font-semibold tracking-[0.3em] uppercase justify-center">04 — Proceso</span>
      <h2 class="reveal font-display font-bold text-4xl md:text-5xl mt-5">Así de simple es <span class="text-grad">cambiarte al sol</span></h2>
    </div>

    <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-10 lg:gap-6 mt-16">
      <div class="reveal relative text-center lg:text-left">
        <div class="step-line"></div>
        <div class="relative z-10 w-[68px] h-[68px] mx-auto lg:mx-0 rounded-2xl bg-gradient-to-br from-sun-400 to-sun-700 flex items-center justify-center font-display font-extrabold text-2xl text-ink shadow-[0_0_25px_rgba(255,176,32,.35)]">1</div>
        <h3 class="font-display font-bold text-xl mt-6">Diagnóstico gratuito</h3>
        <p class="mt-3 text-sm text-white/55 leading-relaxed">Analizamos tu recibo de luz y tus hábitos de consumo. Visita técnica sin costo.</p>
      </div>
      <div class="reveal relative text-center lg:text-left" style="transition-delay:.12s">
        <div class="step-line"></div>
        <div class="relative z-10 w-[68px] h-[68px] mx-auto lg:mx-0 rounded-2xl bg-gradient-to-br from-sun-400 to-sun-700 flex items-center justify-center font-display font-extrabold text-2xl text-ink shadow-[0_0_25px_rgba(255,176,32,.35)]">2</div>
        <h3 class="font-display font-bold text-xl mt-6">Diseño a medida</h3>
        <p class="mt-3 text-sm text-white/55 leading-relaxed">Propuesta técnica y económica personalizada, con proyección exacta de ahorro.</p>
      </div>
      <div class="reveal relative text-center lg:text-left" style="transition-delay:.24s">
        <div class="step-line"></div>
        <div class="relative z-10 w-[68px] h-[68px] mx-auto lg:mx-0 rounded-2xl bg-gradient-to-br from-sun-400 to-sun-700 flex items-center justify-center font-display font-extrabold text-2xl text-ink shadow-[0_0_25px_rgba(255,176,32,.35)]">3</div>
        <h3 class="font-display font-bold text-xl mt-6">Instalación certificada</h3>
        <p class="mt-3 text-sm text-white/55 leading-relaxed">Montaje profesional en 3 a 5 días. Nos encargamos de todos los trámites ante CFE.</p>
      </div>
      <div class="reveal relative text-center lg:text-left" style="transition-delay:.36s">
        <div class="relative z-10 w-[68px] h-[68px] mx-auto lg:mx-0 rounded-2xl bg-gradient-to-br from-sun-400 to-sun-700 flex items-center justify-center font-display font-extrabold text-2xl text-ink shadow-[0_0_25px_rgba(255,176,32,.35)]">4</div>
        <h3 class="font-display font-bold text-xl mt-6">Monitoreo y soporte</h3>
        <p class="mt-3 text-sm text-white/55 leading-relaxed">Supervisamos tu producción y te acompañamos con mantenimiento de por vida.</p>
      </div>
    </div>
  </div>
</section>

<!-- ============ PROYECTOS ============ -->
<section id="proyectos" class="relative py-24">
  <div class="max-w-7xl mx-auto px-5 md:px-8">
    <div class="flex flex-wrap items-end justify-between gap-6">
      <div class="max-w-xl">
        <span class="reveal sec-label text-sun-500 text-xs font-semibold tracking-[0.3em] uppercase">05 — Proyectos</span>
        <h2 class="reveal font-display font-bold text-4xl md:text-5xl mt-5 leading-tight">Energía que ya está <span class="text-grad">funcionando</span></h2>
      </div>
      <p class="reveal text-white/50 text-sm max-w-sm">Más de 850 sistemas instalados en hogares, comercios e industrias en todo el país.</p>
    </div>

    <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-6 mt-14">
      <div class="reveal project-card relative rounded-3xl overflow-hidden border border-white/10 h-80 group">
        <img src="https://images.unsplash.com/photo-1613665813446-82a78c468a1d?q=80&w=1200&auto=format&fit=crop" alt="Casa residencial con paneles solares" class="w-full h-full object-cover"/>
        <div class="proj-overlay absolute inset-0"></div>
        <div class="absolute top-5 left-5"><span class="text-[10px] font-bold tracking-[0.2em] uppercase bg-sun-500 text-ink px-3 py-1.5 rounded-full">Residencial</span></div>
        <div class="absolute bottom-0 left-0 right-0 p-6">
          <h3 class="font-display font-bold text-xl">Casa Lomas</h3>
          <p class="text-sm text-white/60 mt-1">8.2 kWp · CDMX · Ahorro del 96%</p>
        </div>
      </div>
      <div class="reveal project-card relative rounded-3xl overflow-hidden border border-white/10 h-80 group" style="transition-delay:.1s">
        <img src="https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?q=80&w=1200&auto=format&fit=crop" alt="Paneles solares comerciales" class="w-full h-full object-cover"/>
        <div class="proj-overlay absolute inset-0"></div>
        <div class="absolute top-5 left-5"><span class="text-[10px] font-bold tracking-[0.2em] uppercase bg-white text-ink px-3 py-1.5 rounded-full">Comercial</span></div>
        <div class="absolute bottom-0 left-0 right-0 p-6">
          <h3 class="font-display font-bold text-xl">Plaza Norte</h3>
          <p class="text-sm text-white/60 mt-1">120 kWp · Estado de México · 340 paneles</p>
        </div>
      </div>
      <div class="reveal project-card relative rounded-3xl overflow-hidden border border-white/10 h-80 group" style="transition-delay:.2s">
        <img src="https://images.unsplash.com/photo-1466611653911-95081537e5b7?q=80&w=1200&auto=format&fit=crop" alt="Parque de energía renovable" class="w-full h-full object-cover"/>
        <div class="proj-overlay absolute inset-0"></div>
        <div class="absolute top-5 left-5"><span class="text-[10px] font-bold tracking-[0.2em] uppercase bg-ink text-sun-400 border border-sun-500/50 px-3 py-1.5 rounded-full">Industrial</span></div>
        <div class="absolute bottom-0 left-0 right-0 p-6">
          <h3 class="font-display font-bold text-xl">Planta Textil del Valle</h3>
          <p class="text-sm text-white/60 mt-1">350 kWp · Puebla · Retorno en 3.2 años</p>
        </div>
      </div>
      <div class="reveal project-card relative rounded-3xl overflow-hidden border border-white/10 h-80 group">
        <img src="https://images.unsplash.com/photo-1545209463-e2825498edbf?q=80&w=1200&auto=format&fit=crop" alt="Paneles solares contra el cielo" class="w-full h-full object-cover"/>
        <div class="proj-overlay absolute inset-0"></div>
        <div class="absolute top-5 left-5"><span class="text-[10px] font-bold tracking-[0.2em] uppercase bg-sun-500 text-ink px-3 py-1.5 rounded-full">Residencial</span></div>
        <div class="absolute bottom-0 left-0 right-0 p-6">
          <h3 class="font-display font-bold text-xl">Casa del Sol</h3>
          <p class="text-sm text-white/60 mt-1">12.4 kWp · Querétaro · Con baterías de respaldo</p>
        </div>
      </div>
      <div class="reveal project-card relative rounded-3xl overflow-hidden border border-white/10 h-80 group" style="transition-delay:.1s">
        <img src="https://images.unsplash.com/photo-1595437193398-f24279553f4f?q=80&w=1200&auto=format&fit=crop" alt="Detalle de panel solar azul" class="w-full h-full object-cover"/>
        <div class="proj-overlay absolute inset-0"></div>
        <div class="absolute top-5 left-5"><span class="text-[10px] font-bold tracking-[0.2em] uppercase bg-white text-ink px-3 py-1.5 rounded-full">Comercial</span></div>
        <div class="absolute bottom-0 left-0 right-0 p-6">
          <h3 class="font-display font-bold text-xl">Corporativo Andares</h3>
          <p class="text-sm text-white/60 mt-1">85 kWp · Guadalajara · Monitoreo 24/7</p>
        </div>
      </div>
      <div class="reveal project-card relative rounded-3xl overflow-hidden border border-white/10 h-80 group" style="transition-delay:.2s">
        <img src="https://images.unsplash.com/photo-1566093097221-ac2335b09e70?q=80&w=1200&auto=format&fit=crop" alt="Técnico trabajando en instalación solar" class="w-full h-full object-cover"/>
        <div class="proj-overlay absolute inset-0"></div>
        <div class="absolute top-5 left-5"><span class="text-[10px] font-bold tracking-[0.2em] uppercase bg-ink text-sun-400 border border-sun-500/50 px-3 py-1.5 rounded-full">Industrial</span></div>
        <div class="absolute bottom-0 left-0 right-0 p-6">
          <h3 class="font-display font-bold text-xl">Agroindustrias del Campo</h3>
          <p class="text-sm text-white/60 mt-1">210 kWp · Guanajuato · Bombeo solar incluido</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ TESTIMONIOS ============ -->
<section class="relative py-24 bg-panel/40 overflow-hidden">
  <div class="absolute font-display font-extrabold outline-text text-[22vw] leading-none top-4 left-1/2 -translate-x-1/2 select-none pointer-events-none whitespace-nowrap">SHELDA</div>

  <div class="relative max-w-7xl mx-auto px-5 md:px-8">
    <div class="text-center max-w-2xl mx-auto">
      <span class="reveal sec-label text-sun-500 text-xs font-semibold tracking-[0.3em] uppercase justify-center">Testimonios</span>
      <h2 class="reveal font-display font-bold text-4xl md:text-5xl mt-5">Lo que dicen <span class="text-grad">nuestros clientes</span></h2>
    </div>

    <div class="grid md:grid-cols-3 gap-6 mt-14">
      <div class="reveal glass rounded-3xl p-8 border border-white/8 flex flex-col">
        <svg width="32" height="32" viewBox="0 0 24 24" fill="rgba(255,176,32,.3)"><path d="M9.6 5C6 7 4 10 4 13.6 4 16.6 5.9 19 8.8 19c2.3 0 4-1.7 4-4 0-2.2-1.6-3.8-3.7-3.8-.4 0-.8.1-1 .1.4-2 1.9-3.9 3.9-5L9.6 5zm10 0c-3.6 2-5.6 5-5.6 8.6 0 3 1.9 5.4 4.8 5.4 2.3 0 4-1.7 4-4 0-2.2-1.6-3.8-3.7-3.8-.4 0-.8.1-1 .1.4-2 1.9-3.9 3.9-5L19.6 5z"/></svg>
        <div class="flex gap-1 mt-4 mb-4">
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
        </div>
        <p class="text-white/70 text-sm leading-relaxed flex-1">"Mi recibo bajó de $4,200 a $180 pesos al bimestre. La instalación fue impecable y en solo 4 días. El equipo de SHELDA resolvió todas mis dudas, incluso meses después."</p>
        <div class="flex items-center gap-3 mt-6 pt-6 border-t border-white/8">
          <span class="w-11 h-11 rounded-full bg-gradient-to-br from-sun-400 to-sun-700 flex items-center justify-center font-display font-bold text-ink">MR</span>
          <div>
            <div class="font-semibold text-sm">Mariana Robles</div>
            <div class="text-xs text-white/45">Casa habitación · CDMX</div>
          </div>
        </div>
      </div>

      <div class="reveal glass rounded-3xl p-8 border border-white/8 flex flex-col" style="transition-delay:.12s">
        <svg width="32" height="32" viewBox="0 0 24 24" fill="rgba(255,176,32,.3)"><path d="M9.6 5C6 7 4 10 4 13.6 4 16.6 5.9 19 8.8 19c2.3 0 4-1.7 4-4 0-2.2-1.6-3.8-3.7-3.8-.4 0-.8.1-1 .1.4-2 1.9-3.9 3.9-5L9.6 5zm10 0c-3.6 2-5.6 5-5.6 8.6 0 3 1.9 5.4 4.8 5.4 2.3 0 4-1.7 4-4 0-2.2-1.6-3.8-3.7-3.8-.4 0-.8.1-1 .1.4-2 1.9-3.9 3.9-5L19.6 5z"/></svg>
        <div class="flex gap-1 mt-4 mb-4">
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
        </div>
        <p class="text-white/70 text-sm leading-relaxed flex-1">"Instalaron 340 paneles en nuestra plaza comercial sin interrumpir la operación ni un solo día. Profesionalismo de otro nivel. Recuperamos la inversión antes de lo proyectado."</p>
        <div class="flex items-center gap-3 mt-6 pt-6 border-t border-white/8">
          <span class="w-11 h-11 rounded-full bg-gradient-to-br from-sun-400 to-sun-700 flex items-center justify-center font-display font-bold text-ink">JG</span>
          <div>
            <div class="font-semibold text-sm">Jorge Gutiérrez</div>
            <div class="text-xs text-white/45">Director · Plaza Norte</div>
          </div>
        </div>
      </div>

      <div class="reveal glass rounded-3xl p-8 border border-white/8 flex flex-col" style="transition-delay:.24s">
        <svg width="32" height="32" viewBox="0 0 24 24" fill="rgba(255,176,32,.3)"><path d="M9.6 5C6 7 4 10 4 13.6 4 16.6 5.9 19 8.8 19c2.3 0 4-1.7 4-4 0-2.2-1.6-3.8-3.7-3.8-.4 0-.8.1-1 .1.4-2 1.9-3.9 3.9-5L9.6 5zm10 0c-3.6 2-5.6 5-5.6 8.6 0 3 1.9 5.4 4.8 5.4 2.3 0 4-1.7 4-4 0-2.2-1.6-3.8-3.7-3.8-.4 0-.8.1-1 .1.4-2 1.9-3.9 3.9-5L19.6 5z"/></svg>
        <div class="flex gap-1 mt-4 mb-4">
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
          <svg width="15" height="15" viewBox="0 0 24 24" fill="#FFB020"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01z"/></svg>
        </div>
        <p class="text-white/70 text-sm leading-relaxed flex-1">"Contraté el plan de mantenimiento anual y valió cada peso. Detectaron y corrigieron un detalle antes de que afectara la producción. Siempre atentos por WhatsApp."</p>
        <div class="flex items-center gap-3 mt-6 pt-6 border-t border-white/8">
          <span class="w-11 h-11 rounded-full bg-gradient-to-br from-sun-400 to-sun-700 flex items-center justify-center font-display font-bold text-ink">LC</span>
          <div>
            <div class="font-semibold text-sm">Lucía Carranza</div>
            <div class="text-xs text-white/45">Residencial · Querétaro</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ FAQ ============ -->
<section class="relative py-24">
  <div class="max-w-4xl mx-auto px-5 md:px-8">
    <div class="text-center">
      <span class="reveal sec-label text-sun-500 text-xs font-semibold tracking-[0.3em] uppercase justify-center">Preguntas frecuentes</span>
      <h2 class="reveal font-display font-bold text-4xl md:text-5xl mt-5">Resolvemos <span class="text-grad">tus dudas</span></h2>
    </div>

    <div class="mt-12 space-y-4">
      <div class="reveal faq-item glass rounded-2xl border border-white/8">
        <button class="faq-q w-full flex items-center justify-between gap-4 p-6 text-left">
          <span class="font-display font-semibold">¿Cuánto puedo ahorrar con paneles solares?</span>
          <span class="faq-icon shrink-0 w-8 h-8 rounded-full border border-white/15 flex items-center justify-center"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span>
        </button>
        <div class="faq-answer"><p class="px-6 pb-6 text-sm text-white/60 leading-relaxed">La mayoría de nuestros clientes reduce su recibo entre un 90% y 95%. El ahorro exacto depende de tu consumo, la tarifa y el espacio disponible. Con nuestra calculadora puedes obtener una estimación inmediata, y con el diagnóstico gratuito, una cifra exacta.</p></div>
      </div>
      <div class="reveal faq-item glass rounded-2xl border border-white/8" style="transition-delay:.08s">
        <button class="faq-q w-full flex items-center justify-between gap-4 p-6 text-left">
          <span class="font-display font-semibold">¿Qué garantías ofrecen?</span>
          <span class="faq-icon shrink-0 w-8 h-8 rounded-full border border-white/15 flex items-center justify-center"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span>
        </button>
        <div class="faq-answer"><p class="px-6 pb-6 text-sm text-white/60 leading-relaxed">Paneles con garantía de producto de 12 a 15 años y garantía de producción lineal de 25 años; inversores de 5 a 10 años; y nuestra garantía de instalación por escrito de 5 años. Además, soporte post-venta de por vida.</p></div>
      </div>
      <div class="reveal faq-item glass rounded-2xl border border-white/8" style="transition-delay:.16s">
        <button class="faq-q w-full flex items-center justify-between gap-4 p-6 text-left">
          <span class="font-display font-semibold">¿Cuánto tiempo toma la instalación?</span>
          <span class="faq-icon shrink-0 w-8 h-8 rounded-full border border-white/15 flex items-center justify-center"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span>
        </button>
        <div class="faq-answer"><p class="px-6 pb-6 text-sm text-white/60 leading-relaxed">Un sistema residencial típico se instala en 3 a 5 días hábiles. Proyectos comerciales e industriales varían según la potencia. Nosotros gestionamos todo el trámite de interconexión ante CFE para que tú no te preocupes por nada.</p></div>
      </div>
      <div class="reveal faq-item glass rounded-2xl border border-white/8" style="transition-delay:.24s">
        <button class="faq-q w-full flex items-center justify-between gap-4 p-6 text-left">
          <span class="font-display font-semibold">¿Los paneles funcionan en días nublados?</span>
          <span class="faq-icon shrink-0 w-8 h-8 rounded-full border border-white/15 flex items-center justify-center"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span>
        </button>
        <div class="faq-answer"><p class="px-6 pb-6 text-sm text-white/60 leading-relaxed">Sí. Los paneles generan energía con luz difusa, aunque a menor capacidad (10–25%). El sistema está dimensionado considerando el clima de tu región durante todo el año, por lo que tu ahorro anual está garantizado.</p></div>
      </div>
      <div class="reveal faq-item glass rounded-2xl border border-white/8" style="transition-delay:.32s">
        <button class="faq-q w-full flex items-center justify-between gap-4 p-6 text-left">
          <span class="font-display font-semibold">¿Qué mantenimiento necesitan los paneles?</span>
          <span class="faq-icon shrink-0 w-8 h-8 rounded-full border border-white/15 flex items-center justify-center"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span>
        </button>
        <div class="faq-answer"><p class="px-6 pb-6 text-sm text-white/60 leading-relaxed">Muy poco: limpieza de módulos 2 a 4 veces al año y una revisión eléctrica anual. Nuestros planes de mantenimiento incluyen limpieza profesional, termografía, torqueo de conexiones y monitoreo continuo de producción.</p></div>
      </div>
      <div class="reveal faq-item glass rounded-2xl border border-white/8" style="transition-delay:.4s">
        <button class="faq-q w-full flex items-center justify-between gap-4 p-6 text-left">
          <span class="font-display font-semibold">¿Qué pasa con la energía que no uso?</span>
          <span class="faq-icon shrink-0 w-8 h-8 rounded-full border border-white/15 flex items-center justify-center"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg></span>
        </button>
        <div class="faq-answer"><p class="px-6 pb-6 text-sm text-white/60 leading-relaxed">Con la interconexión a la red de CFE (medición neta), los excedentes que generas se inyectan a la red y se acreditan a tu favor, reduciendo aún más tu recibo. También ofrecemos sistemas con baterías para máxima independencia.</p></div>
      </div>
    </div>
  </div>
</section>

<!-- ============ CTA BANNER ============ -->
<section class="relative py-20">
  <div class="max-w-7xl mx-auto px-5 md:px-8">
    <div class="reveal relative rounded-[32px] overflow-hidden border border-sun-500/25">
      <img src="https://images.unsplash.com/photo-1509391366360-2e959784a276?q=80&w=1800&auto=format&fit=crop" alt="Campo de paneles solares" class="absolute inset-0 w-full h-full object-cover"/>
      <div class="absolute inset-0" style="background:linear-gradient(100deg, rgba(7,11,20,.96) 20%, rgba(7,11,20,.75) 60%, rgba(232,130,12,.3) 100%)"></div>
      <div class="relative p-10 md:p-16 lg:p-20 max-w-2xl">
        <h2 class="font-display font-extrabold text-4xl md:text-5xl leading-tight">¿Listo para generar tu <span class="text-grad">propia energía?</span></h2>
        <p class="mt-5 text-white/65 leading-relaxed">Agenda hoy tu diagnóstico gratuito. Un asesor experto te contactará en menos de 24 horas con una propuesta a la medida.</p>
        <div class="mt-8 flex flex-wrap gap-4">
          <a href="https://wa.me/5215584213690?text=Hola%20SHELDA%2C%20quiero%20agendar%20mi%20diagn%C3%B3stico%20gratuito." target="_blank" rel="noopener" class="btn-sun px-8 py-4 rounded-full text-sm flex items-center gap-2">
            Agendar diagnóstico gratis
            <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><line x1="5" y1="12" x2="19" y2="12"/><polyline points="12 5 19 12 12 19"/></svg>
          </a>
          <a href="tel:+525584213690" class="btn-ghost px-8 py-4 rounded-full text-sm font-semibold flex items-center gap-2">
            <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
            Llamar ahora
          </a>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ CONTACTO ============ -->
<section id="contacto" class="relative py-24 bg-panel/40 overflow-hidden">
  <div class="orb w-[400px] h-[400px] bg-sun-600/08 top-10 -right-48"></div>

  <div class="max-w-7xl mx-auto px-5 md:px-8">
    <div class="text-center max-w-2xl mx-auto">
      <span class="reveal sec-label text-sun-500 text-xs font-semibold tracking-[0.3em] uppercase justify-center">06 — Contacto</span>
      <h2 class="reveal font-display font-bold text-4xl md:text-5xl mt-5">Hablemos de <span class="text-grad">tu proyecto</span></h2>
      <p class="reveal mt-5 text-white/55">Elige el canal que prefieras. Respondemos rápido, siempre con un asesor humano y experto.</p>
    </div>

    <!-- Contact channels -->
    <div class="grid md:grid-cols-3 gap-6 mt-14">
      <!-- Phone -->
      <div class="reveal service-card glass rounded-3xl p-8 border border-white/8 text-center">
        <span class="mx-auto w-16 h-16 rounded-2xl bg-gradient-to-br from-sun-400/20 to-sun-700/20 border border-sun-500/30 flex items-center justify-center">
          <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
        </span>
        <h3 class="font-display font-bold text-xl mt-5">Teléfono</h3>
        <p class="text-sm text-white/50 mt-2">Lun–Vie 9:00–18:00 · Sáb 9:00–14:00</p>
        <a href="tel:+525584213690" class="block mt-4 font-display font-semibold text-lg text-sun-400 hover:text-sun-300 transition-colors">+52 (55) 8421 3690</a>
        <button data-copy="+525584213690" class="mt-4 text-xs text-white/45 hover:text-sun-400 transition-colors inline-flex items-center gap-1.5 border border-white/12 rounded-full px-4 py-2">
          <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="9" width="13" height="13" rx="2"/><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"/></svg>
          Copiar número
        </button>
      </div>

      <!-- Email -->
      <div class="reveal service-card glass rounded-3xl p-8 border border-white/8 text-center" style="transition-delay:.12s">
        <span class="mx-auto w-16 h-16 rounded-2xl bg-gradient-to-br from-sun-400/20 to-sun-700/20 border border-sun-500/30 flex items-center justify-center">
          <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
        </span>
        <h3 class="font-display font-bold text-xl mt-5">Correo</h3>
        <p class="text-sm text-white/50 mt-2">Respondemos en menos de 24 horas</p>
        <a href="mailto:contacto@shelda.mx?subject=Cotizaci%C3%B3n%20de%20paneles%20solares" class="block mt-4 font-display font-semibold text-lg text-sun-400 hover:text-sun-300 transition-colors">contacto@shelda.mx</a>
        <button data-copy="contacto@shelda.mx" class="mt-4 text-xs text-white/45 hover:text-sun-400 transition-colors inline-flex items-center gap-1.5 border border-white/12 rounded-full px-4 py-2">
          <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="9" width="13" height="13" rx="2"/><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"/></svg>
          Copiar correo
        </button>
      </div>

      <!-- WhatsApp -->
      <div class="reveal service-card glass rounded-3xl p-8 border border-white/8 text-center" style="transition-delay:.24s">
        <span class="mx-auto w-16 h-16 rounded-2xl flex items-center justify-center" style="background:rgba(37,211,102,.1);border:1px solid rgba(37,211,102,.3)">
          <svg width="28" height="28" viewBox="0 0 24 24" fill="#25D366"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
        </span>
        <h3 class="font-display font-bold text-xl mt-5">WhatsApp</h3>
        <p class="text-sm text-white/50 mt-2">Atención inmediata en horario laboral</p>
        <a href="https://wa.me/5215584213690" target="_blank" rel="noopener" class="block mt-4 font-display font-semibold text-lg hover:opacity-80 transition-opacity" style="color:#25D366">+52 1 55 8421 3690</a>
        <a href="https://wa.me/5215584213690?text=Hola%20SHELDA%2C%20quiero%20informaci%C3%B3n%20sobre%20paneles%20solares." target="_blank" rel="noopener" class="mt-4 text-xs inline-flex items-center gap-1.5 rounded-full px-4 py-2 font-semibold text-ink transition-transform hover:scale-105" style="background:#25D366">
          <svg width="12" height="12" viewBox="0 0 24 24" fill="currentColor"><path d="M21 11.5a8.38 8.38 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.38 8.38 0 0 1-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.38 8.38 0 0 1 3.8-.9h.5a8.48 8.48 0 0 1 8 8v.5z"/></svg>
          Abrir chat
        </a>
      </div>
    </div>

    <!-- Form + info -->
    <div class="grid lg:grid-cols-5 gap-8 mt-10">
      <!-- Form -->
      <div class="reveal lg:col-span-3 glass rounded-[28px] p-8 md:p-10 border border-white/10">
        <h3 class="font-display font-bold text-2xl">Solicita tu cotización gratuita</h3>
        <p class="text-sm text-white/50 mt-2">Completa el formulario y te contactaremos por WhatsApp con tu propuesta.</p>

        <form id="quoteForm" class="mt-8 grid sm:grid-cols-2 gap-5">
          <div>
            <label class="text-xs font-medium text-white/60 block mb-2">Nombre completo *</label>
            <input required id="fName" type="text" placeholder="Ej. Ana Martínez" class="w-full bg-white/[0.04] border border-white/12 rounded-xl px-4 py-3.5 text-sm placeholder:text-white/25 transition-all"/>
          </div>
          <div>
            <label class="text-xs font-medium text-white/60 block mb-2">Teléfono / WhatsApp *</label>
            <input required id="fPhone" type="tel" placeholder="Ej. 55 1234 5678" class="w-full bg-white/[0.04] border border-white/12 rounded-xl px-4 py-3.5 text-sm placeholder:text-white/25 transition-all"/>
          </div>
          <div>
            <label class="text-xs font-medium text-white/60 block mb-2">Correo electrónico</label>
            <input id="fEmail" type="email" placeholder="tucorreo@ejemplo.com" class="w-full bg-white/[0.04] border border-white/12 rounded-xl px-4 py-3.5 text-sm placeholder:text-white/25 transition-all"/>
          </div>
          <div>
            <label class="text-xs font-medium text-white/60 block mb-2">Servicio de interés *</label>
            <select required id="fService" class="w-full bg-white/[0.04] border border-white/12 rounded-xl px-4 py-3.5 text-sm text-white/80 transition-all" style="appearance:none;">
              <option value="" class="bg-panel">Selecciona una opción</option>
              <option value="Venta de sistema fotovoltaico" class="bg-panel">Venta de sistema fotovoltaico</option>
              <option value="Instalación de paneles solares" class="bg-panel">Instalación de paneles solares</option>
              <option value="Mantenimiento de sistema existente" class="bg-panel">Mantenimiento de sistema existente</option>
              <option value="Proyecto comercial o industrial" class="bg-panel">Proyecto comercial o industrial</option>
            </select>
          </div>
          <div class="sm:col-span-2">
            <label class="text-xs font-medium text-white/60 block mb-2">Cuéntanos sobre tu proyecto</label>
            <textarea id="fMsg" rows="4" placeholder="Ej. Pago $3,500 de luz al mes y tengo un techo de aproximadamente 60 m²..." class="w-full bg-white/[0.04] border border-white/12 rounded-xl px-4 py-3.5 text-sm placeholder:text-white/25 transition-all resize-none"></textarea>
          </div>
          <div class="sm:col-span-2">
            <button type="submit" class="btn-sun w-full py-4 rounded-full text-sm flex items-center justify-center gap-2">
              Enviar y continuar por WhatsApp
              <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
            </button>
            <p class="text-[11px] text-white/35 mt-3 text-center">Al enviar, se abrirá WhatsApp con tu mensaje listo. Sin spam, sin compromiso.</p>
          </div>
        </form>
      </div>

      <!-- Info side -->
      <div class="lg:col-span-2 space-y-6">
        <div class="reveal glass rounded-[28px] p-8 border border-white/10">
          <h4 class="font-display font-bold text-lg flex items-center gap-2">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>
            Oficinas centrales
          </h4>
          <p class="text-sm text-white/55 mt-3 leading-relaxed">Av. Insurgentes Sur 1425, Piso 8<br>Col. Insurgentes Mixcoac, CDMX, 03920</p>
          <p class="text-sm text-white/55 mt-3">Cobertura de instalación en <strong class="text-sun-400">toda la República Mexicana</strong>.</p>
        </div>

        <div class="reveal glass rounded-[28px] p-8 border border-white/10" style="transition-delay:.1s">
          <h4 class="font-display font-bold text-lg flex items-center gap-2">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
            Horario de atención
          </h4>
          <div class="mt-3 space-y-2 text-sm">
            <div class="flex justify-between text-white/55"><span>Lunes a Viernes</span><span class="text-white/80">9:00 – 18:00</span></div>
            <div class="flex justify-between text-white/55"><span>Sábados</span><span class="text-white/80">9:00 – 14:00</span></div>
            <div class="flex justify-between text-white/55"><span>Emergencias 24/7</span><span class="text-sun-400">Clientes con plan</span></div>
          </div>
        </div>

        <div class="reveal rounded-[28px] p-8 border border-sun-500/30" style="background:linear-gradient(135deg,rgba(255,176,32,.1),rgba(255,138,0,.03));transition-delay:.2s">
          <div class="flex items-center gap-3">
            <svg width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/><polyline points="9 12 11 14 15 10"/></svg>
            <h4 class="font-display font-bold text-lg">Compra protegida</h4>
          </div>
          <p class="text-sm text-white/60 mt-3 leading-relaxed">Contrato por escrito, póliza de responsabilidad civil y garantías respaldadas por fabricante. Tu inversión está segura con nosotros.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ FOOTER ============ -->
<footer class="relative border-t border-white/8 pt-16 pb-8" style="border-color:rgba(255,255,255,.07)">
  <div class="max-w-7xl mx-auto px-5 md:px-8">
    <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-10">
      <div>
        <a href="#inicio" class="flex items-center gap-3">
          <span class="flex items-center justify-center w-10 h-10 rounded-xl bg-gradient-to-br from-sun-400 to-sun-700">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#070B14" stroke-width="2.2" stroke-linecap="round"><circle cx="12" cy="12" r="4" fill="#070B14" stroke="none"/><line x1="12" y1="2" x2="12" y2="5"/><line x1="12" y1="19" x2="12" y2="22"/><line x1="2" y1="12" x2="5" y2="12"/><line x1="19" y1="12" x2="22" y2="12"/><line x1="4.9" y1="4.9" x2="7" y2="7"/><line x1="17" y1="17" x2="19.1" y2="19.1"/><line x1="4.9" y1="19.1" x2="7" y2="17"/><line x1="17" y1="7" x2="19.1" y2="4.9"/></svg>
          </span>
          <span class="leading-none">
            <span class="block font-display font-bold tracking-[0.18em]">SHELDA</span>
            <span class="block text-[9px] tracking-[0.42em] text-sun-500 uppercase">vida solar</span>
          </span>
        </a>
        <p class="text-sm text-white/45 mt-5 leading-relaxed">10 años transformando la energía del sol en ahorro, independencia y futuro para hogares y empresas mexicanas.</p>
      </div>

      <div>
        <h5 class="font-display font-semibold text-sm tracking-widest uppercase text-white/70 mb-5">Navegación</h5>
        <ul class="space-y-3 text-sm text-white/45">
          <li><a href="#nosotros" class="hover:text-sun-400 transition-colors">Nosotros</a></li>
          <li><a href="#servicios" class="hover:text-sun-400 transition-colors">Servicios</a></li>
          <li><a href="#calculadora" class="hover:text-sun-400 transition-colors">Calculadora solar</a></li>
          <li><a href="#proyectos" class="hover:text-sun-400 transition-colors">Proyectos</a></li>
          <li><a href="#contacto" class="hover:text-sun-400 transition-colors">Contacto</a></li>
        </ul>
      </div>

      <div>
        <h5 class="font-display font-semibold text-sm tracking-widest uppercase text-white/70 mb-5">Servicios</h5>
        <ul class="space-y-3 text-sm text-white/45">
          <li><a href="#servicios" class="hover:text-sun-400 transition-colors">Venta de sistemas fotovoltaicos</a></li>
          <li><a href="#servicios" class="hover:text-sun-400 transition-colors">Instalación profesional</a></li>
          <li><a href="#servicios" class="hover:text-sun-400 transition-colors">Mantenimiento y monitoreo</a></li>
          <li><a href="#servicios" class="hover:text-sun-400 transition-colors">Proyectos industriales</a></li>
        </ul>
      </div>

      <div>
        <h5 class="font-display font-semibold text-sm tracking-widest uppercase text-white/70 mb-5">Contacto</h5>
        <ul class="space-y-3 text-sm text-white/45">
          <li><a href="tel:+525584213690" class="hover:text-sun-400 transition-colors">+52 (55) 8421 3690</a></li>
          <li><a href="mailto:contacto@shelda.mx" class="hover:text-sun-400 transition-colors">contacto@shelda.mx</a></li>
          <li><a href="https://wa.me/5215584213690" target="_blank" rel="noopener" class="hover:text-sun-400 transition-colors">WhatsApp directo</a></li>
          <li class="text-white/35">CDMX · Cobertura nacional</li>
        </ul>
      </div>
    </div>

    <div class="mt-14 pt-7 border-t flex flex-col md:flex-row items-center justify-between gap-4 text-xs text-white/35" style="border-color:rgba(255,255,255,.07)">
      <span>© <span id="year">2025</span> SHELDA vida solar. Todos los derechos reservados.</span>
      <span class="flex items-center gap-2">
        <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round"><circle cx="12" cy="12" r="4" fill="#FFB020" stroke="none"/><line x1="12" y1="2" x2="12" y2="5"/><line x1="12" y1="19" x2="12" y2="22"/><line x1="2" y1="12" x2="5" y2="12"/><line x1="19" y1="12" x2="22" y2="12"/><line x1="4.9" y1="4.9" x2="7" y2="7"/><line x1="17" y1="17" x2="19.1" y2="19.1"/><line x1="4.9" y1="19.1" x2="7" y2="17"/><line x1="17" y1="7" x2="19.1" y2="4.9"/></svg>
        Energía limpia, hecha por expertos.
      </span>
    </div>
  </div>
</footer>

<!-- ============ WHATSAPP FLOAT ============ -->
<div class="wa-wrap fixed bottom-6 right-6 z-[100] flex items-center gap-3">
  <span class="wa-tooltip glass px-4 py-2.5 rounded-full text-xs font-medium whitespace-nowrap">¿Dudas? Escríbenos ahora</span>
  <a href="https://wa.me/5215584213690?text=Hola%20SHELDA%2C%20quiero%20informaci%C3%B3n%20sobre%20paneles%20solares." target="_blank" rel="noopener" aria-label="Contactar por WhatsApp" class="wa-pulse relative w-16 h-16 rounded-full flex items-center justify-center shadow-2xl transition-transform hover:scale-110" style="background:#25D366; box-shadow:0 10px 30px -5px rgba(37,211,102,.45)">
    <svg width="28" height="28" viewBox="0 0 24 24" fill="#fff"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
  </a>
</div>

<!-- ============ SCRIPTS ============ -->
<script>
/* ============ MARQUEE BUILD ============ */
(function(){
  const items = ['VENTA DE SISTEMAS','INSTALACIÓN PROFESIONAL','MANTENIMIENTO ESPECIALIZADO','MONITOREO 24/7','GARANTÍA 25 AÑOS','10 AÑOS DE EXPERIENCIA'];
  const sun = '<svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#FFB020" stroke-width="2" stroke-linecap="round"><circle cx="12" cy="12" r="4" fill="#FFB020" stroke="none"/><line x1="12" y1="2" x2="12" y2="5"/><line x1="12" y1="19" x2="12" y2="22"/><line x1="2" y1="12" x2="5" y2="12"/><line x1="19" y1="12" x2="22" y2="12"/></svg>';
  const html = items.map(t => '<span class="flex items-center gap-10"><span class="font-display font-semibold text-lg tracking-[0.15em] text-white/70 whitespace-nowrap">'+t+'</span>'+sun+'</span>').join('');
  document.getElementById('marqueeA').innerHTML = html;
  document.getElementById('marqueeB').innerHTML = html;
})();

/* ============ PRELOADER ============ */
(function(){
  const preloader = document.getElementById('preloader');
  const fill = document.getElementById('loaderFill');
  let done = false;

  function finish(){
    if(done) return;
    done = true;
    fill.style.width = '100%';
    setTimeout(() => {
      preloader.classList.add('fade-out');
      setTimeout(() => { preloader.style.display = 'none'; }, 500);
      // Animate hero elements
      document.querySelectorAll('.hero-anim').forEach((el, i) => {
        setTimeout(() => {
          el.style.opacity = '1';
          el.style.transform = 'translateY(0)';
        }, 100 + i * 120);
      });
    }, 600);
  }

  // Set initial state for hero anims
  document.querySelectorAll('.hero-anim').forEach(el => {
    el.style.opacity = '0';
    el.style.transform = 'translateY(30px)';
    el.style.transition = 'opacity .6s ease, transform .6s ease';
  });

  window.addEventListener('load', finish);
  setTimeout(finish, 3200);
})();

/* ============ CUSTOM CURSOR ============ */
(function(){
  if(!window.matchMedia('(pointer:fine)').matches) return;
  const dot = document.getElementById('cursorDot');
  const ring = document.getElementById('cursorRing');
  let mx = innerWidth/2, my = innerHeight/2;
  let rx = mx, ry = my;

  window.addEventListener('mousemove', e => {
    mx = e.clientX; my = e.clientY;
    dot.style.left = mx + 'px';
    dot.style.top = my + 'px';
  }, {passive: true});

  function loop(){
    rx += (mx - rx) * 0.14;
    ry += (my - ry) * 0.14;
    ring.style.left = rx + 'px';
    ring.style.top = ry + 'px';
    requestAnimationFrame(loop);
  }
  loop();

  document.querySelectorAll('a, button, input, textarea, select, .faq-q').forEach(el => {
    el.addEventListener('mouseenter', () => ring.classList.add('hovered'));
    el.addEventListener('mouseleave', () => ring.classList.remove('hovered'));
  });
})();

/* ============ SUN CANVAS - Optimized ============ */
(function(){
  const canvas = document.getElementById('sun-canvas');
  if(!canvas) return;
  const ctx = canvas.getContext('2d');
  const DPR = Math.min(window.devicePixelRatio || 1, 1.5); // Lower DPR for performance
  let w, h, cx, cy, R;
  let isVisible = true;

  function resize(){
    const rect = canvas.parentElement.getBoundingClientRect();
    w = rect.width; h = rect.height;
    canvas.width = w * DPR;
    canvas.height = h * DPR;
    canvas.style.width = w + 'px';
    canvas.style.height = h + 'px';
    ctx.setTransform(DPR, 0, 0, DPR, 0, 0);
    cx = w / 2; cy = h / 2;
    R = Math.min(w, h) * 0.16;
  }
  resize();
  window.addEventListener('resize', resize);

  // Fewer particles for performance
  const particles = [];
  const PARTICLE_COUNT = 30;

  function resetP(p, init){
    p.a = Math.random() * Math.PI * 2;
    p.d = init ? R * (1.1 + Math.random() * 2.2) : R * 1.1;
    p.maxD = R * (2.2 + Math.random() * 1.4);
    p.r = 1 + Math.random() * 1.8;
    p.sp = 0.2 + Math.random() * 0.45;
  }

  for(let i = 0; i < PARTICLE_COUNT; i++){
    const p = {};
    resetP(p, true);
    particles.push(p);
  }

  let mX = 0, mY = 0;
  window.addEventListener('mousemove', e => {
    mX = (e.clientX / window.innerWidth - 0.5);
    mY = (e.clientY / window.innerHeight - 0.5);
  }, {passive: true});

  // Fewer rays
  const RAYS = 24;
  let lastTime = 0;
  const targetFPS = 60;
  const frameInterval = 1000 / targetFPS;

  // Visibility observer to pause when off-screen
  const observer = new IntersectionObserver(entries => {
    isVisible = entries[0].isIntersecting;
  }, {threshold: 0.1});
  observer.observe(canvas);

  function draw(timestamp){
    requestAnimationFrame(draw);
    if(!isVisible) return;

    // Throttle frame rate
    if(timestamp - lastTime < frameInterval) return;
    lastTime = timestamp;

    ctx.clearRect(0, 0, w, h);
    const px = cx + mX * 18;
    const py = cy + mY * 18;
    const pulse = 1 + Math.sin(timestamp * 0.001) * 0.025;
    const r = R * pulse;

    // Outer glow
    const g = ctx.createRadialGradient(px, py, 0, px, py, r * 4);
    g.addColorStop(0, 'rgba(255,176,32,0.25)');
    g.addColorStop(0.4, 'rgba(255,138,0,0.08)');
    g.addColorStop(1, 'rgba(255,138,0,0)');
    ctx.fillStyle = g;
    ctx.fillRect(0, 0, w, h);

    // Rays
    ctx.save();
    ctx.translate(px, py);
    ctx.rotate(timestamp * 0.00005);
    for(let i = 0; i < RAYS; i++){
      const ang = (i / RAYS) * Math.PI * 2;
      const len = r * (0.45 + 0.3 * Math.sin(timestamp * 0.0008 + i * 1.5));
      const x1 = Math.cos(ang) * r * 1.15;
      const y1 = Math.sin(ang) * r * 1.15;
      const x2 = Math.cos(ang) * (r * 1.15 + len);
      const y2 = Math.sin(ang) * (r * 1.15 + len);
      const lg = ctx.createLinearGradient(x1, y1, x2, y2);
      lg.addColorStop(0, 'rgba(255,200,80,0.45)');
      lg.addColorStop(1, 'rgba(255,200,80,0)');
      ctx.strokeStyle = lg;
      ctx.lineWidth = 1.4;
      ctx.beginPath();
      ctx.moveTo(x1, y1);
      ctx.lineTo(x2, y2);
      ctx.stroke();
    }
    ctx.restore();

    // Core
    const core = ctx.createRadialGradient(px - r * 0.3, py - r * 0.3, r * 0.1, px, py, r);
    core.addColorStop(0, '#FFF4D8');
    core.addColorStop(0.45, '#FFD76A');
    core.addColorStop(1, '#FF9A1F');
    ctx.beginPath();
    ctx.arc(px, py, r, 0, Math.PI * 2);
    ctx.fillStyle = core;
    ctx.shadowColor = 'rgba(255,170,40,0.7)';
    ctx.shadowBlur = 45;
    ctx.fill();
    ctx.shadowBlur = 0;

    // Particles
    for(let i = 0; i < particles.length; i++){
      const p = particles[i];
      p.d += p.sp;
      if(p.d > p.maxD) resetP(p, false);
      const x = px + Math.cos(p.a) * p.d;
      const y = py + Math.sin(p.a) * p.d;
      const fade = Math.max(0, 1 - (p.d - R * 1.1) / (p.maxD - R * 1.1));
      ctx.beginPath();
      ctx.arc(x, y, p.r, 0, Math.PI * 2);
      ctx.fillStyle = 'rgba(255,200,90,' + (0.5 * fade).toFixed(3) + ')';
      ctx.fill();
    }
  }
  requestAnimationFrame(draw);
})();

/* ============ NAV SCROLL + PROGRESS ============ */
(function(){
  const nav = document.getElementById('nav');
  const prog = document.getElementById('progress');
  let ticking = false;

  window.addEventListener('scroll', () => {
    if(!ticking){
      requestAnimationFrame(() => {
        if(window.scrollY > 40) nav.classList.add('nav-scrolled');
        else nav.classList.remove('nav-scrolled');
        const max = document.documentElement.scrollHeight - window.innerHeight;
        prog.style.width = (max > 0 ? (window.scrollY / max) * 100 : 0) + '%';
        ticking = false;
      });
      ticking = true;
    }
  }, {passive: true});
})();

/* ============ MOBILE MENU ============ */
(function(){
  const btn = document.getElementById('menuBtn');
  const menu = document.getElementById('mobileMenu');
  const lines = btn.querySelectorAll('.menu-line');
  let open = false;

  function toggle(force){
    open = (typeof force === 'boolean') ? force : !open;
    menu.classList.toggle('hidden', !open);
    menu.classList.toggle('flex', open);
    document.body.style.overflow = open ? 'hidden' : '';
    lines[0].style.transform = open ? 'translateY(8px) rotate(45deg)' : '';
    lines[1].style.opacity = open ? '0' : '1';
    lines[2].style.transform = open ? 'translateY(-8px) rotate(-45deg)' : '';
  }

  btn.addEventListener('click', () => toggle());
  menu.querySelectorAll('.mob-link').forEach(a => a.addEventListener('click', () => toggle(false)));
})();

/* ============ SCROLL REVEALS - Using IntersectionObserver ============ */
(function(){
  const reveals = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if(entry.isIntersecting){
        entry.target.classList.add('revealed');
        observer.unobserve(entry.target);
      }
    });
  }, {
    threshold: 0.12,
    rootMargin: '0px 0px -40px 0px'
  });

  reveals.forEach(el => observer.observe(el));
})();

/* ============ COUNTERS ============ */
(function(){
  const counters = document.querySelectorAll('[data-count]');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if(entry.isIntersecting){
        const el = entry.target;
        const target = parseFloat(el.dataset.count);
        let current = 0;
        const duration = 1800;
        const startTime = performance.now();

        function update(now){
          const elapsed = now - startTime;
          const progress = Math.min(elapsed / duration, 1);
          // Ease out cubic
          const eased = 1 - Math.pow(1 - progress, 3);
          current = Math.round(eased * target);
          el.textContent = current.toLocaleString('es-MX');
          if(progress < 1) requestAnimationFrame(update);
        }
        requestAnimationFrame(update);
        observer.unobserve(el);
      }
    });
  }, {threshold: 0.5});

  counters.forEach(el => observer.observe(el));
})();

/* ============ SERVICE CARD SPOTLIGHT ============ */
(function(){
  document.querySelectorAll('.service-card').forEach(card => {
    card.addEventListener('mousemove', e => {
      const r = card.getBoundingClientRect();
      card.style.setProperty('--mx', (e.clientX - r.left) + 'px');
      card.style.setProperty('--my', (e.clientY - r.top) + 'px');
    });
  });
})();

/* ============ CALCULATOR ============ */
(function(){
  const slider = document.getElementById('billRange');
  const billLabel = document.getElementById('billLabel');
  const outKwp = document.getElementById('outKwp');
  const outPanels = document.getElementById('outPanels');
  const outMonthly = document.getElementById('outMonthly');
  const outSave25 = document.getElementById('outSave25');
  const outPayback = document.getElementById('outPayback');
  const paybackBar = document.getElementById('paybackBar');
  const insight = document.getElementById('insightText');
  const waBtn = document.getElementById('calcWhatsapp');

  const fmt = n => Math.round(n).toLocaleString('es-MX');

  function paintTrack(){
    const min = +slider.min, max = +slider.max, val = +slider.value;
    const pct = ((val - min) / (max - min)) * 100;
    slider.style.background = 'linear-gradient(to right, #FFB020 ' + pct + '%, rgba(255,255,255,0.1) ' + pct + '%)';
  }

  function calc(){
    const bill = +slider.value;
    const kwhMonth = bill / 3.2;
    const kwp = (kwhMonth * 12) / 1550;
    const panels = Math.max(2, Math.ceil(kwp / 0.55));
    const monthlySave = bill * 0.95;
    const annualSave = monthlySave * 12;
    const save25 = annualSave * 25;
    const cost = kwp * 19000;
    const payback = Math.max(1.2, cost / annualSave);

    billLabel.textContent = fmt(bill);
    outKwp.textContent = kwp.toFixed(1);
    outPanels.textContent = panels;
    outMonthly.textContent = fmt(monthlySave);
    outSave25.textContent = fmt(save25);
    outPayback.textContent = payback.toFixed(1);
    paybackBar.style.width = Math.min(100, (payback / 25) * 100) + '%';

    insight.innerHTML = 'Recuperas tu inversión en aproximadamente <strong class="text-sun-400">' + payback.toFixed(1) + ' años</strong> y disfrutas más de 20 años de energía prácticamente gratis.';

    const msg = 'Hola SHELDA, usé su calculadora solar. Pago $' + fmt(bill) + ' MXN al mes de luz. Me estimaron un sistema de ' + kwp.toFixed(1) + ' kWp (' + panels + ' paneles) con ahorro de $' + fmt(monthlySave) + '/mes. Quiero una cotización exacta, por favor.';
    waBtn.href = 'https://wa.me/5215584213690?text=' + encodeURIComponent(msg);
    paintTrack();
  }

  slider.addEventListener('input', calc);
  calc();
})();

/* ============ FAQ ============ */
document.querySelectorAll('.faq-item').forEach(item => {
  item.querySelector('.faq-q').addEventListener('click', () => {
    const wasOpen = item.classList.contains('open');
    // Close all
    document.querySelectorAll('.faq-item.open').forEach(i => i.classList.remove('open'));
    // Toggle current
    if(!wasOpen) item.classList.add('open');
  });
});

/* ============ COPY TO CLIPBOARD ============ */
document.querySelectorAll('[data-copy]').forEach(btn => {
  btn.addEventListener('click', () => {
    const text = btn.dataset.copy;
    navigator.clipboard.writeText(text).then(() => {
      const toast = document.getElementById('toast');
      const msg = document.getElementById('toastMsg');
      msg.textContent = 'Copiado: ' + text;
      toast.classList.add('show');
      setTimeout(() => toast.classList.remove('show'), 2500);
    });
  });
});

/* ============ FORM -> WHATSAPP ============ */
document.getElementById('quoteForm').addEventListener('submit', function(e){
  e.preventDefault();
  const name = document.getElementById('fName').value.trim();
  const phone = document.getElementById('fPhone').value.trim();
  const email = document.getElementById('fEmail').value.trim();
  const service = document.getElementById('fService').value;
  const msg = document.getElementById('fMsg').value.trim();

  let waMsg = 'Hola SHELDA, quiero solicitar una cotización gratuita.\n\n';
  waMsg += '👤 Nombre: ' + name + '\n';
  waMsg += '📱 Teléfono: ' + phone + '\n';
  if(email) waMsg += '📧 Email: ' + email + '\n';
  waMsg += '🔧 Servicio: ' + service + '\n';
  if(msg) waMsg += '📝 Detalles: ' + msg + '\n';

  window.open('https://wa.me/5215584213690?text=' + encodeURIComponent(waMsg), '_blank');
});

/* ============ YEAR ============ */
document.getElementById('year').textContent = new Date().getFullYear();
</script>

</body>
</html>
