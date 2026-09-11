<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SHELDA | Sistemas Fotovoltaicos en Querétaro · 12 años de experiencia</title>
<meta name="description" content="SHELDA: venta, instalación y mantenimiento de sistemas fotovoltaicos en Querétaro. 12 años de experiencia. Calcula tu sistema solar y solicita tu cotización.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@500;600;700;800&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>
<script>
tailwind.config = {
  theme: {
    extend: {
      fontFamily: {
        display: ['"Plus Jakarta Sans"', 'sans-serif'],
        body: ['Inter', 'sans-serif'],
      },
      colors: {
        brand: {50:'#F0F5FA',100:'#DCE7F2',200:'#B9CDE3',300:'#86A9CB',400:'#4F80AE',500:'#1F5F9E',600:'#174B80',700:'#123B66',800:'#0E2C4D',900:'#0A1F38',950:'#061426'},
        sun: {50:'#FFFBEB',100:'#FEF3C7',200:'#FDE68A',300:'#FCD34D',400:'#FBBF24',500:'#F59E0B',600:'#D97706'},
        leaf: {400:'#34D399',500:'#10B981',600:'#059669'},
      },
      boxShadow: {
        soft: '0 10px 40px -12px rgba(10,31,56,.18)',
        glow: '0 0 0 4px rgba(245,158,11,.18)',
      }
    }
  }
}
</script>
<style>
 html {
  scroll-behavior: smooth;
  height: 100vh;
  width: 100%;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Inter', sans-serif;
  color: #0E2C4D;
  background: #fff;
  -webkit-font-smoothing: antialiased;
  margin: 0;
  padding: 0;
  width: 100%;
  min-height: 100vh;
}
  .reveal{opacity:0;transform:translateY(28px);transition:opacity .8s cubic-bezier(.2,.7,.2,1),transform .8s cubic-bezier(.2,.7,.2,1)}
  .reveal.in{opacity:1;transform:none}
  .delay-1{transition-delay:.1s}.delay-2{transition-delay:.2s}.delay-3{transition-delay:.3s}.delay-4{transition-delay:.4s}
  .grad-text{background:linear-gradient(90deg,#FBBF24,#F59E0B 50%,#FDE68A);-webkit-background-clip:text;background-clip:text;color:transparent}
  .hero-bg{background:radial-gradient(1200px 600px at 80% -10%,rgba(31,95,158,.55),transparent 60%),radial-gradient(800px 500px at -10% 110%,rgba(245,158,11,.22),transparent 60%),linear-gradient(160deg,#061426 0%,#0A1F38 55%,#0E2C4D 100%)}
  .grid-pattern{background-image:linear-gradient(rgba(255,255,255,.05) 1px,transparent 1px),linear-gradient(90deg,rgba(255,255,255,.05) 1px,transparent 1px);background-size:44px 44px;mask-image:radial-gradient(ellipse at center,black 40%,transparent 75%)}
  /* Panel illustration */
  .panel-scene{perspective:1400px}
  .panel{transform:rotateX(55deg) rotateZ(-32deg);transform-style:preserve-3d;animation:panelfloat 7s ease-in-out infinite}
  @keyframes panelfloat{0%,100%{transform:rotateX(55deg) rotateZ(-32deg) translateZ(0)}50%{transform:rotateX(55deg) rotateZ(-32deg) translateZ(18px)}}
  .cell{background:linear-gradient(145deg,#173F7A 0%,#0F2E5C 60%,#0B2148 100%);border:1px solid rgba(255,255,255,.14);position:relative;overflow:hidden}
  .cell::after{content:'';position:absolute;inset:0;background:linear-gradient(115deg,transparent 30%,rgba(255,255,255,.35) 50%,transparent 70%);transform:translateX(-120%);animation:shine 5s ease-in-out infinite}
  .cell:nth-child(odd)::after{animation-delay:1.5s}
  @keyframes shine{0%{transform:translateX(-120%)}35%{transform:translateX(120%)}100%{transform:translateX(120%)}}
  .float-card{animation:floaty 6s ease-in-out infinite}
  .float-card.f2{animation-delay:1.6s}.float-card.f3{animation-delay:3.1s}
  @keyframes floaty{0%,100%{transform:translateY(0)}50%{transform:translateY(-12px)}}
  .sun-orb{background:radial-gradient(circle at 35% 35%,#FDE68A,#F59E0B 55%,#D97706);box-shadow:0 0 60px 18px rgba(245,158,11,.35);animation:pulse-sun 4s ease-in-out infinite}
  @keyframes pulse-sun{0%,100%{box-shadow:0 0 60px 18px rgba(245,158,11,.35)}50%{box-shadow:0 0 90px 30px rgba(245,158,11,.5)}}
  /* Nav */
  .nav-glass{backdrop-filter:blur(14px);-webkit-backdrop-filter:blur(14px)}
  .nav-link{position:relative}
  .nav-link::after{content:'';position:absolute;left:0;bottom:-6px;width:0;height:2px;background:#F59E0B;transition:width .3s}
  .nav-link:hover::after,.nav-link.active::after{width:100%}
  /* Cards */
  .card-hover{transition:transform .35s cubic-bezier(.2,.7,.2,1),box-shadow .35s}
  .card-hover:hover{transform:translateY(-6px);box-shadow:0 24px 50px -16px rgba(10,31,56,.25)}
  /* Sliders */
  input[type=range]{-webkit-appearance:none;appearance:none;width:100%;height:6px;border-radius:999px;background:linear-gradient(90deg,#F59E0B var(--p,50%),#DCE7F2 var(--p,50%));outline:none}
  input[type=range]::-webkit-slider-thumb{-webkit-appearance:none;width:22px;height:22px;border-radius:50%;background:#fff;border:3px solid #F59E0B;box-shadow:0 2px 8px rgba(0,0,0,.2);cursor:pointer;transition:transform .15s}
  input[type=range]::-webkit-slider-thumb:hover{transform:scale(1.12)}
  input[type=range]::-moz-range-thumb{width:22px;height:22px;border-radius:50%;background:#fff;border:3px solid #F59E0B;cursor:pointer}
  .field{width:100%;border:1.5px solid #DCE7F2;border-radius:.9rem;padding:.8rem 1rem;font-weight:500;background:#fff;transition:border-color .2s,box-shadow .2s}
  .field:focus{outline:none;border-color:#F59E0B;box-shadow:0 0 0 4px rgba(245,158,11,.18)}
  .stepper button{width:44px;height:44px;border-radius:.8rem;font-weight:700;font-size:1.25rem;background:#F0F5FA;color:#0E2C4D;transition:background .2s,transform .1s}
  .stepper button:hover{background:#DCE7F2}.stepper button:active{transform:scale(.94)}
  .tab-btn{transition:all .3s}
  .tab-btn.active{background:#0A1F38;color:#fff;box-shadow:0 10px 30px -10px rgba(10,31,56,.5)}
  .result-num{font-variant-numeric:tabular-nums;transition:transform .2s}
  .result-num.bump{transform:scale(1.06)}
  /* Timeline */
  .step-line::before{content:'';position:absolute;left:0;right:0;top:34px;height:2px;background:linear-gradient(90deg,transparent,#DCE7F2 10%,#DCE7F2 90%,transparent)}
  /* Project tiles */
  .proj{position:relative;overflow:hidden;border-radius:1.25rem}
  .proj::before{content:'';position:absolute;inset:0;background-image:linear-gradient(rgba(255,255,255,.12) 1px,transparent 1px),linear-gradient(90deg,rgba(255,255,255,.12) 1px,transparent 1px);background-size:28px 28px;opacity:.6;transition:transform .6s}
  .proj:hover::before{transform:scale(1.08)}
  .proj .badge{transition:transform .35s}
  .proj:hover .badge{transform:translateY(-4px)}
  /* FAQ */
  .faq-body{max-height:0;overflow:hidden;transition:max-height .45s cubic-bezier(.2,.7,.2,1),padding .3s}
  .faq.open .faq-body{max-height:300px}
  .faq.open .chev{transform:rotate(180deg)}
  .chev{transition:transform .35s}
  /* Marquee */
  .marquee{overflow:hidden;mask-image:linear-gradient(90deg,transparent,black 10%,black 90%,transparent)}
  .marquee-track{display:flex;gap:3rem;width:max-content;animation:scroll 28s linear infinite}
  @keyframes scroll{to{transform:translateX(-50%)}}
  .wa-btn{background:linear-gradient(135deg,#25D366,#128C7E);box-shadow:0 12px 30px -10px rgba(37,211,102,.6)}
  .wa-btn:hover{filter:brightness(1.06)}
  .btn-sun{background:linear-gradient(135deg,#FBBF24,#F59E0B);box-shadow:0 12px 30px -10px rgba(245,158,11,.7)}
  .btn-sun:hover{filter:brightness(1.05);transform:translateY(-1px)}
  .ring-anim{position:absolute;inset:-6px;border-radius:9999px;border:2px solid rgba(37,211,102,.5);animation:ring 2.2s ease-out infinite}
  @keyframes ring{0%{transform:scale(.9);opacity:.8}100%{transform:scale(1.35);opacity:0}}
  @media (prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}.reveal{opacity:1;transform:none}}
</style>
</head>
<body class="font-body">

<!-- ================= NAV ================= -->
<header id="nav" class="fixed top-0 inset-x-0 z-50 transition-all duration-300">
  <div class="nav-glass bg-brand-950/70 border-b border-white/5" id="navInner">
    <div class="max-w-7xl mx-auto px-5 sm:px-8 h-[72px] flex items-center justify-between">
     <a href="#inicio" class="flex items-center gap-3">
<img src="LOGO SHELDA SF.png" alt="SHELDA" class="h-12 w-auto">
       <div class="leading-none">
          <span class="font-display font-800 text-white text-xl tracking-[.14em] font-extrabold">SHELDA</span>
          <span class="block text-[10px] text-brand-200/80 tracking-widest uppercase mt-0.5">Energía Solar · Querétaro</span>
        </div>
      </a>
      <nav class="hidden lg:flex items-center gap-8 text-[14px] font-medium text-brand-100/90">
        <a class="nav-link hover:text-white" href="#servicios">Servicios</a>
        <a class="nav-link hover:text-white" href="#porque">Por qué SHELDA</a>
        <a class="nav-link hover:text-white" href="#proceso">Proceso</a>
        <a class="nav-link hover:text-white" href="#calculadora">Calculadora</a>
        <a class="nav-link hover:text-white" href="#proyectos">Proyectos</a>
        <a class="nav-link hover:text-white" href="#faq">Preguntas</a>
      </nav>
      <div class="flex items-center gap-3">
        <a href="#calculadora" class="hidden sm:inline-flex btn-sun items-center gap-2 text-brand-950 font-semibold text-sm px-5 py-2.5 rounded-xl transition">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="2" width="16" height="20" rx="2"/><path d="M8 6h8M8 10h2M12 10h2M16 10h0M8 14h2M12 14h2M16 14h0M8 18h2M12 18h2M16 18h0"/></svg>
          Calcular mi sistema
        </a>
        <button id="menuBtn" class="lg:hidden w-11 h-11 grid place-items-center rounded-xl text-white bg-white/5 hover:bg-white/10" aria-label="Menú">
          <svg id="menuIcon" width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round"><path d="M4 7h16M4 12h16M4 17h16"/></svg>
        </button>
      </div>
    </div>
    <div id="mobileMenu" class="lg:hidden hidden border-t border-white/5 bg-brand-950/95">
      <div class="px-5 py-4 flex flex-col gap-1 text-brand-100 font-medium">
        <a class="py-3 px-3 rounded-lg hover:bg-white/5" href="#servicios">Servicios</a>
        <a class="py-3 px-3 rounded-lg hover:bg-white/5" href="#porque">Por qué SHELDA</a>
        <a class="py-3 px-3 rounded-lg hover:bg-white/5" href="#proceso">Proceso</a>
        <a class="py-3 px-3 rounded-lg hover:bg-white/5" href="#calculadora">Calculadora</a>
        <a class="py-3 px-3 rounded-lg hover:bg-white/5" href="#proyectos">Proyectos</a>
        <a class="py-3 px-3 rounded-lg hover:bg-white/5" href="#faq">Preguntas</a>
        <a class="mt-2 btn-sun text-center text-brand-950 font-semibold py-3 rounded-xl" href="#calculadora">Calcular mi sistema</a>
      </div>
    </div>
  </div>
</header>

<!-- ================= HERO ================= -->
<section id="inicio" class="hero-bg relative overflow-hidden pt-[72px] text-white">
  <div class="absolute inset-0 grid-pattern pointer-events-none"></div>
  <div class="max-w-7xl mx-auto px-5 sm:px-8 pt-16 pb-20 lg:pt-24 lg:pb-28 grid lg:grid-cols-12 gap-12 items-center relative">
    <div class="lg:col-span-6 reveal">
      <div class="inline-flex items-center gap-2 bg-white/5 border border-white/10 rounded-full px-4 py-1.5 text-sm text-brand-100">
        <span class="w-2 h-2 rounded-full bg-leaf-400 animate-pulse"></span>
        12 años iluminando Querétaro con energía solar
      </div>
      <h1 class="font-display font-extrabold text-4xl sm:text-5xl lg:text-[3.6rem] leading-[1.08] mt-6 tracking-tight">
        Energía solar que <span class="grad-text">sí paga</span>, instalada por expertos.
      </h1>
      <p class="mt-6 text-lg text-brand-100/85 max-w-xl leading-relaxed">
        En <strong class="text-white">SHELDA</strong> vendemos, instalamos y damos mantenimiento a sistemas fotovoltaicos residenciales, comerciales e industriales. Ingeniería certificada, equipos Tier 1 y garantía real: reduce tu recibo de CFE hasta un <strong class="text-white">98%</strong>.
      </p>

      <!-- CONTACT (inicio) -->
      <div class="mt-8 flex flex-wrap gap-3" id="heroContact">
        <a href="https://wa.me/524423344713?text=Hola%20SHELDA%2C%20me%20interesa%20un%20sistema%20fotovoltaico.%20%C2%BFMe%20pueden%20asesorar%3F" target="_blank" rel="noopener" class="wa-btn inline-flex items-center gap-2.5 text-white font-semibold px-5 py-3.5 rounded-xl transition">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M20.5 3.5A11.9 11.9 0 0 0 12 0C5.4 0 .1 5.3.1 11.9c0 2.1.6 4.1 1.6 5.9L0 24l6.4-1.7a11.9 11.9 0 0 0 5.6 1.4c6.6 0 11.9-5.3 11.9-11.9 0-3.2-1.2-6.2-3.4-8.3zM12 21.8c-1.8 0-3.5-.5-5-1.4l-.4-.2-3.8 1 1-3.7-.2-.4A9.9 9.9 0 0 1 2.1 12C2.1 6.5 6.5 2 12 2c2.6 0 5.1 1 7 2.9a9.8 9.8 0 0 1 2.9 7c0 5.5-4.4 9.9-9.9 9.9zm5.4-7.4c-.3-.1-1.8-.9-2-1-.3-.1-.5-.1-.7.1-.2.3-.8 1-.9 1.2-.2.2-.3.2-.6.1-.3-.1-1.3-.5-2.4-1.5-.9-.8-1.5-1.8-1.7-2.1-.2-.3 0-.5.1-.6l.4-.5c.1-.2.2-.3.3-.5.1-.2 0-.4 0-.5l-.9-2.2c-.2-.6-.5-.5-.7-.5h-.6c-.2 0-.5.1-.8.4-.3.3-1 1-1 2.5s1.1 2.9 1.2 3.1c.1.2 2.1 3.2 5.1 4.5.7.3 1.3.5 1.7.6.7.2 1.4.2 1.9.1.6-.1 1.8-.7 2-1.4.2-.7.2-1.3.2-1.4-.1-.2-.3-.3-.6-.4z"/></svg>
          WhatsApp
        </a>
        <a href="tel:+524422219667" class="inline-flex items-center gap-2.5 bg-white/10 hover:bg-white/15 border border-white/15 text-white font-semibold px-5 py-3.5 rounded-xl transition">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.9v3a2 2 0 0 1-2.2 2 19.8 19.8 0 0 1-8.6-3.1 19.5 19.5 0 0 1-6-6A19.8 19.8 0 0 1 2.1 4.2 2 2 0 0 1 4.1 2h3a2 2 0 0 1 2 1.7c.1.9.4 1.9.7 2.8a2 2 0 0 1-.5 2.1L8 9.9a16 16 0 0 0 6 6l1.3-1.3a2 2 0 0 1 2.1-.4c.9.3 1.8.6 2.8.7A2 2 0 0 1 22 16.9z"/></svg>
          442 123 4567
        </a>
        <a href="mailto:sheldaingenieria@gmail.com" class="inline-flex items-center gap-2.5 bg-white/10 hover:bg-white/15 border border-white/15 text-white font-semibold px-5 py-3.5 rounded-xl transition">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m2 7 10 7 10-7"/></svg>
          sheldaingenieria@gmail.com
        </a>
      </div>

      <div class="mt-10 flex items-center gap-5 text-sm text-brand-200">
        <div class="flex -space-x-2">
          <span class="w-9 h-9 rounded-full ring-2 ring-brand-900 bg-gradient-to-br from-sun-300 to-sun-600"></span>
          <span class="w-9 h-9 rounded-full ring-2 ring-brand-900 bg-gradient-to-br from-brand-300 to-brand-600"></span>
          <span class="w-9 h-9 rounded-full ring-2 ring-brand-900 bg-gradient-to-br from-leaf-400 to-brand-500"></span>
          <span class="w-9 h-9 rounded-full ring-2 ring-brand-900 bg-brand-700 grid place-items-center text-[11px] font-bold text-white">+850</span>
        </div>
        <p>familias y empresas queretanas ya generan su propia energía.</p>
      </div>
    </div>

    <!-- Illustration -->
    <div class="lg:col-span-6 relative h-[420px] sm:h-[480px] reveal delay-2">
      <div class="absolute right-6 top-2 sm:right-14 sm:top-4 w-20 h-20 sm:w-24 sm:h-24 rounded-full sun-orb"></div>
      <div class="panel-scene absolute inset-0 grid place-items-center">
        <div class="panel w-[300px] sm:w-[360px] rounded-md p-2 bg-gradient-to-br from-slate-200 to-slate-400 shadow-[0_50px_80px_-20px_rgba(0,0,0,.6)]">
          <div id="panelCells" class="grid grid-cols-6 gap-[3px] rounded-sm overflow-hidden"></div>
        </div>
      </div>
      <!-- Floating cards -->
      <div class="float-card absolute left-0 top-6 sm:left-2 bg-white/10 backdrop-blur-md border border-white/15 rounded-2xl p-4 w-48 shadow-soft">
        <p class="text-[11px] uppercase tracking-wider text-brand-200">Generando ahora</p>
        <p class="font-display font-bold text-2xl mt-1"><span id="liveKw">4.82</span> <span class="text-sun-400 text-base">kW</span></p>
        <div class="mt-2 h-1.5 bg-white/10 rounded-full overflow-hidden"><div id="liveBar" class="h-full bg-gradient-to-r from-sun-400 to-leaf-400 rounded-full" style="width:78%"></div></div>
      </div>
      <div class="float-card f2 absolute right-0 bottom-16 sm:right-2 bg-white/10 backdrop-blur-md border border-white/15 rounded-2xl p-4 w-52 shadow-soft">
        <div class="flex items-center gap-3">
          <div class="w-10 h-10 rounded-xl bg-leaf-500/20 grid place-items-center text-leaf-400">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m3 17 6-6 4 4 8-8"/><path d="M14 7h7v7"/></svg>
          </div>
          <div>
            <p class="text-[11px] uppercase tracking-wider text-brand-200">Ahorro en recibo</p>
            <p class="font-display font-bold text-xl">-96%</p>
          </div>
        </div>
      </div>
      <div class="float-card f3 absolute left-4 bottom-2 sm:left-10 bg-white/10 backdrop-blur-md border border-white/15 rounded-2xl px-4 py-3 shadow-soft flex items-center gap-3">
        <span class="w-2.5 h-2.5 rounded-full bg-leaf-400 animate-pulse"></span>
        <p class="text-sm"><strong>Interconexión CFE</strong> aprobada</p>
      </div>
    </div>
  </div>

  <!-- Stats -->
  <div class="relative border-t border-white/10 bg-brand-950/40">
    <div class="max-w-7xl mx-auto px-5 sm:px-8 py-8 grid grid-cols-2 md:grid-cols-4 gap-6">
      <div class="reveal"><p class="font-display font-extrabold text-3xl sm:text-4xl"><span class="counter" data-to="12">0</span>+</p><p class="text-brand-200 text-sm mt-1">años de experiencia</p></div>
      <div class="reveal delay-1"><p class="font-display font-extrabold text-3xl sm:text-4xl"><span class="counter" data-to="850">0</span>+</p><p class="text-brand-200 text-sm mt-1">proyectos instalados</p></div>
      <div class="reveal delay-2"><p class="font-display font-extrabold text-3xl sm:text-4xl"><span class="counter" data-to="9.6" data-dec="1">0</span> MW</p><p class="text-brand-200 text-sm mt-1">de potencia instalada</p></div>
      <div class="reveal delay-3"><p class="font-display font-extrabold text-3xl sm:text-4xl"><span class="counter" data-to="98">0</span>%</p><p class="text-brand-200 text-sm mt-1">clientes satisfechos</p></div>
    </div>
  </div>
</section>

<!-- Marquee -->
<div class="bg-brand-50 border-b border-brand-100 py-4 marquee">
  <div class="marquee-track text-sm font-semibold text-brand-700/80 uppercase tracking-wider">
    <span>☀ Paneles Tier 1</span><span>⚡ Inversores Huawei · Fronius · SolarEdge · Enphase</span><span>✔ Trámite de interconexión CFE incluido</span><span>🛡 Garantía de 25 años en producción</span><span>📍 Querétaro, Qro. y toda la región Bajío</span><span>🔧 Mantenimiento preventivo y correctivo</span>
    <span>☀ Paneles Tier 1</span><span>⚡ Inversores Huawei · Fronius · SolarEdge · Enphase</span><span>✔ Trámite de interconexión CFE incluido</span><span>🛡 Garantía de 25 años en producción</span><span>📍 Querétaro, Qro. y toda la región Bajío</span><span>🔧 Mantenimiento preventivo y correctivo</span>
  </div>
</div>

<!-- ================= SERVICIOS ================= -->
<section id="servicios" class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-5 sm:px-8">
    <div class="max-w-2xl reveal">
      <p class="text-sun-600 font-semibold tracking-wider text-sm uppercase">Nuestros servicios</p>
      <h2 class="font-display font-extrabold text-3xl sm:text-4xl lg:text-5xl text-brand-900 mt-3 tracking-tight">Todo el ciclo solar, en un solo equipo.</h2>
      <p class="mt-4 text-brand-700/80 text-lg">Desde el diagnóstico hasta el mantenimiento anual. Sin intermediarios, sin sorpresas: ingeniería propia y responsabilidad total sobre tu sistema.</p>
    </div>
    <div class="grid md:grid-cols-3 gap-6 mt-14">
      <!-- Venta -->
      <article class="card-hover reveal relative bg-white border border-brand-100 rounded-3xl p-8 overflow-hidden">
        <div class="absolute -right-10 -top-10 w-40 h-40 rounded-full bg-sun-100 blur-2xl"></div>
        <div class="relative">
          <div class="w-14 h-14 rounded-2xl bg-gradient-to-br from-sun-400 to-sun-600 grid place-items-center text-brand-950 shadow-lg shadow-sun-500/30">
            <svg width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 9 5 3h14l2 6"/><rect x="3" y="9" width="18" height="12" rx="2"/><path d="M3 13h18M9 9v12M15 9v12"/></svg>
          </div>
          <h3 class="font-display font-bold text-2xl text-brand-900 mt-6">Venta y diseño</h3>
          <p class="mt-3 text-brand-700/80 leading-relaxed">Dimensionamos tu sistema con simulación de sombras y análisis de tu historial de consumo. Solo marcas Tier 1 con respaldo en México.</p>
          <ul class="mt-6 space-y-2.5 text-sm text-brand-800">
            <li class="flex gap-2.5"><span class="text-leaf-500 font-bold">✓</span> Estudio técnico y propuesta económica sin costo</li>
            <li class="flex gap-2.5"><span class="text-leaf-500 font-bold">✓</span> Paneles bifaciales y de alta eficiencia (≥ 21%)</li>
            <li class="flex gap-2.5"><span class="text-leaf-500 font-bold">✓</span> Opciones de financiamiento y arrendamiento</li>
          </ul>
        </div>
      </article>
      <!-- Instalación -->
      <article class="card-hover reveal delay-1 relative bg-brand-900 text-white rounded-3xl p-8 overflow-hidden">
        <div class="absolute -right-10 -top-10 w-40 h-40 rounded-full bg-brand-500/40 blur-2xl"></div>
        <div class="relative">
          <div class="w-14 h-14 rounded-2xl bg-white/10 border border-white/15 grid place-items-center text-sun-400">
            <svg width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M14.7 6.3a4 4 0 0 0 5 5l-9.4 9.4a2.1 2.1 0 0 1-3-3l9.4-9.4z"/><path d="m14 9.5 1 1"/><path d="M4 20l1-1"/></svg>
          </div>
          <h3 class="font-display font-bold text-2xl mt-6">Instalación certificada</h3>
          <p class="mt-3 text-brand-100/85 leading-relaxed">Cuadrillas propias certificadas por CONOCER y EC0586. Cumplimos NOM-001-SEDE y gestionamos tu interconexión con CFE de principio a fin.</p>
          <ul class="mt-6 space-y-2.5 text-sm text-brand-100">
            <li class="flex gap-2.5"><span class="text-sun-400 font-bold">✓</span> Estructuras de aluminio anodizado y acero galvanizado</li>
            <li class="flex gap-2.5"><span class="text-sun-400 font-bold">✓</span> Protecciones DC/AC, tierras físicas y supresores</li>
            <li class="flex gap-2.5"><span class="text-sun-400 font-bold">✓</span> Entrega con monitoreo en tu celular</li>
          </ul>
        </div>
      </article>
      <!-- Mantenimiento -->
      <article class="card-hover reveal delay-2 relative bg-white border border-brand-100 rounded-3xl p-8 overflow-hidden">
        <div class="absolute -right-10 -top-10 w-40 h-40 rounded-full bg-leaf-400/20 blur-2xl"></div>
        <div class="relative">
          <div class="w-14 h-14 rounded-2xl bg-gradient-to-br from-leaf-400 to-leaf-600 grid place-items-center text-white shadow-lg shadow-leaf-500/30">
            <svg width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/><path d="m9 12 2 2 4-4"/></svg>
          </div>
          <h3 class="font-display font-bold text-2xl text-brand-900 mt-6">Mantenimiento y monitoreo</h3>
          <p class="mt-3 text-brand-700/80 leading-relaxed">Un sistema limpio y revisado produce hasta 15% más. Planes anuales con limpieza, termografía, revisión eléctrica y reporte de desempeño.</p>
          <ul class="mt-6 space-y-2.5 text-sm text-brand-800">
            <li class="flex gap-2.5"><span class="text-leaf-500 font-bold">✓</span> Limpieza con agua desionizada</li>
            <li class="flex gap-2.5"><span class="text-leaf-500 font-bold">✓</span> Termografía y prueba de curvas I-V</li>
            <li class="flex gap-2.5"><span class="text-leaf-500 font-bold">✓</span> Atención a sistemas de otras empresas</li>
          </ul>
        </div>
      </article>
    </div>
  </div>
</section>

<!-- ================= POR QUÉ SHELDA ================= -->
<section id="porque" class="py-24 bg-brand-50 relative overflow-hidden">
  <div class="absolute -left-40 top-20 w-96 h-96 bg-sun-200/40 rounded-full blur-3xl"></div>
  <div class="max-w-7xl mx-auto px-5 sm:px-8 relative">
    <div class="grid lg:grid-cols-12 gap-12 items-start">
      <div class="lg:col-span-5 lg:sticky lg:top-28 reveal">
        <p class="text-sun-600 font-semibold tracking-wider text-sm uppercase">Por qué SHELDA</p>
        <h2 class="font-display font-extrabold text-3xl sm:text-4xl lg:text-5xl text-brand-900 mt-3 tracking-tight">12 años de ingeniería, no de improvisación.</h2>
        <p class="mt-5 text-brand-700/80 text-lg leading-relaxed">Hemos visto de todo en techos queretanos: desde láminas industriales hasta tejas coloniales. Esa experiencia se traduce en sistemas que producen lo prometido, año tras año.</p>
        <div class="mt-8 p-6 bg-white rounded-2xl border border-brand-100 shadow-soft">
          <div class="flex items-center justify-between text-sm font-semibold text-brand-800"><span>Producción real vs. prometida</span><span class="text-leaf-600">103%</span></div>
          <div class="mt-3 h-3 bg-brand-100 rounded-full overflow-hidden"><div class="h-full w-0 bg-gradient-to-r from-sun-400 to-leaf-500 rounded-full transition-all duration-[1600ms] barfill" data-w="100%"></div></div>
          <p class="text-xs text-brand-700/70 mt-3">Promedio de nuestra flota monitoreada (2019–2024). Diseñamos conservador para superar expectativas.</p>
        </div>
      </div>
      <div class="lg:col-span-7 grid sm:grid-cols-2 gap-5">
        <div class="card-hover reveal bg-white rounded-2xl p-6 border border-brand-100">
          <div class="w-11 h-11 rounded-xl bg-sun-100 text-sun-600 grid place-items-center"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2 2 7l10 5 10-5-10-5z"/><path d="m2 17 10 5 10-5"/><path d="m2 12 10 5 10-5"/></svg></div>
          <h3 class="font-display font-bold text-lg text-brand-900 mt-4">Equipos Tier 1 con garantía real</h3>
          <p class="text-sm text-brand-700/80 mt-2 leading-relaxed">25 años de producción en paneles y 10–12 en inversores, con centros de servicio en México. Nosotros gestionamos cualquier garantía por ti.</p>
        </div>
        <div class="card-hover reveal delay-1 bg-white rounded-2xl p-6 border border-brand-100">
          <div class="w-11 h-11 rounded-xl bg-brand-100 text-brand-600 grid place-items-center"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 12h6M12 9v6"/><path d="M20 7 12 3 4 7v10l8 4 8-4z"/></svg></div>
          <h3 class="font-display font-bold text-lg text-brand-900 mt-4">Ingeniería propia certificada</h3>
          <p class="text-sm text-brand-700/80 mt-2 leading-relaxed">Ingenieros eléctricos con estándar EC0586 y UVIE aliada. Diseñamos con PVsyst y análisis de sombras 3D para cada techo.</p>
        </div>
        <div class="card-hover reveal delay-2 bg-white rounded-2xl p-6 border border-brand-100">
          <div class="w-11 h-11 rounded-xl bg-leaf-400/20 text-leaf-600 grid place-items-center"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 8v4l3 3"/><circle cx="12" cy="12" r="9"/></svg></div>
          <h3 class="font-display font-bold text-lg text-brand-900 mt-4">Trámite CFE en tiempo récord</h3>
          <p class="text-sm text-brand-700/80 mt-2 leading-relaxed">Conocemos los procesos de la División Bajío. Contrato de interconexión y cambio de medidor bidireccional sin que tú muevas un dedo.</p>
        </div>
        <div class="card-hover reveal delay-3 bg-white rounded-2xl p-6 border border-brand-100">
          <div class="w-11 h-11 rounded-xl bg-sun-100 text-sun-600 grid place-items-center"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><rect x="5" y="2" width="14" height="20" rx="2"/><path d="M12 18h.01"/></svg></div>
          <h3 class="font-display font-bold text-lg text-brand-900 mt-4">Monitoreo 24/7 desde tu celular</h3>
          <p class="text-sm text-brand-700/80 mt-2 leading-relaxed">Sabrás cuánto generas cada hora. Nuestro centro de monitoreo detecta caídas de producción antes de que las notes.</p>
        </div>
        <div class="card-hover reveal delay-2 bg-white rounded-2xl p-6 border border-brand-100">
          <div class="w-11 h-11 rounded-xl bg-brand-100 text-brand-600 grid place-items-center"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 21h18"/><path d="M5 21V7l7-4 7 4v14"/><path d="M9 21v-6h6v6"/></svg></div>
          <h3 class="font-display font-bold text-lg text-brand-900 mt-4">Estructuras a la medida</h3>
          <p class="text-sm text-brand-700/80 mt-2 leading-relaxed">Losa, lámina, teja, pergolado o piso. Cálculo de cargas de viento según zona y garantía de impermeabilidad en cada fijación.</p>
        </div>
        <div class="card-hover reveal delay-3 bg-gradient-to-br from-brand-900 to-brand-700 text-white rounded-2xl p-6">
          <div class="w-11 h-11 rounded-xl bg-white/10 text-sun-400 grid place-items-center"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"/></svg></div>
          <h3 class="font-display font-bold text-lg mt-4">Garantía SHELDA de 5 años en instalación</h3>
          <p class="text-sm text-brand-100/85 mt-2 leading-relaxed">Mano de obra, cableado, estructura y sellado. Si algo falla por nuestra instalación, lo resolvemos sin costo. Así de simple.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ================= PROCESO ================= -->
<section id="proceso" class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-5 sm:px-8">
    <div class="text-center max-w-2xl mx-auto reveal">
      <p class="text-sun-600 font-semibold tracking-wider text-sm uppercase">Nuestro proceso</p>
      <h2 class="font-display font-extrabold text-3xl sm:text-4xl lg:text-5xl text-brand-900 mt-3 tracking-tight">De tu recibo a tu techo en 5 pasos.</h2>
      <p class="mt-4 text-brand-700/80 text-lg">Un proceso claro y sin sorpresas. La mayoría de nuestros proyectos residenciales se instalan en 1–2 días.</p>
    </div>
    <div class="relative mt-16 grid md:grid-cols-5 gap-8 md:step-line">
      <div class="reveal text-center relative">
        <div class="w-[68px] h-[68px] mx-auto rounded-2xl bg-white border-2 border-sun-400 grid place-items-center font-display font-extrabold text-xl text-brand-900 shadow-soft relative z-10">01</div>
        <h3 class="font-display font-bold text-brand-900 mt-5">Diagnóstico</h3>
        <p class="text-sm text-brand-700/80 mt-2">Analizamos tu recibo de CFE, hábitos de consumo y visitamos tu techo.</p>
      </div>
      <div class="reveal delay-1 text-center relative">
        <div class="w-[68px] h-[68px] mx-auto rounded-2xl bg-white border-2 border-sun-400 grid place-items-center font-display font-extrabold text-xl text-brand-900 shadow-soft relative z-10">02</div>
        <h3 class="font-display font-bold text-brand-900 mt-5">Diseño y propuesta</h3>
        <p class="text-sm text-brand-700/80 mt-2">Simulación de producción, plano de arreglo y propuesta económica transparente.</p>
      </div>
      <div class="reveal delay-2 text-center relative">
        <div class="w-[68px] h-[68px] mx-auto rounded-2xl bg-white border-2 border-sun-400 grid place-items-center font-display font-extrabold text-xl text-brand-900 shadow-soft relative z-10">03</div>
        <h3 class="font-display font-bold text-brand-900 mt-5">Instalación</h3>
        <p class="text-sm text-brand-700/80 mt-2">Cuadrilla certificada, materiales de primera y pruebas eléctricas completas.</p>
      </div>
      <div class="reveal delay-3 text-center relative">
        <div class="w-[68px] h-[68px] mx-auto rounded-2xl bg-white border-2 border-sun-400 grid place-items-center font-display font-extrabold text-xl text-brand-900 shadow-soft relative z-10">04</div>
        <h3 class="font-display font-bold text-brand-900 mt-5">Interconexión CFE</h3>
        <p class="text-sm text-brand-700/80 mt-2">Gestionamos contrato, UVIE y medidor bidireccional. Tú solo firmas.</p>
      </div>
      <div class="reveal delay-4 text-center relative">
        <div class="w-[68px] h-[68px] mx-auto rounded-2xl bg-gradient-to-br from-sun-400 to-sun-600 grid place-items-center font-display font-extrabold text-xl text-brand-950 shadow-lg shadow-sun-500/40 relative z-10">05</div>
        <h3 class="font-display font-bold text-brand-900 mt-5">Monitoreo y mantenimiento</h3>
        <p class="text-sm text-brand-700/80 mt-2">App de monitoreo, reportes y planes de mantenimiento para 25 años de producción.</p>
      </div>
    </div>
  </div>
</section>

<!-- ================= CALCULADORA ================= -->
<section id="calculadora" class="py-24 relative overflow-hidden hero-bg text-white">
  <div class="absolute inset-0 grid-pattern pointer-events-none"></div>
  <div class="max-w-7xl mx-auto px-5 sm:px-8 relative">
    <div class="text-center max-w-2xl mx-auto reveal">
      <p class="text-sun-400 font-semibold tracking-wider text-sm uppercase">Calculadora solar</p>
      <h2 class="font-display font-extrabold text-3xl sm:text-4xl lg:text-5xl mt-3 tracking-tight">¿Qué sistema necesitas? Descúbrelo en 30 segundos.</h2>
      <p class="mt-4 text-brand-100/85 text-lg">Estimación basada en la radiación solar real de Querétaro (5.6 kWh/m²/día). Elige el método que prefieras.</p>
    </div>

    <!-- Tabs -->
    <div class="mt-10 flex justify-center reveal">
      <div class="inline-flex bg-white/10 border border-white/10 rounded-2xl p-1.5 gap-1.5" role="tablist">
        <button class="tab-btn active px-5 sm:px-6 py-3 rounded-xl text-sm font-semibold text-brand-100 flex items-center gap-2" data-tab="recibo" role="tab">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6M8 13h8M8 17h5"/></svg>
          Por mi recibo de CFE
        </button>
        <button class="tab-btn px-5 sm:px-6 py-3 rounded-xl text-sm font-semibold text-brand-100 flex items-center gap-2" data-tab="equipos" role="tab">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 17h14l-1.5-5H6.5z"/><circle cx="7.5" cy="17.5" r="1.5"/><circle cx="16.5" cy="17.5" r="1.5"/><path d="M8 12l1.5-4h5L16 12"/></svg>
          Por mis autos y clima
        </button>
      </div>
    </div>

    <div class="mt-10 grid lg:grid-cols-12 gap-6 reveal">
      <!-- INPUTS -->
      <div class="lg:col-span-7 bg-white text-brand-900 rounded-3xl p-6 sm:p-8 shadow-2xl">
        <!-- TAB 1 -->
        <div id="tab-recibo" class="tab-panel">
          <h3 class="font-display font-bold text-xl">Cuéntanos de tu recibo</h3>
          <p class="text-sm text-brand-700/70 mt-1">Toma el total a pagar de tu último recibo de CFE.</p>

          <div class="mt-6">
            <div class="flex items-center justify-between mb-2">
              <label class="text-sm font-semibold" for="billAmount">¿Cuánto pagas de luz?</label>
              <div class="inline-flex bg-brand-50 rounded-lg p-1 text-xs font-semibold">
                <button class="period-btn px-3 py-1.5 rounded-md bg-brand-900 text-white" data-period="2">Bimestral</button>
                <button class="period-btn px-3 py-1.5 rounded-md text-brand-700" data-period="1">Mensual</button>
              </div>
            </div>
            <div class="relative">
<span class="absolute left-4 top-1/2 -translate-y-1/2 text-brand-400 font-semibold text-sm">$</span>
              
<input id="billAmount" type="number" min="200" max="100000" step="50" value="3500" class="field pl-14 text-lg font-display font-bold">            </div>
            <input id="billRange" type="range" min="500" max="30000" step="100" value="3500" class="mt-4">
            <div class="flex justify-between text-[11px] text-brand-400 mt-1"><span>$500</span><span>$30,000+</span></div>
          </div>

          <div class="mt-6 grid sm:grid-cols-2 gap-5">
            <div>
              <label class="text-sm font-semibold block mb-2" for="tariff">Tarifa CFE</label>
              <select id="tariff" class="field">
                <option value="1" data-price="3.1">Residencial (Tarifa 1 / 1B)</option>
                <option value="DAC" data-price="6.9" selected>Residencial DAC (Alto consumo)</option>
                <option value="PDBT" data-price="5.7">Comercial PDBT (Baja tensión)</option>
                <option value="GDMTO" data-price="4.3">Media tensión GDMTO</option>
              </select>
            </div>
            <div>
              <label class="text-sm font-semibold block mb-2" for="coverage">Porcentaje a cubrir</label>
              <select id="coverage" class="field">
                <option value="1">100 % — Eliminar el recibo</option>
                <option value="0.8">80 % — Salir de DAC</option>
                <option value="0.5">50 % — Iniciar y crecer después</option>
              </select>
            </div>
          </div>

          <div class="mt-6 flex items-start gap-3 p-4 bg-sun-50 border border-sun-200 rounded-xl text-sm text-brand-800">
            <svg class="shrink-0 mt-0.5 text-sun-600" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><path d="M12 16v-4M12 8h.01"/></svg>
            <p><strong>¿No sabes tu tarifa?</strong> Aparece en la parte superior de tu recibo. Si pagas más de ~$2,500 bimestrales en casa, es muy probable que estés en <strong>DAC</strong>.</p>
          </div>
        </div>

        <!-- TAB 2 -->
        <div id="tab-equipos" class="tab-panel hidden">
          <h3 class="font-display font-bold text-xl">Cuéntanos qué vas a alimentar</h3>
          <p class="text-sm text-brand-700/70 mt-1">Ideal si estás por comprar un auto eléctrico o instalar aire acondicionado.</p>

          <div class="mt-6">
            <label class="text-sm font-semibold block mb-2" for="homeBase">Consumo base de tu casa o negocio</label>
            <select id="homeBase" class="field">
              <option value="150">Departamento / casa pequeña (~150 kWh/mes)</option>
              <option value="300" selected>Casa mediana (~300 kWh/mes)</option>
              <option value="550">Casa grande (~550 kWh/mes)</option>
              <option value="1200">Negocio pequeño (~1,200 kWh/mes)</option>
              <option value="3000">Negocio mediano (~3,000 kWh/mes)</option>
            </select>
          </div>

          <div class="mt-6 grid sm:grid-cols-2 gap-5">
            <div class="p-4 rounded-2xl border border-brand-100 bg-brand-50/60">
              <div class="flex items-center gap-2 text-sm font-semibold"><span class="text-lg">🔋</span> Autos 100 % eléctricos</div>
              <div class="stepper flex items-center justify-between mt-3">
                <button data-step="-1" data-target="evCount">−</button>
                <span id="evCount" class="font-display font-extrabold text-2xl">1</span>
                <button data-step="1" data-target="evCount">+</button>
              </div>
              <p class="text-[11px] text-brand-700/60 mt-2">≈ 9 kWh/día c/u (40 km diarios)</p>
            </div>
            <div class="p-4 rounded-2xl border border-brand-100 bg-brand-50/60">
              <div class="flex items-center gap-2 text-sm font-semibold"><span class="text-lg">⚡</span> Híbridos enchufables</div>
              <div class="stepper flex items-center justify-between mt-3">
                <button data-step="-1" data-target="phevCount">−</button>
                <span id="phevCount" class="font-display font-extrabold text-2xl">0</span>
                <button data-step="1" data-target="phevCount">+</button>
              </div>
              <p class="text-[11px] text-brand-700/60 mt-2">≈ 4 kWh/día c/u</p>
            </div>
          </div>

          <div class="mt-5 p-4 rounded-2xl border border-brand-100 bg-brand-50/60">
            <div class="flex items-center gap-2 text-sm font-semibold"><span class="text-lg">❄️</span> Aires acondicionados</div>
            <div class="grid sm:grid-cols-3 gap-4 mt-3 items-end">
              <div>
                <p class="text-xs text-brand-700/70 mb-1">Cantidad de equipos</p>
                <div class="stepper flex items-center justify-between bg-white rounded-xl p-1">
                  <button data-step="-1" data-target="acCount">−</button>
                  <span id="acCount" class="font-display font-extrabold text-2xl">2</span>
                  <button data-step="1" data-target="acCount">+</button>
                </div>
              </div>
              <div>
                <p class="text-xs text-brand-700/70 mb-1">Capacidad promedio</p>
                <select id="acTons" class="field py-3">
                  <option value="1.1">1 tonelada (12,000 BTU)</option>
                  <option value="1.6" selected>1.5 toneladas (18,000 BTU)</option>
                  <option value="2.1">2 toneladas (24,000 BTU)</option>
                  <option value="3.2">3 toneladas (36,000 BTU)</option>
                </select>
              </div>
              <div>
                <p class="text-xs text-brand-700/70 mb-1">Horas de uso al día: <strong id="acHoursLbl">6</strong> h</p>
                <input id="acHours" type="range" min="0" max="16" step="1" value="6" class="mt-3">
              </div>
            </div>
          </div>

          <div class="mt-5 grid sm:grid-cols-2 gap-5">
            <label class="flex items-center gap-3 p-4 rounded-2xl border border-brand-100 cursor-pointer hover:bg-brand-50/60 transition">
              <input id="hasPool" type="checkbox" class="w-5 h-5 accent-sun-500">
              <span class="text-sm font-semibold">🏊 Bomba de alberca <span class="block text-[11px] font-normal text-brand-700/60">≈ 6 kWh/día</span></span>
            </label>
            <label class="flex items-center gap-3 p-4 rounded-2xl border border-brand-100 cursor-pointer hover:bg-brand-50/60 transition">
              <input id="hasHeater" type="checkbox" class="w-5 h-5 accent-sun-500">
              <span class="text-sm font-semibold">🚿 Calentador eléctrico <span class="block text-[11px] font-normal text-brand-700/60">≈ 5 kWh/día</span></span>
            </label>
          </div>
        </div>
      </div>

      <!-- RESULTS -->
      <div class="lg:col-span-5">
        <div class="bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-6 sm:p-8 h-full flex flex-col">
          <div class="flex items-center justify-between">
            <p class="text-xs uppercase tracking-wider text-brand-200">Tu sistema recomendado</p>
            <span id="sysTag" class="text-[11px] font-semibold bg-sun-500/20 text-sun-300 border border-sun-400/30 px-2.5 py-1 rounded-full">Residencial</span>
          </div>
          <div class="mt-4 flex items-end gap-2">
            <span id="rKwp" class="result-num font-display font-extrabold text-6xl leading-none">5.5</span>
            <span class="font-display font-bold text-2xl text-sun-400 mb-1">kWp</span>
          </div>
          <p class="text-brand-100/80 text-sm mt-2">Consumo estimado: <strong id="rKwhMonth" class="text-white result-num">1,010</strong> kWh/mes</p>

          <div class="grid grid-cols-2 gap-3 mt-6">
            <div class="bg-white/5 rounded-2xl p-4 border border-white/10">
              <p class="text-[11px] uppercase tracking-wider text-brand-200">Paneles 720 W</p>
              <p class="font-display font-extrabold text-2xl mt-1"><span id="rPanels" class="result-num">10</span></p>
            </div>
            <div class="bg-white/5 rounded-2xl p-4 border border-white/10">
              <p class="text-[11px] uppercase tracking-wider text-brand-200">Área en techo</p>
              <p class="font-display font-extrabold text-2xl mt-1"><span id="rArea" class="result-num">26</span> <span class="text-sm font-semibold text-brand-200">m²</span></p>
            </div>
            <div class="bg-white/5 rounded-2xl p-4 border border-white/10">
              <p class="text-[11px] uppercase tracking-wider text-brand-200">Generación anual</p>
              <p class="font-display font-extrabold text-2xl mt-1"><span id="rGen" class="result-num">9,000</span> <span class="text-sm font-semibold text-brand-200">kWh</span></p>
            </div>
            <div class="bg-white/5 rounded-2xl p-4 border border-white/10">
              <p class="text-[11px] uppercase tracking-wider text-brand-200">Ahorro anual est.</p>
<p class="font-display font-extrabold text-xl mt-1 text-leaf-400 whitespace-nowrap">$<span id="rSave" class="result-num">60,000</span></p>            </div>
          </div>

          <div class="mt-5 flex items-center gap-3 bg-leaf-500/15 border border-leaf-400/30 rounded-2xl p-4">
            <span class="text-2xl">🌳</span>
            <p class="text-sm text-brand-100">Evitas <strong id="rCo2" class="text-white result-num">3.9</strong> ton de CO₂ al año, equivalente a plantar <strong id="rTrees" class="text-white result-num">180</strong> árboles.</p>
          </div>

          <div class="mt-auto pt-6">
            <a id="waQuote" href="#" target="_blank" rel="noopener" class="wa-btn relative w-full inline-flex items-center justify-center gap-2.5 text-white font-semibold px-5 py-4 rounded-2xl transition text-base">
              <svg width="22" height="22" viewBox="0 0 24 24" fill="currentColor"><path d="M20.5 3.5A11.9 11.9 0 0 0 12 0C5.4 0 .1 5.3.1 11.9c0 2.1.6 4.1 1.6 5.9L0 24l6.4-1.7a11.9 11.9 0 0 0 5.6 1.4c6.6 0 11.9-5.3 11.9-11.9 0-3.2-1.2-6.2-3.4-8.3zM12 21.8c-1.8 0-3.5-.5-5-1.4l-.4-.2-3.8 1 1-3.7-.2-.4A9.9 9.9 0 0 1 2.1 12C2.1 6.5 6.5 2 12 2c2.6 0 5.1 1 7 2.9a9.8 9.8 0 0 1 2.9 7c0 5.5-4.4 9.9-9.9 9.9zm5.4-7.4c-.3-.1-1.8-.9-2-1-.3-.1-.5-.1-.7.1-.2.3-.8 1-.9 1.2-.2.2-.3.2-.6.1-.3-.1-1.3-.5-2.4-1.5-.9-.8-1.5-1.8-1.7-2.1-.2-.3 0-.5.1-.6l.4-.5c.1-.2.2-.3.3-.5.1-.2 0-.4 0-.5l-.9-2.2c-.2-.6-.5-.5-.7-.5h-.6c-.2 0-.5.1-.8.4-.3.3-1 1-1 2.5s1.1 2.9 1.2 3.1c.1.2 2.1 3.2 5.1 4.5.7.3 1.3.5 1.7.6.7.2 1.4.2 1.9.1.6-.1 1.8-.7 2-1.4.2-.7.2-1.3.2-1.4-.1-.2-.3-.3-.6-.4z"/></svg>
              Solicitar cotización por WhatsApp
            </a>
            <p class="text-[11px] text-brand-200/70 text-center mt-3">Enviaremos tus resultados a nuestro equipo. Estimación orientativa; la propuesta final se define tras la visita técnica.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ================= PROYECTOS ================= -->
<section id="proyectos" class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-5 sm:px-8">
    <div class="flex flex-col md:flex-row md:items-end md:justify-between gap-6 reveal">
      <div class="max-w-2xl">
        <p class="text-sun-600 font-semibold tracking-wider text-sm uppercase">Proyectos destacados</p>
        <h2 class="font-display font-extrabold text-3xl sm:text-4xl lg:text-5xl text-brand-900 mt-3 tracking-tight">Techos que ya trabajan para sus dueños.</h2>
      </div>
      <p class="text-brand-700/80 md:max-w-sm">Más de 850 sistemas en Querétaro, San Juan del Río, Corregidora, El Marqués y toda la región Bajío.</p>
    </div>
    <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-5 mt-12">
      <div class="proj card-hover reveal h-72 bg-gradient-to-br from-brand-700 via-brand-800 to-brand-950 p-6 flex flex-col justify-end text-white">
        <span class="badge self-start text-[11px] font-semibold bg-sun-500 text-brand-950 px-2.5 py-1 rounded-full mb-3">Residencial</span>
        <h3 class="font-display font-bold text-xl">Casa en Juriquilla</h3>
        <p class="text-brand-100/80 text-sm mt-1">6.6 kWp · 12 paneles · Salió de tarifa DAC · Ahorro 97%</p>
      </div>
      <div class="proj card-hover reveal delay-1 h-72 bg-gradient-to-br from-sun-500 via-sun-600 to-brand-900 p-6 flex flex-col justify-end text-white">
        <span class="badge self-start text-[11px] font-semibold bg-white text-brand-900 px-2.5 py-1 rounded-full mb-3">Industrial</span>
        <h3 class="font-display font-bold text-xl">Nave en Parque Industrial Bernardo Quintana</h3>
        <p class="text-brand-100/90 text-sm mt-1">248 kWp · 450 paneles · Retorno en 3.2 años</p>
      </div>
      <div class="proj card-hover reveal delay-2 h-72 bg-gradient-to-br from-leaf-500 via-brand-600 to-brand-900 p-6 flex flex-col justify-end text-white">
        <span class="badge self-start text-[11px] font-semibold bg-white text-brand-900 px-2.5 py-1 rounded-full mb-3">Agroindustrial</span>
        <h3 class="font-display font-bold text-xl">Bombeo solar en Ezequiel Montes</h3>
        <p class="text-brand-100/90 text-sm mt-1">32 kWp · Riego de 40 ha sin diésel</p>
      </div>
      <div class="proj card-hover reveal h-72 bg-gradient-to-br from-brand-500 via-brand-700 to-brand-950 p-6 flex flex-col justify-end text-white">
        <span class="badge self-start text-[11px] font-semibold bg-sun-500 text-brand-950 px-2.5 py-1 rounded-full mb-3">Comercial</span>
        <h3 class="font-display font-bold text-xl">Restaurante en Centro Histórico</h3>
        <p class="text-brand-100/80 text-sm mt-1">28 kWp · Estructura sobre teja · Permiso INAH gestionado</p>
      </div>
      <div class="proj card-hover reveal delay-1 h-72 bg-gradient-to-br from-brand-800 via-brand-900 to-sun-600 p-6 flex flex-col justify-end text-white">
        <span class="badge self-start text-[11px] font-semibold bg-sun-500 text-brand-950 px-2.5 py-1 rounded-full mb-3">Residencial + EV</span>
        <h3 class="font-display font-bold text-xl">Casa con 2 autos eléctricos, El Refugio</h3>
        <p class="text-brand-100/80 text-sm mt-1">12.1 kWp · Cargador nivel 2 · Baterías 10 kWh</p>
      </div>
      <div class="proj card-hover reveal delay-2 h-72 bg-gradient-to-br from-brand-600 via-leaf-600 to-brand-900 p-6 flex flex-col justify-end text-white">
        <span class="badge self-start text-[11px] font-semibold bg-white text-brand-900 px-2.5 py-1 rounded-full mb-3">Educativo</span>
        <h3 class="font-display font-bold text-xl">Colegio en Corregidora</h3>
        <p class="text-brand-100/90 text-sm mt-1">85 kWp · Techumbre de estacionamiento (carport)</p>
      </div>
    </div>
  </div>
</section>

<!-- ================= TESTIMONIOS ================= -->
<section class="py-24 bg-brand-50">
  <div class="max-w-7xl mx-auto px-5 sm:px-8">
    <div class="text-center max-w-2xl mx-auto reveal">
      <p class="text-sun-600 font-semibold tracking-wider text-sm uppercase">Testimonios</p>
      <h2 class="font-display font-extrabold text-3xl sm:text-4xl lg:text-5xl text-brand-900 mt-3 tracking-tight">Lo que dicen nuestros clientes.</h2>
    </div>
    <div class="grid md:grid-cols-3 gap-6 mt-12">
      <figure class="card-hover reveal bg-white rounded-3xl p-7 border border-brand-100">
        <div class="text-sun-500 tracking-widest">★★★★★</div>
        <blockquote class="mt-4 text-brand-800 leading-relaxed">"Pagábamos $5,800 bimestrales en DAC. Desde que SHELDA instaló, el recibo llegó en $118. Todo el trámite con CFE lo hicieron ellos."</blockquote>
        <figcaption class="mt-6 flex items-center gap-3">
          <span class="w-11 h-11 rounded-full bg-gradient-to-br from-sun-300 to-sun-600 grid place-items-center font-bold text-brand-950">MG</span>
          <div><p class="font-semibold text-brand-900">Mariana G.</p><p class="text-xs text-brand-700/70">Zibatá, Querétaro · 7.7 kWp</p></div>
        </figcaption>
      </figure>
      <figure class="card-hover reveal delay-1 bg-white rounded-3xl p-7 border border-brand-100">
        <div class="text-sun-500 tracking-widest">★★★★★</div>
        <blockquote class="mt-4 text-brand-800 leading-relaxed">"Cotizamos con cuatro empresas. SHELDA fue la única que subió al techo antes de cotizar y explicó las sombras. La producción supera lo que prometieron."</blockquote>
        <figcaption class="mt-6 flex items-center gap-3">
          <span class="w-11 h-11 rounded-full bg-gradient-to-br from-brand-400 to-brand-700 grid place-items-center font-bold text-white">RA</span>
          <div><p class="font-semibold text-brand-900">Ing. Roberto A.</p><p class="text-xs text-brand-700/70">Dirección de planta · 180 kWp</p></div>
        </figcaption>
      </figure>
      <figure class="card-hover reveal delay-2 bg-white rounded-3xl p-7 border border-brand-100">
        <div class="text-sun-500 tracking-widest">★★★★★</div>
        <blockquote class="mt-4 text-brand-800 leading-relaxed">"Compramos un auto eléctrico y ampliaron nuestro sistema sin problema. El mantenimiento anual es puntual y siempre nos mandan el reporte."</blockquote>
        <figcaption class="mt-6 flex items-center gap-3">
          <span class="w-11 h-11 rounded-full bg-gradient-to-br from-leaf-400 to-brand-600 grid place-items-center font-bold text-white">LC</span>
          <div><p class="font-semibold text-brand-900">Familia López C.</p><p class="text-xs text-brand-700/70">El Campanario · 11 kWp</p></div>
        </figcaption>
      </figure>
    </div>
  </div>
</section>

<!-- ================= FAQ ================= -->
<section id="faq" class="py-24 bg-white">
  <div class="max-w-4xl mx-auto px-5 sm:px-8">
    <div class="text-center reveal">
      <p class="text-sun-600 font-semibold tracking-wider text-sm uppercase">Preguntas frecuentes</p>
      <h2 class="font-display font-extrabold text-3xl sm:text-4xl lg:text-5xl text-brand-900 mt-3 tracking-tight">Resolvemos tus dudas.</h2>
    </div>
    <div class="mt-12 space-y-3">
      <div class="faq reveal border border-brand-100 rounded-2xl bg-white overflow-hidden">
        <button class="faq-btn w-full flex items-center justify-between gap-4 text-left px-6 py-5 font-display font-bold text-brand-900">¿En cuánto tiempo recupero mi inversión?<svg class="chev shrink-0 text-sun-600" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="m6 9 6 6 6-6"/></svg></button>
        <div class="faq-body px-6 text-brand-700/85 leading-relaxed"><p class="pb-6">En tarifa DAC, típicamente entre 2.5 y 4 años. En tarifas comerciales, entre 3 y 5 años. Considerando 25 años de vida útil, el retorno total suele superar 6 veces la inversión inicial.</p></div>
      </div>
      <div class="faq reveal border border-brand-100 rounded-2xl bg-white overflow-hidden">
        <button class="faq-btn w-full flex items-center justify-between gap-4 text-left px-6 py-5 font-display font-bold text-brand-900">¿Qué pasa en días nublados o de noche?<svg class="chev shrink-0 text-sun-600" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="m6 9 6 6 6-6"/></svg></button>
        <div class="faq-body px-6 text-brand-700/85 leading-relaxed"><p class="pb-6">Con la interconexión a CFE (net metering), la energía que sobra de día se "guarda" como crédito en la red y la usas de noche. Tu medidor bidireccional lleva la cuenta. No necesitas baterías, aunque podemos integrarlas si quieres respaldo ante apagones.</p></div>
      </div>
      <div class="faq reveal border border-brand-100 rounded-2xl bg-white overflow-hidden">
        <button class="faq-btn w-full flex items-center justify-between gap-4 text-left px-6 py-5 font-display font-bold text-brand-900">¿Cuánto mantenimiento requiere un sistema solar?<svg class="chev shrink-0 text-sun-600" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="m6 9 6 6 6-6"/></svg></button>
        <div class="faq-body px-6 text-brand-700/85 leading-relaxed"><p class="pb-6">Muy poco: una limpieza y revisión eléctrica 1–2 veces al año. En Querétaro el polvo y el polen en primavera pueden reducir la producción entre 8 y 15%, por eso ofrecemos planes anuales con reporte de desempeño.</p></div>
      </div>
      <div class="faq reveal border border-brand-100 rounded-2xl bg-white overflow-hidden">
        <button class="faq-btn w-full flex items-center justify-between gap-4 text-left px-6 py-5 font-display font-bold text-brand-900">¿Mi techo aguanta? ¿Se puede en teja o lámina?<svg class="chev shrink-0 text-sun-600" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="m6 9 6 6 6-6"/></svg></button>
        <div class="faq-body px-6 text-brand-700/85 leading-relaxed"><p class="pb-6">Sí. Un sistema pesa entre 12 y 15 kg/m², menos que una persona caminando. Tenemos estructuras específicas para losa, lámina, teja, pergolados y piso, con garantía de impermeabilidad en cada fijación.</p></div>
      </div>
      <div class="faq reveal border border-brand-100 rounded-2xl bg-white overflow-hidden">
        <button class="faq-btn w-full flex items-center justify-between gap-4 text-left px-6 py-5 font-display font-bold text-brand-900">¿Puedo ampliar el sistema si compro un auto eléctrico?<svg class="chev shrink-0 text-sun-600" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="m6 9 6 6 6-6"/></svg></button>
        <div class="faq-body px-6 text-brand-700/85 leading-relaxed"><p class="pb-6">Claro. Diseñamos pensando en crecimiento: dejamos espacio en el inversor o usamos microinversores para agregar paneles después. Además instalamos cargadores nivel 2 para vehículos eléctricos.</p></div>
      </div>
    </div>
  </div>
</section>

<!-- ================= CONTACTO (final) ================= -->
<section id="contacto" class="py-24 hero-bg text-white relative overflow-hidden">
  <div class="absolute inset-0 grid-pattern pointer-events-none"></div>
  <div class="max-w-7xl mx-auto px-5 sm:px-8 relative">
    <div class="grid lg:grid-cols-2 gap-12 items-center">
      <div class="reveal">
        <p class="text-sun-400 font-semibold tracking-wider text-sm uppercase">Contáctanos</p>
        <h2 class="font-display font-extrabold text-3xl sm:text-4xl lg:text-5xl mt-3 tracking-tight">Hablemos de tu proyecto solar.</h2>
        <p class="mt-5 text-brand-100/85 text-lg leading-relaxed">Visita técnica y propuesta sin costo en Querétaro y área metropolitana. Respondemos en menos de 2 horas en horario laboral.</p>
        <div class="mt-8 space-y-4 text-brand-100">
          <div class="flex items-start gap-3">
            <svg class="mt-1 text-sun-400 shrink-0" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 10c0 6-8 12-8 12s-8-6-8-12a8 8 0 0 1 16 0z"/><circle cx="12" cy="10" r="3"/></svg>
            <p>Av. Constituyentes 120, Col. Centro, Santiago de Querétaro, Qro. 76000</p>
          </div>
          <div class="flex items-start gap-3">
            <svg class="mt-1 text-sun-400 shrink-0" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><path d="M12 6v6l4 2"/></svg>
            <p>Lunes a viernes 9:00 – 18:00 · Sábados 9:00 – 14:00</p>
          </div>
        </div>
      </div>
      <div class="grid sm:grid-cols-3 lg:grid-cols-1 gap-4 reveal delay-2">
        <a href="https://wa.me/524423344713?text=Hola%20SHELDA%2C%20me%20interesa%20un%20sistema%20fotovoltaico.%20%C2%BFMe%20pueden%20asesorar%3F" target="_blank" rel="noopener" class="card-hover group flex items-center gap-5 bg-white/10 hover:bg-white/15 border border-white/15 rounded-2xl p-5">
          <div class="relative w-14 h-14 shrink-0 rounded-2xl wa-btn grid place-items-center text-white"><span class="ring-anim"></span>
            <svg width="26" height="26" viewBox="0 0 24 24" fill="currentColor"><path d="M20.5 3.5A11.9 11.9 0 0 0 12 0C5.4 0 .1 5.3.1 11.9c0 2.1.6 4.1 1.6 5.9L0 24l6.4-1.7a11.9 11.9 0 0 0 5.6 1.4c6.6 0 11.9-5.3 11.9-11.9 0-3.2-1.2-6.2-3.4-8.3zM12 21.8c-1.8 0-3.5-.5-5-1.4l-.4-.2-3.8 1 1-3.7-.2-.4A9.9 9.9 0 0 1 2.1 12C2.1 6.5 6.5 2 12 2c2.6 0 5.1 1 7 2.9a9.8 9.8 0 0 1 2.9 7c0 5.5-4.4 9.9-9.9 9.9zm5.4-7.4c-.3-.1-1.8-.9-2-1-.3-.1-.5-.1-.7.1-.2.3-.8 1-.9 1.2-.2.2-.3.2-.6.1-.3-.1-1.3-.5-2.4-1.5-.9-.8-1.5-1.8-1.7-2.1-.2-.3 0-.5.1-.6l.4-.5c.1-.2.2-.3.3-.5.1-.2 0-.4 0-.5l-.9-2.2c-.2-.6-.5-.5-.7-.5h-.6c-.2 0-.5.1-.8.4-.3.3-1 1-1 2.5s1.1 2.9 1.2 3.1c.1.2 2.1 3.2 5.1 4.5.7.3 1.3.5 1.7.6.7.2 1.4.2 1.9.1.6-.1 1.8-.7 2-1.4.2-.7.2-1.3.2-1.4-.1-.2-.3-.3-.6-.4z"/></svg>
          </div>
          <div><p class="text-xs uppercase tracking-wider text-brand-200">WhatsApp</p><p class="font-display font-bold text-lg">+52 442 123 4567</p><p class="text-xs text-brand-200/80">Respuesta inmediata</p></div>
          <svg class="ml-auto text-brand-200 group-hover:translate-x-1 transition" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
        </a>
        <a href="tel:+524422219667" class="card-hover group flex items-center gap-5 bg-white/10 hover:bg-white/15 border border-white/15 rounded-2xl p-5">
          <div class="w-14 h-14 shrink-0 rounded-2xl bg-gradient-to-br from-brand-400 to-brand-600 grid place-items-center text-white">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.9v3a2 2 0 0 1-2.2 2 19.8 19.8 0 0 1-8.6-3.1 19.5 19.5 0 0 1-6-6A19.8 19.8 0 0 1 2.1 4.2 2 2 0 0 1 4.1 2h3a2 2 0 0 1 2 1.7c.1.9.4 1.9.7 2.8a2 2 0 0 1-.5 2.1L8 9.9a16 16 0 0 0 6 6l1.3-1.3a2 2 0 0 1 2.1-.4c.9.3 1.8.6 2.8.7A2 2 0 0 1 22 16.9z"/></svg>
          </div>
          <div><p class="text-xs uppercase tracking-wider text-brand-200">Llámanos</p><p class="font-display font-bold text-lg">(442) 123 4567</p><p class="text-xs text-brand-200/80">Lun – Sáb en horario laboral</p></div>
          <svg class="ml-auto text-brand-200 group-hover:translate-x-1 transition" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
        </a>
        <a href="mailto:sheldaingenieria@gmail.com?subject=Cotizaci%C3%B3n%20sistema%20fotovoltaico" class="card-hover group flex items-center gap-5 bg-white/10 hover:bg-white/15 border border-white/15 rounded-2xl p-5">
          <div class="w-14 h-14 shrink-0 rounded-2xl bg-gradient-to-br from-sun-400 to-sun-600 grid place-items-center text-brand-950">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m2 7 10 7 10-7"/></svg>
          </div>
          <div><p class="text-xs uppercase tracking-wider text-brand-200">Correo</p><p class="font-display font-bold text-lg break-all">sheldaingenieria@gmail.com</p><p class="text-xs text-brand-200/80">Envíanos tu recibo y te cotizamos</p></div>
          <svg class="ml-auto text-brand-200 group-hover:translate-x-1 transition" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
        </a>
      </div>
    </div>
  </div>
</section>

<!-- ================= FOOTER ================= -->
<footer class="bg-brand-950 text-brand-200 border-t border-white/5">
  <div class="max-w-7xl mx-auto px-5 sm:px-8 py-12 grid md:grid-cols-3 gap-10">
    <div>
      <div class="flex items-center gap-3">
<img src="LOGO SHELDA SF.png" alt="SHELDA" class="h-12 w-auto">
        <span class="font-display font-extrabold text-white text-xl tracking-[.14em]">SHELDA</span>
      </div>
      <p class="mt-4 text-sm leading-relaxed text-brand-200/80">Sistemas fotovoltaicos en Querétaro desde 2012. Venta, instalación y mantenimiento con ingeniería certificada.</p>
    </div>
    <div>
      <p class="font-display font-bold text-white">Navegación</p>
      <ul class="mt-4 space-y-2 text-sm">
        <li><a class="hover:text-white" href="#servicios">Servicios</a></li>
        <li><a class="hover:text-white" href="#porque">Por qué SHELDA</a></li>
        <li><a class="hover:text-white" href="#calculadora">Calculadora solar</a></li>
        <li><a class="hover:text-white" href="#proyectos">Proyectos</a></li>
        <li><a class="hover:text-white" href="#faq">Preguntas frecuentes</a></li>
      </ul>
    </div>
    <div>
      <p class="font-display font-bold text-white">Contacto</p>
      <ul class="mt-4 space-y-2 text-sm">
        <li><a class="hover:text-white" href="https://wa.me/524423344713" target="_blank" rel="noopener">WhatsApp: +52 442 123 4567</a></li>
        <li><a class="hover:text-white" href="tel:+524422219667">Tel: (442) 123 4567</a></li>
        <li><a class="hover:text-white" href="mailto:sheldaingenieria@gmail.com">sheldaingenieria@gmail.com</a></li>
        <li class="text-brand-200/70">Santiago de Querétaro, Qro.</li>
      </ul>
    </div>
  </div>
  <div class="border-t border-white/5">
    <div class="max-w-7xl mx-auto px-5 sm:px-8 py-5 flex flex-col sm:flex-row items-center justify-between gap-3 text-xs text-brand-200/60">
      <p>© <span id="year"></span> SHELDA Energía Solar. Todos los derechos reservados.</p>
      <p>Sitio de demostración · Estimaciones orientativas, no constituyen una cotización.</p>
    </div>
  </div>
</footer>

<script>
(function(){
  /* ---------- Config ---------- */
const CFG = { hsp: 5.6, perf: 0.80, panelW: 720, panelArea: 3.5, co2: 0.438, wa: '524422219667', treesPerTon: 46 };  const $ = s => document.querySelector(s);
  const $$ = s => Array.from(document.querySelectorAll(s));
  const fmt = (n, d=0) => n.toLocaleString('es-MX',{minimumFractionDigits:d, maximumFractionDigits:d});

  document.getElementById('year').textContent = new Date().getFullYear();

  /* ---------- Panel cells ---------- */
  const cells = $('#panelCells');
  for (let i=0;i<36;i++){ const c=document.createElement('div'); c.className='cell aspect-[4/5]'; cells.appendChild(c); }

  /* ---------- Live kW ticker ---------- */
  const liveKw = $('#liveKw'), liveBar = $('#liveBar');
  setInterval(()=>{ const v = 4.4 + Math.random()*0.9; liveKw.textContent = v.toFixed(2); liveBar.style.width = (v/6.2*100).toFixed(0)+'%'; }, 1800);

  /* ---------- Nav ---------- */
  const nav = $('#navInner'), menuBtn = $('#menuBtn'), mobileMenu = $('#mobileMenu');
  window.addEventListener('scroll', ()=>{ nav.classList.toggle('shadow-2xl', window.scrollY > 20); nav.classList.toggle('bg-brand-950/90', window.scrollY > 20); }, {passive:true});
  menuBtn.addEventListener('click', ()=> mobileMenu.classList.toggle('hidden'));
  $$('#mobileMenu a').forEach(a=>a.addEventListener('click', ()=> mobileMenu.classList.add('hidden')));

  // Scroll spy
  const sections = ['servicios','porque','proceso','calculadora','proyectos','faq'].map(id=>document.getElementById(id));
  const links = $$('.nav-link');
  const spy = new IntersectionObserver(entries=>{
    entries.forEach(e=>{ if(e.isIntersecting){ links.forEach(l=>l.classList.toggle('active', l.getAttribute('href')==='#'+e.target.id)); } });
  }, {rootMargin:'-40% 0px -55% 0px'});
  sections.forEach(s=>spy.observe(s));

  /* ---------- Reveal on scroll ---------- */
  const io = new IntersectionObserver(entries=>{
    entries.forEach(e=>{ if(e.isIntersecting){ e.target.classList.add('in'); io.unobserve(e.target);
      e.target.querySelectorAll('.counter').forEach(animateCounter);
      e.target.querySelectorAll('.barfill').forEach(b=> setTimeout(()=> b.style.width = b.dataset.w, 200));
      if(e.target.classList.contains('counter')) animateCounter(e.target);
    }});
  }, {threshold:.15});
  $$('.reveal').forEach(el=>io.observe(el));

  function animateCounter(el){
    if(el.dataset.done) return; el.dataset.done = 1;
    const to = parseFloat(el.dataset.to), dec = parseInt(el.dataset.dec||0), dur = 1600, t0 = performance.now();
    (function tick(t){ const p = Math.min(1,(t-t0)/dur), e = 1-Math.pow(1-p,3); el.textContent = fmt(to*e, dec); if(p<1) requestAnimationFrame(tick); })(t0);
  }

  /* ---------- FAQ ---------- */
  $$('.faq-btn').forEach(b=> b.addEventListener('click', ()=>{
    const item = b.parentElement, open = item.classList.contains('open');
    $$('.faq').forEach(f=>f.classList.remove('open'));
    if(!open) item.classList.add('open');
  }));

  /* ---------- Calculator ---------- */
  let activeTab = 'recibo', period = 2;
  const state = { evCount:1, phevCount:0, acCount:2 };

  // Tabs
  $$('.tab-btn').forEach(b=> b.addEventListener('click', ()=>{
    $$('.tab-btn').forEach(x=>x.classList.remove('active')); b.classList.add('active');
    activeTab = b.dataset.tab;
    $$('.tab-panel').forEach(p=>p.classList.add('hidden'));
    $('#tab-'+activeTab).classList.remove('hidden');
    calc();
  }));

  // Period
  $$('.period-btn').forEach(b=> b.addEventListener('click', ()=>{
    $$('.period-btn').forEach(x=>{ x.classList.remove('bg-brand-900','text-white'); x.classList.add('text-brand-700'); });
    b.classList.add('bg-brand-900','text-white'); b.classList.remove('text-brand-700');
    period = parseInt(b.dataset.period);
    const r = $('#billRange');
    if(period===1){ r.min=250; r.max=15000; } else { r.min=500; r.max=30000; }
    syncRange(r);
    calc();
  }));

  // Sliders
  function syncRange(r){ const p = (r.value - r.min)/(r.max - r.min)*100; r.style.setProperty('--p', p+'%'); }
  const billAmount = $('#billAmount'), billRange = $('#billRange');
  billRange.addEventListener('input', ()=>{ billAmount.value = billRange.value; syncRange(billRange); calc(); });
  billAmount.addEventListener('input', ()=>{ billRange.value = Math.min(Math.max(billAmount.value, billRange.min), billRange.max); syncRange(billRange); calc(); });
  const acHours = $('#acHours');
  acHours.addEventListener('input', ()=>{ $('#acHoursLbl').textContent = acHours.value; syncRange(acHours); calc(); });
  syncRange(billRange); syncRange(acHours);

  // Steppers
  $$('.stepper button').forEach(b=> b.addEventListener('click', ()=>{
    const k = b.dataset.target, max = k==='acCount' ? 12 : 6;
    state[k] = Math.min(max, Math.max(0, state[k] + parseInt(b.dataset.step)));
    const el = document.getElementById(k); el.textContent = state[k];
    el.classList.add('bump'); setTimeout(()=>el.classList.remove('bump'), 200);
    calc();
  }));

  ['tariff','coverage','homeBase','acTons','hasPool','hasHeater'].forEach(id=> document.getElementById(id).addEventListener('change', calc));

  function setNum(id, val){ const el = document.getElementById(id); if(el.textContent!==val){ el.textContent = val; el.classList.add('bump'); setTimeout(()=>el.classList.remove('bump'),200); } }

  function calc(){
    let kwhMonth, price, detail = '';
    if(activeTab==='recibo'){
      const amount = Math.max(0, parseFloat(billAmount.value)||0);
      const tOpt = $('#tariff').selectedOptions[0];
      price = parseFloat(tOpt.dataset.price);
      const coverage = parseFloat($('#coverage').value);
      const monthlyPay = period===2 ? amount/2 : amount;
      kwhMonth = (monthlyPay / price) * coverage;
      detail = `• Método: Recibo de CFE\n• Pago ${period===2?'bimestral':'mensual'}: $${fmt(amount)} MXN\n• Tarifa: ${tOpt.textContent.trim()}\n• Cobertura deseada: ${Math.round(coverage*100)}%`;
    } else {
      const base = parseFloat($('#homeBase').value);
      const acKw = parseFloat($('#acTons').value), hrs = parseFloat(acHours.value);
      const daily = state.evCount*9 + state.phevCount*4 + state.acCount*acKw*hrs*0.7 /*ciclo compresor*/ + ($('#hasPool').checked?6:0) + ($('#hasHeater').checked?5:0);
      kwhMonth = base + daily*30.4;
      price = kwhMonth > 500 ? 6.9 : (kwhMonth > 250 ? 4.2 : 3.1);
      if(base>=1200) price = 5.7;
      detail = `• Método: Autos y equipos\n• Consumo base: ${$('#homeBase').selectedOptions[0].textContent.trim()}\n• Autos eléctricos: ${state.evCount}\n• Híbridos enchufables: ${state.phevCount}\n• Aires acondicionados: ${state.acCount} × ${$('#acTons').selectedOptions[0].textContent.trim()} (${hrs} h/día)` + ($('#hasPool').checked?'\n• Bomba de alberca: sí':'') + ($('#hasHeater').checked?'\n• Calentador eléctrico: sí':'');
    }

    const dailyKwh = kwhMonth/30.4;
    let kwp = dailyKwh / (CFG.hsp * CFG.perf);
    let panels = Math.max(1, Math.ceil(kwp*1000/CFG.panelW));
    kwp = panels*CFG.panelW/1000;
    const area = panels*CFG.panelArea;
    const genYear = kwp*CFG.hsp*365*CFG.perf;
    const saveYear = Math.min(genYear, kwhMonth*12) * price;
    const co2 = genYear*CFG.co2/1000;
    const trees = Math.round(co2*CFG.treesPerTon);

    setNum('rKwp', fmt(kwp, kwp<10?2:1));
    setNum('rKwhMonth', fmt(kwhMonth));
    setNum('rPanels', fmt(panels));
    setNum('rArea', fmt(area));
    setNum('rGen', fmt(genYear));
    setNum('rSave', fmt(saveYear));
    setNum('rCo2', fmt(co2,1));
    setNum('rTrees', fmt(trees));

    const tag = $('#sysTag');
    tag.textContent = kwp < 10 ? 'Residencial' : kwp < 30 ? 'Residencial Plus' : kwp < 100 ? 'Comercial' : 'Industrial';

    const msg = `Hola SHELDA 👋, calculé mi sistema solar en su página web:\n\n${detail}\n\n☀️ *Resultados:*\n• Consumo estimado: ${fmt(kwhMonth)} kWh/mes\n• Sistema recomendado: *${fmt(kwp,2)} kWp* (${panels} paneles de ${CFG.panelW} W)\n• Área aproximada: ${fmt(area)} m²\n• Generación anual: ${fmt(genYear)} kWh\n• Ahorro estimado: $${fmt(saveYear)} MXN/año\n\nMe gustaría recibir una cotización formal. ¡Gracias! 😊`;
    $('#waQuote').href = `https://wa.me/${CFG.wa}?text=${encodeURIComponent(msg)}`;
  }
  calc();
})();
</script>
</body>
</html>
