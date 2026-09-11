<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>SHELDA · Sistemas Fotovoltaicos en Querétaro | Venta, Instalación y Mantenimiento</title>
<meta name="description" content="SHELDA: 12 años de experiencia en energía solar en Querétaro. Diseño, venta, instalación y mantenimiento de sistemas fotovoltaicos residenciales y comerciales.">
<script src="https://cdn.tailwindcss.com"></script>
<script>
tailwind.config = {
  theme: {
    extend: {
      colors: {
        navy: {50:'#EFF6FF',100:'#DBEAFE',700:'#17395F',800:'#0F2745',900:'#0A1A2F',950:'#050E1C'},
        solar: {50:'#FFFBEB',100:'#FEF3C7',200:'#FDE68A',300:'#FCD34D',400:'#FBBF24',500:'#F59E0B',600:'#D97706',700:'#B45309'},
        eco: {400:'#34D399',500:'#10B981',600:'#059669'}
      },
      fontFamily: {
        sans: ['Inter','system-ui','-apple-system','Segoe UI','sans-serif'],
        display: ['Sora','Inter','system-ui','sans-serif']
      },
      boxShadow: {
        'soft': '0 10px 40px -12px rgba(10,26,47,0.18)',
        'card': '0 4px 24px -6px rgba(10,26,47,0.10)'
      }
    }
  }
}
</script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Sora:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
  html { scroll-behavior: smooth; }
  body { -webkit-font-smoothing: antialiased; text-rendering: optimizeLegibility; }
  section { scroll-margin-top: 110px; }

  /* Reveal animations */
  .reveal { opacity: 0; transform: translateY(26px); transition: opacity .8s cubic-bezier(.2,.7,.3,1), transform .8s cubic-bezier(.2,.7,.3,1); }
  .reveal.in { opacity: 1; transform: none; }

  /* Background grid */
  .grid-lines {
    background-image: linear-gradient(rgba(255,255,255,.06) 1px, transparent 1px),
                      linear-gradient(90deg, rgba(255,255,255,.06) 1px, transparent 1px);
    background-size: 58px 58px;
    mask-image: radial-gradient(ellipse at 50% 0%, #000 20%, transparent 78%);
    -webkit-mask-image: radial-gradient(ellipse at 50% 0%, #000 20%, transparent 78%);
  }
  .grid-lines-light {
    background-image: linear-gradient(rgba(10,26,47,.045) 1px, transparent 1px),
                      linear-gradient(90deg, rgba(10,26,47,.045) 1px, transparent 1px);
    background-size: 48px 48px;
  }

  /* Glow blobs */
  .glow { position: absolute; border-radius: 9999px; filter: blur(100px); pointer-events: none; }

  /* Floating */
  @keyframes floaty { 0%,100% { transform: translateY(0) } 50% { transform: translateY(-14px) } }
  .floaty { animation: floaty 6.5s ease-in-out infinite; }

  /* Solar panel sheen */
  .panel-cell { position: relative; overflow: hidden; }
  .panel-cell::after {
    content: ''; position: absolute; inset: 0;
    background: linear-gradient(115deg, transparent 32%, rgba(255,255,255,.42) 50%, transparent 68%);
    transform: translateX(-130%);
    animation: sheen 5s ease-in-out infinite;
  }
  @keyframes sheen { 0% { transform: translateX(-130%);} 55%,100% { transform: translateX(130%);} }

  /* Range sliders */
  input[type="range"] {
    -webkit-appearance: none; appearance: none;
    width: 100%; height: 6px; border-radius: 999px;
    background: #E2E8F0; outline: none; cursor: pointer;
  }
  input[type="range"]::-webkit-slider-thumb {
    -webkit-appearance: none; appearance: none;
    width: 22px; height: 22px; border-radius: 50%;
    background: linear-gradient(145deg,#FBBF24,#D97706);
    border: 3px solid #fff;
    box-shadow: 0 2px 10px rgba(217,119,6,.55);
    cursor: pointer;
    transition: transform .15s ease;
  }
  input[type="range"]::-webkit-slider-thumb:hover { transform: scale(1.12); }
  input[type="range"]::-moz-range-thumb {
    width: 16px; height: 16px; border-radius: 50%;
    background: #F59E0B; border: 3px solid #fff;
    box-shadow: 0 2px 10px rgba(217,119,6,.55); cursor: pointer;
  }

  /* WhatsApp pulse */
  @keyframes pulseRing {
    0% { box-shadow: 0 0 0 0 rgba(37,211,102,.6); }
    70% { box-shadow: 0 0 0 18px rgba(37,211,102,0); }
    100% { box-shadow: 0 0 0 0 rgba(37,211,102,0); }
  }
  .wa-pulse { animation: pulseRing 2.4s infinite; }

  .tab-active { background: linear-gradient(135deg,#0A1A2F,#17395F); color: #fff; box-shadow: 0 10px 30px -10px rgba(10,26,47,.6); }

  .text-gradient {
    background: linear-gradient(100deg,#FBBF24 0%,#F59E0B 45%,#FCD34D 100%);
    -webkit-background-clip: text; background-clip: text; color: transparent;
  }

  ::selection { background: #FCD34D; color: #0A1A2F; }

  /* Custom scrollbar */
  ::-webkit-scrollbar { width: 11px; }
  ::-webkit-scrollbar-track { background: #F1F5F9; }
  ::-webkit-scrollbar-thumb { background: #94A3B8; border-radius: 99px; border: 3px solid #F1F5F9; }
  ::-webkit-scrollbar-thumb:hover { background: #64748B; }
</style>
</head>
<body class="font-sans bg-white text-navy-900 antialiased">

<!-- ================= HEADER ================= -->
<header class="fixed top-0 inset-x-0 z-50">
  <div class="mx-auto max-w-7xl px-4 sm:px-6">
    <nav class="mt-3 sm:mt-4 flex items-center justify-between rounded-2xl border border-white/10 bg-navy-900/75 px-4 sm:px-5 py-3 backdrop-blur-xl shadow-lg shadow-black/25">
      <a href="#inicio" class="flex items-center gap-3 group">
        <span class="relative grid h-10 w-10 place-items-center rounded-xl bg-gradient-to-br from-solar-400 to-solar-600 shadow-lg shadow-solar-600/30">
          <svg viewBox="0 0 24 24" class="h-6 w-6 text-navy-950" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round">
            <circle cx="12" cy="12" r="4" fill="currentColor" stroke="none"/>
            <path d="M12 2v2M12 20v2M4.9 4.9l1.4 1.4M17.7 17.7l1.4 1.4M2 12h2M20 12h2M4.9 19.1l1.4-1.4M17.7 6.3l1.4-1.4"/>
          </svg>
        </span>
        <span class="leading-none">
          <span class="block font-display text-lg font-extrabold tracking-tight text-white">SHELDA</span>
          <span class="block text-[10px] font-semibold uppercase tracking-[0.18em] text-solar-400/90">Energía Solar · QRO</span>
        </span>
      </a>

      <div class="hidden items-center gap-1 lg:flex">
        <a href="#servicios" class="rounded-lg px-4 py-2 text-sm font-medium text-slate-300 transition hover:bg-white/5 hover:text-white">Servicios</a>
        <a href="#nosotros" class="rounded-lg px-4 py-2 text-sm font-medium text-slate-300 transition hover:bg-white/5 hover:text-white">Nosotros</a>
        <a href="#calculadora" class="rounded-lg px-4 py-2 text-sm font-medium text-slate-300 transition hover:bg-white/5 hover:text-white">Calculadora</a>
        <a href="#proceso" class="rounded-lg px-4 py-2 text-sm font-medium text-slate-300 transition hover:bg-white/5 hover:text-white">Proceso</a>
        <a href="#contacto" class="rounded-lg px-4 py-2 text-sm font-medium text-slate-300 transition hover:bg-white/5 hover:text-white">Contacto</a>
      </div>

      <div class="flex items-center gap-2">
        <a href="https://wa.me/524421234567?text=Hola%20SHELDA%2C%20me%20interesa%20cotizar%20un%20sistema%20fotovoltaico." target="_blank" rel="noopener"
           class="hidden items-center gap-2 rounded-xl bg-gradient-to-r from-solar-400 to-solar-500 px-4 py-2.5 text-sm font-bold text-navy-950 shadow-lg shadow-solar-500/25 transition hover:brightness-105 hover:shadow-solar-500/40 sm:inline-flex">
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M17.47 14.38c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.48-.89-.79-1.48-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.13-.13.3-.35.44-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.08-.15-.67-1.62-.92-2.21-.24-.58-.49-.5-.67-.51-.17-.01-.37-.01-.57-.01-.2 0-.52.07-.79.37-.27.3-1.04 1.02-1.04 2.48 0 1.46 1.07 2.88 1.22 3.08.15.2 2.1 3.2 5.08 4.49.71.31 1.26.49 1.69.62.71.23 1.36.2 1.87.12.57-.08 1.76-.72 2.01-1.41.25-.7.25-1.29.17-1.42-.07-.13-.27-.2-.57-.35z"/><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.46 1.32 4.96L2 22l5.25-1.38a9.86 9.86 0 004.79 1.22h.01c5.46 0 9.9-4.45 9.9-9.91 0-2.65-1.03-5.14-2.9-7.01A9.82 9.82 0 0012.04 2zm0 18.13h-.01a8.2 8.2 0 01-4.18-1.14l-.3-.18-3.11.82.83-3.04-.2-.31a8.17 8.17 0 01-1.26-4.37c0-4.54 3.7-8.23 8.24-8.23a8.2 8.2 0 015.82 2.41 8.16 8.16 0 012.41 5.83c0 4.54-3.7 8.21-8.24 8.21z"/></svg>
          WhatsApp
        </a>
        <button id="menuBtn" aria-label="Menú" class="grid h-10 w-10 place-items-center rounded-xl border border-white/10 bg-white/5 text-white transition hover:bg-white/10 lg:hidden">
          <svg id="menuIcon" viewBox="0 0 24 24" class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round">
            <path d="M4 7h16M4 12h16M4 17h16"/>
          </svg>
        </button>
      </div>
    </nav>

    <!-- Mobile menu -->
    <div id="mobileMenu" class="hidden lg:hidden mt-2 rounded-2xl border border-white/10 bg-navy-900/95 p-3 backdrop-blur-xl shadow-2xl">
      <a href="#servicios" class="mobile-link block rounded-xl px-4 py-3 text-sm font-medium text-slate-200 transition hover:bg-white/10">Servicios</a>
      <a href="#nosotros" class="mobile-link block rounded-xl px-4 py-3 text-sm font-medium text-slate-200 transition hover:bg-white/10">Nosotros</a>
      <a href="#calculadora" class="mobile-link block rounded-xl px-4 py-3 text-sm font-medium text-slate-200 transition hover:bg-white/10">Calculadora Solar</a>
      <a href="#proceso" class="mobile-link block rounded-xl px-4 py-3 text-sm font-medium text-slate-200 transition hover:bg-white/10">Proceso</a>
      <a href="#contacto" class="mobile-link block rounded-xl px-4 py-3 text-sm font-medium text-slate-200 transition hover:bg-white/10">Contacto</a>
      <a href="https://wa.me/524421234567?text=Hola%20SHELDA%2C%20me%20interesa%20cotizar%20un%20sistema%20fotovoltaico." target="_blank" rel="noopener"
         class="mt-2 flex items-center justify-center gap-2 rounded-xl bg-gradient-to-r from-solar-400 to-solar-500 px-4 py-3 text-sm font-bold text-navy-950">
        Escríbenos por WhatsApp
      </a>
    </div>
  </div>
</header>

<!-- ================= HERO ================= -->
<section id="inicio" class="relative overflow-hidden bg-navy-950 pt-32 pb-20 lg:pt-44 lg:pb-28">
  <div class="absolute inset-0 grid-lines opacity-70"></div>
  <div class="glow h-[520px] w-[520px] bg-solar-500/25 -top-44 -right-24"></div>
  <div class="glow h-[420px] w-[420px] bg-eco-500/15 top-56 -left-40"></div>
  <div class="glow h-[300px] w-[300px] bg-blue-600/20 bottom-0 right-1/3"></div>

  <div class="relative mx-auto max-w-7xl px-5 sm:px-6">
    <div class="grid items-center gap-14 lg:grid-cols-[1.05fr_0.95fr] lg:gap-10">
      <!-- Copy -->
      <div class="reveal">
        <span class="inline-flex items-center gap-2 rounded-full border border-solar-400/30 bg-solar-400/10 px-4 py-1.5 text-xs font-semibold uppercase tracking-[0.14em] text-solar-300">
          <span class="relative flex h-2 w-2">
            <span class="absolute inline-flex h-full w-full animate-ping rounded-full bg-solar-400 opacity-75"></span>
            <span class="relative inline-flex h-2 w-2 rounded-full bg-solar-400"></span>
          </span>
          12 años iluminando Querétaro
        </span>

        <h1 class="mt-6 font-display text-4xl font-extrabold leading-[1.08] tracking-tight text-white sm:text-5xl lg:text-[3.55rem]">
          Energía solar que
          <span class="text-gradient"> trabaja para ti</span>, no al revés.
        </h1>

        <p class="mt-6 max-w-xl text-base leading-relaxed text-slate-300/90 sm:text-lg">
          Diseñamos, vendemos, instalamos y damos mantenimiento a sistemas fotovoltaicos en Querétaro.
          Ingeniería real, equipo certificado y trámites de interconexión con CFE incluidos.
        </p>

        <div class="mt-9 flex flex-col gap-3 sm:flex-row sm:items-center">
          <a href="#calculadora"
             class="inline-flex items-center justify-center gap-2 rounded-xl bg-gradient-to-r from-solar-400 to-solar-500 px-7 py-4 text-sm font-bold text-navy-950 shadow-xl shadow-solar-500/25 transition hover:-translate-y-0.5 hover:shadow-solar-500/45">
            <svg viewBox="0 0 24 24" class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M9 7h6M9 11h6M9 15h3"/><rect x="4" y="3" width="16" height="18" rx="2"/></svg>
            Calcular mi sistema
          </a>
          <a href="https://wa.me/524421234567?text=Hola%20SHELDA%2C%20me%20interesa%20una%20cotizaci%C3%B3n%20sin%20compromiso." target="_blank" rel="noopener"
             class="inline-flex items-center justify-center gap-2 rounded-xl border border-white/15 bg-white/5 px-7 py-4 text-sm font-semibold text-white backdrop-blur transition hover:border-white/30 hover:bg-white/10">
            <svg viewBox="0 0 24 24" class="h-5 w-5 text-eco-400" fill="currentColor"><path d="M17.47 14.38c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.48-.89-.79-1.48-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.13-.13.3-.35.44-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.08-.15-.67-1.62-.92-2.21-.24-.58-.49-.5-.67-.51-.17-.01-.37-.01-.57-.01-.2 0-.52.07-.79.37-.27.3-1.04 1.02-1.04 2.48 0 1.46 1.07 2.88 1.22 3.08.15.2 2.1 3.2 5.08 4.49.71.31 1.26.49 1.69.62.71.23 1.36.2 1.87.12.57-.08 1.76-.72 2.01-1.41.25-.7.25-1.29.17-1.42-.07-.13-.27-.2-.57-.35z"/><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.46 1.32 4.96L2 22l5.25-1.38a9.86 9.86 0 004.79 1.22h.01c5.46 0 9.9-4.45 9.9-9.91 0-2.65-1.03-5.14-2.9-7.01A9.82 9.82 0 0012.04 2zm0 18.13h-.01a8.2 8.2 0 01-4.18-1.14l-.3-.18-3.11.82.83-3.04-.2-.31a8.17 8.17 0 01-1.26-4.37c0-4.54 3.7-8.23 8.24-8.23a8.2 8.2 0 015.82 2.41 8.16 8.16 0 012.41 5.83c0 4.54-3.7 8.21-8.24 8.21z"/></svg>
            Hablar con un asesor
          </a>
        </div>

        <div class="mt-12 grid max-w-lg grid-cols-3 gap-6 border-t border-white/10 pt-8">
          <div>
            <div class="font-display text-3xl font-extrabold text-white">12<span class="text-solar-400">+</span></div>
            <div class="mt-1 text-xs font-medium uppercase tracking-wider text-slate-400">Años de experiencia</div>
          </div>
          <div>
            <div class="font-display text-3xl font-extrabold text-white">800<span class="text-solar-400">+</span></div>
            <div class="mt-1 text-xs font-medium uppercase tracking-wider text-slate-400">Proyectos instalados</div>
          </div>
          <div>
            <div class="font-display text-3xl font-extrabold text-white">25<span class="text-solar-400"> años</span></div>
            <div class="mt-1 text-xs font-medium uppercase tracking-wider text-slate-400">Garantía paneles</div>
          </div>
        </div>
      </div>

      <!-- Visual -->
      <div class="reveal relative" style="transition-delay:.15s">
        <div class="relative rounded-3xl border border-white/12 bg-white/[0.04] p-5 backdrop-blur-xl shadow-2xl shadow-black/40 sm:p-7">
          <div class="flex items-center justify-between">
            <div>
              <p class="text-xs font-semibold uppercase tracking-[0.16em] text-solar-400">Sistema residencial</p>
              <p class="mt-1 font-display text-xl font-bold text-white">Arreglo fotovoltaico 6.6 kW</p>
            </div>
            <span class="rounded-full border border-eco-500/30 bg-eco-500/10 px-3 py-1 text-[11px] font-bold text-eco-400">EN LÍNEA</span>
          </div>

          <!-- Panel array -->
          <div class="mt-6 grid grid-cols-4 gap-2.5 sm:gap-3">
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:0s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:.25s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:.5s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:.75s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:.99s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:1.24s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:1.49s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:1.74s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:1.99s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:2.24s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:2.49s"></div>
            <div class="panel-cell aspect-[4/3] rounded-lg border border-white/15 bg-gradient-to-br from-[#1E3A8A] via-[#132A54] to-[#0B1F3A]" style="animation-delay:2.74s"></div>
          </div>

          <div class="mt-6 grid grid-cols-3 gap-3">
            <div class="rounded-xl border border-white/10 bg-white/[0.04] p-3.5 text-center">
              <div class="font-display text-lg font-bold text-white" id="heroMetric1">28.4</div>
              <div class="text-[10px] font-medium uppercase tracking-wider text-slate-400">kWh hoy</div>
            </div>
            <div class="rounded-xl border border-white/10 bg-white/[0.04] p-3.5 text-center">
              <div class="font-display text-lg font-bold text-white">96<span class="text-solar-400">%</span></div>
              <div class="text-[10px] font-medium uppercase tracking-wider text-slate-400">Eficiencia</div>
            </div>
            <div class="rounded-xl border border-white/10 bg-white/[0.04] p-3.5 text-center">
              <div class="font-display text-lg font-bold text-eco-400">0.0 t</div>
              <div class="text-[10px] font-medium uppercase tracking-wider text-slate-400">CO₂ hoy</div>
            </div>
          </div>
        </div>

        <!-- Floating badge -->
        <div class="floaty absolute -bottom-6 -left-4 hidden items-center gap-3 rounded-2xl border border-white/12 bg-navy-900/90 px-5 py-3.5 backdrop-blur-xl shadow-2xl sm:flex">
          <span class="grid h-10 w-10 place-items-center rounded-xl bg-eco-500/15">
            <svg viewBox="0 0 24 24" class="h-5 w-5 text-eco-400" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6L9 17l-5-5"/></svg>
          </span>
          <div>
            <p class="text-sm font-bold text-white">Interconexión CFE</p>
            <p class="text-xs text-slate-400">Trámite 100% incluido</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ================= TRUST BAR ================= -->
<section class="border-b border-slate-100 bg-white">
  <div class="mx-auto max-w-7xl px-5 sm:px-6">
    <div class="grid grid-cols-2 gap-y-8 py-10 sm:grid-cols-4 sm:py-12">
      <div class="reveal flex flex-col items-center text-center">
        <svg viewBox="0 0 24 24" class="h-7 w-7 text-solar-500" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
        <p class="mt-3 font-display text-sm font-bold text-navy-900">Ingeniería certificada</p>
        <p class="mt-1 text-xs leading-relaxed text-slate-500">Diseño avalado por ingenieros eléctricos titulados</p>
      </div>
      <div class="reveal flex flex-col items-center text-center" style="transition-delay:.08s">
        <svg viewBox="0 0 24 24" class="h-7 w-7 text-solar-500" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/><path d="M9 12l2 2 4-4"/></svg>
        <p class="mt-3 font-display text-sm font-bold text-navy-900">Garantía por escrito</p>
        <p class="mt-1 text-xs leading-relaxed text-slate-500">Cobertura en equipo, mano de obra y producción</p>
      </div>
      <div class="reveal flex flex-col items-center text-center" style="transition-delay:.16s">
        <svg viewBox="0 0 24 24" class="h-7 w-7 text-solar-500" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M3 21h18M5 21V7l7-4 7 4v14M9 21v-6h6v6"/></svg>
        <p class="mt-3 font-display text-sm font-bold text-navy-900">Mantenimiento local</p>
        <p class="mt-1 text-xs leading-relaxed text-slate-500">Equipo propio en Querétaro, respuesta en 48 h</p>
      </div>
      <div class="reveal flex flex-col items-center text-center" style="transition-delay:.24s">
        <svg viewBox="0 0 24 24" class="h-7 w-7 text-solar-500" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2v6M12 22v-6M4.9 4.9l4.2 4.2M19.1 19.1l-4.2-4.2M2 12h6M22 12h-6M4.9 19.1l4.2-4.2M19.1 4.9l-4.2 4.2"/></svg>
        <p class="mt-3 font-display text-sm font-bold text-navy-900">Monitoreo remoto</p>
        <p class="mt-1 text-xs leading-relaxed text-slate-500">Vigilamos tu generación desde el primer día</p>
      </div>
    </div>
  </div>
</section>

<!-- ================= SERVICIOS ================= -->
<section id="servicios" class="relative bg-slate-50 py-20 lg:py-28">
  <div class="absolute inset-0 grid-lines-light"></div>
  <div class="relative mx-auto max-w-7xl px-5 sm:px-6">
    <div class="reveal mx-auto max-w-2xl text-center">
      <span class="text-xs font-bold uppercase tracking-[0.2em] text-solar-600">Nuestros servicios</span>
      <h2 class="mt-3 font-display text-3xl font-extrabold tracking-tight text-navy-900 sm:text-4xl">
        Todo el ciclo de vida de tu sistema solar
      </h2>
      <p class="mt-4 text-base leading-relaxed text-slate-600">
        Desde el estudio energético hasta el mantenimiento a los 10 años. Un solo proveedor, una sola responsabilidad.
      </p>
    </div>

    <div class="mt-14 grid gap-6 md:grid-cols-2 lg:grid-cols-4">
      <!-- Card 1 -->
      <div class="reveal group relative overflow-hidden rounded-2xl border border-slate-200 bg-white p-7 shadow-card transition duration-300 hover:-translate-y-1.5 hover:border-solar-300 hover:shadow-soft">
        <div class="absolute -right-10 -top-10 h-32 w-32 rounded-full bg-solar-100/60 blur-2xl transition group-hover:bg-solar-200/70"></div>
        <div class="relative">
          <span class="grid h-12 w-12 place-items-center rounded-xl bg-gradient-to-br from-navy-800 to-navy-900 shadow-lg shadow-navy-900/20">
            <svg viewBox="0 0 24 24" class="h-6 w-6 text-solar-400" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18M3 15h18M9 3v18M15 3v18"/></svg>
          </span>
          <h3 class="mt-5 font-display text-lg font-bold text-navy-900">Venta de equipo</h3>
          <p class="mt-2.5 text-sm leading-relaxed text-slate-600">
            Paneles, inversores híbridos, microinversores y bancos de baterías de las marcas líderes del mercado, con factura y garantía.
          </p>
          <ul class="mt-5 space-y-2 text-sm text-slate-600">
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Paneles Tier 1</li>
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Respaldo con baterías</li>
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Asesoría de compra</li>
          </ul>
        </div>
      </div>

      <!-- Card 2 -->
      <div class="reveal group relative overflow-hidden rounded-2xl border border-slate-200 bg-white p-7 shadow-card transition duration-300 hover:-translate-y-1.5 hover:border-solar-300 hover:shadow-soft" style="transition-delay:.08s">
        <div class="absolute -right-10 -top-10 h-32 w-32 rounded-full bg-solar-100/60 blur-2xl transition group-hover:bg-solar-200/70"></div>
        <div class="relative">
          <span class="grid h-12 w-12 place-items-center rounded-xl bg-gradient-to-br from-navy-800 to-navy-900 shadow-lg shadow-navy-900/20">
            <svg viewBox="0 0 24 24" class="h-6 w-6 text-solar-400" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M14.7 6.3a1 1 0 000 1.4l1.6 1.6a1 1 0 001.4 0l3.77-3.77a6 6 0 01-7.94 7.94l-6.91 6.91a2.12 2.12 0 01-3-3l6.91-6.91a6 6 0 017.94-7.94l-3.76 3.76z"/></svg>
          </span>
          <h3 class="mt-5 font-display text-lg font-bold text-navy-900">Instalación</h3>
          <p class="mt-2.5 text-sm leading-relaxed text-slate-600">
            Montaje estructural, cableado, protecciones DC/AC y puesta en marcha. Cumplimos NOM-001-SEDE y las especificaciones de CFE.
          </p>
          <ul class="mt-5 space-y-2 text-sm text-slate-600">
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Estructura anticiclónica</li>
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Trámite CFE incluido</li>
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Pruebas y certificado</li>
          </ul>
        </div>
      </div>

      <!-- Card 3 -->
      <div class="reveal group relative overflow-hidden rounded-2xl border border-slate-200 bg-white p-7 shadow-card transition duration-300 hover:-translate-y-1.5 hover:border-solar-300 hover:shadow-soft" style="transition-delay:.16s">
        <div class="absolute -right-10 -top-10 h-32 w-32 rounded-full bg-solar-100/60 blur-2xl transition group-hover:bg-solar-200/70"></div>
        <div class="relative">
          <span class="grid h-12 w-12 place-items-center rounded-xl bg-gradient-to-br from-navy-800 to-navy-900 shadow-lg shadow-navy-900/20">
            <svg viewBox="0 0 24 24" class="h-6 w-6 text-solar-400" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22a7 7 0 007-7c0-2-1-3.9-3-5.5s-3.5-4-4-6.5c-.5 2.5-2 4.9-4 6.5S5 13 5 15a7 7 0 007 7z"/></svg>
          </span>
          <h3 class="mt-5 font-display text-lg font-bold text-navy-900">Mantenimiento</h3>
          <p class="mt-2.5 text-sm leading-relaxed text-slate-600">
            Limpieza profesional, termografía, revisión de strings, torque de conexiones y reporte de desempeño anual.
          </p>
          <ul class="mt-5 space-y-2 text-sm text-slate-600">
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Limpieza sin químicos</li>
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Inspección termográfica</li>
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Plan anual programado</li>
          </ul>
        </div>
      </div>

      <!-- Card 4 -->
      <div class="reveal group relative overflow-hidden rounded-2xl border border-slate-200 bg-white p-7 shadow-card transition duration-300 hover:-translate-y-1.5 hover:border-solar-300 hover:shadow-soft" style="transition-delay:.24s">
        <div class="absolute -right-10 -top-10 h-32 w-32 rounded-full bg-solar-100/60 blur-2xl transition group-hover:bg-solar-200/70"></div>
        <div class="relative">
          <span class="grid h-12 w-12 place-items-center rounded-xl bg-gradient-to-br from-navy-800 to-navy-900 shadow-lg shadow-navy-900/20">
            <svg viewBox="0 0 24 24" class="h-6 w-6 text-solar-400" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3v18h18"/><path d="M7 15l4-5 3.5 3.5L21 7"/></svg>
          </span>
          <h3 class="mt-5 font-display text-lg font-bold text-navy-900">Estudio energético</h3>
          <p class="mt-2.5 text-sm leading-relaxed text-slate-600">
            Analizamos tus 12 últimos recibos, curvas de carga y sombreado del sitio para dimensionar con precisión, sin sobredimensionar.
          </p>
          <ul class="mt-5 space-y-2 text-sm text-slate-600">
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Análisis de recibos CFE</li>
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Simulación de producción</li>
            <li class="flex items-start gap-2"><span class="mt-1.5 h-1.5 w-1.5 shrink-0 rounded-full bg-solar-500"></span>Retorno de inversión</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ================= NOSOTROS ================= -->
<section id="nosotros" class="relative overflow-hidden bg-navy-950 py-20 lg:py-28">
  <div class="glow h-[420px] w-[420px] bg-solar-500/15 -left-32 top-10"></div>
  <div class="glow h-[380px] w-[380px] bg-blue-600/15 -right-24 bottom-0"></div>

  <div class="relative mx-auto max-w-7xl px-5 sm:px-6">
    <div class="grid items-center gap-14 lg:grid-cols-2 lg:gap-16">
      <div class="reveal">
        <span class="text-xs font-bold uppercase tracking-[0.2em] text-solar-400">Quiénes somos</span>
        <h2 class="mt-3 font-display text-3xl font-extrabold leading-tight tracking-tight text-white sm:text-4xl">
          12 años haciendo las cosas bien, no solo rápido.
        </h2>
        <p class="mt-5 text-base leading-relaxed text-slate-300/90">
          SHELDA nació en Querétaro con una convicción simple: la energía solar no se vende, se calcula.
          Cada proyecto parte de un estudio real de consumo y generación, no de una promesa de venta.
        </p>
        <p class="mt-4 text-base leading-relaxed text-slate-300/90">
          En más de una década hemos ejecutado proyectos residenciales, comerciales e industriales en todo el
          Bajío, con equipo propio de instalación y un área técnica dedicada exclusivamente al mantenimiento.
        </p>

        <div class="mt-9 grid gap-4 sm:grid-cols-2">
          <div class="rounded-2xl border border-white/10 bg-white/[0.04] p-5">
            <div class="font-display text-2xl font-extrabold text-solar-400">100%</div>
            <p class="mt-1 text-sm font-medium text-white">Proyectos con trámite CFE concluido</p>
          </div>
          <div class="rounded-2xl border border-white/10 bg-white/[0.04] p-5">
            <div class="font-display text-2xl font-extrabold text-solar-400">48 h</div>
            <p class="mt-1 text-sm font-medium text-white">Tiempo de respuesta en servicio</p>
          </div>
          <div class="rounded-2xl border border-white/10 bg-white/[0.04] p-5">
            <div class="font-display text-2xl font-extrabold text-solar-400">25 años</div>
            <p class="mt-1 text-sm font-medium text-white">Garantía de producción en paneles</p>
          </div>
          <div class="rounded-2xl border border-white/10 bg-white/[0.04] p-5">
            <div class="font-display text-2xl font-extrabold text-solar-400">5 años</div>
            <p class="mt-1 text-sm font-medium text-white">Garantía en instalación y mano de obra</p>
          </div>
        </div>
      </div>

      <div class="reveal" style="transition-delay:.15s">
        <div class="relative rounded-3xl border border-white/10 bg-gradient-to-br from-white/[0.07] to-white/[0.02] p-7 backdrop-blur-xl shadow-2xl shadow-black/40">
          <h3 class="font-display text-lg font-bold text-white">Por qué nos eligen sobre la competencia</h3>
          <div class="mt-6 space-y-5">
            <div class="flex gap-4">
              <span class="grid h-9 w-9 shrink-0 place-items-center rounded-lg bg-eco-500/15 text-sm font-bold text-eco-400">01</span>
              <div>
                <p class="text-sm font-semibold text-white">Dimensionamos con datos, no con estimados</p>
                <p class="mt-1 text-sm leading-relaxed text-slate-400">Analizamos tus recibos y horarios de consumo para evitar que pagues por kW que no necesitas.</p>
              </div>
            </div>
            <div class="h-px bg-white/10"></div>
            <div class="flex gap-4">
              <span class="grid h-9 w-9 shrink-0 place-items-center rounded-lg bg-eco-500/15 text-sm font-bold text-eco-400">02</span>
              <div>
                <p class="text-sm font-semibold text-white">Instaladores propios, no subcontratados</p>
                <p class="mt-1 text-sm leading-relaxed text-slate-400">El mismo equipo que diseña es el que sube al techo. Control total de calidad y seguridad.</p>
              </div>
            </div>
            <div class="h-px bg-white/10"></div>
            <div class="flex gap-4">
              <span class="grid h-9 w-9 shrink-0 place-items-center rounded-lg bg-eco-500/15 text-sm font-bold text-eco-400">03</span>
              <div>
                <p class="text-sm font-semibold text-white">Monitoreo y mantenimiento de por vida</p>
                <p class="mt-1 text-sm leading-relaxed text-slate-400">No desaparecemos al terminar la obra. Revisamos tu generación y te avisamos si algo baja de rendimiento.</p>
              </div>
            </div>
            <div class="h-px bg-white/10"></div>
            <div class="flex gap-4">
              <span class="grid h-9 w-9 shrink-0 place-items-center rounded-lg bg-eco-500/15 text-sm font-bold text-eco-400">04</span>
              <div>
                <p class="text-sm font-semibold text-white">Presencia real en Querétaro</p>
                <p class="mt-1 text-sm leading-relaxed text-slate-400">Oficina y almacén local. Refacciones, respuesta técnica y soporte sin depender de terceros.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ================= CALCULADORA ================= -->
<section id="calculadora" class="relative bg-white py-20 lg:py-28">
  <div class="mx-auto max-w-7xl px-5 sm:px-6">
    <div class="reveal mx-auto max-w-2xl text-center">
      <span class="text-xs font-bold uppercase tracking-[0.2em] text-solar-600">Herramienta interactiva</span>
      <h2 class="mt-3 font-display text-3xl font-extrabold tracking-tight text-navy-900 sm:text-4xl">
        Calcula el tamaño de tu sistema solar
      </h2>
      <p class="mt-4 text-base leading-relaxed text-slate-600">
        Dos formas de dimensionar. Usa tu recibo de luz o suma tus equipos de alto consumo.
        Los resultados son un estimado y se confirman con nuestro estudio energético gratuito.
      </p>
    </div>

    <div class="mt-12 reveal">
      <!-- Tabs -->
      <div class="mx-auto flex max-w-2xl flex-col gap-2 rounded-2xl border border-slate-200 bg-slate-100 p-1.5 sm:flex-row">
        <button id="tabBtn1" data-tab="1"
          class="tab-active flex-1 rounded-xl px-5 py-3 text-sm font-bold transition-all duration-300">
          Por mi recibo de luz
        </button>
        <button id="tabBtn2" data-tab="2"
          class="flex-1 rounded-xl px-5 py-3 text-sm font-bold text-slate-600 transition-all duration-300 hover:text-navy-900">
          Por mis equipos y autos
        </button>
      </div>

      <!-- Panel 1 -->
      <div id="panel1" class="mt-8">
        <div class="grid gap-6 lg:grid-cols-[1.1fr_0.9fr]">
          <!-- Inputs -->
          <div class="rounded-3xl border border-slate-200 bg-slate-50/70 p-6 sm:p-8">
            <div class="flex items-center gap-3">
              <span class="grid h-10 w-10 place-items-center rounded-xl bg-navy-900 text-solar-400">
                <svg viewBox="0 0 24 24" class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18h6M10 22h4M12 2a7 7 0 00-4 12.7V17h8v-2.3A7 7 0 0012 2z"/></svg>
              </span>
              <div>
                <h3 class="font-display text-base font-bold text-navy-900">Datos de tu recibo CFE</h3>
                <p class="text-xs text-slate-500">Bimestral, como lo emite CFE en Querétaro</p>
              </div>
            </div>

            <div class="mt-8 space-y-8">
              <div>
                <div class="flex items-end justify-between">
                  <label for="billAmount" class="text-sm font-semibold text-navy-900">Monto promedio del recibo (bimestral)</label>
                  <span class="font-display text-lg font-extrabold text-solar-600" id="billAmountOut">$3,500</span>
                </div>
                <input id="billAmount" type="range" min="300" max="30000" step="100" value="3500" class="mt-4">
                <div class="mt-2 flex justify-between text-[11px] font-medium text-slate-400">
                  <span>$300</span><span>$30,000+</span>
                </div>
              </div>

              <div>
                <div class="flex items-end justify-between">
                  <label for="billRate" class="text-sm font-semibold text-navy-900">Costo promedio por kWh</label>
                  <span class="font-display text-lg font-extrabold text-solar-600" id="billRateOut">$3.50</span>
                </div>
                <input id="billRate" type="range" min="2.5" max="6.5" step="0.1" value="3.5" class="mt-4">
                <div class="mt-2 flex justify-between text-[11px] font-medium text-slate-400">
                  <span>$2.50 (tarifa 1)</span><span>$6.50 (DAC)</span>
                </div>
                <p class="mt-3 rounded-xl bg-white px-4 py-3 text-xs leading-relaxed text-slate-500 ring-1 ring-slate-200">
                  Consejo: si tu recibo trae la leyenda <strong class="text-navy-900">DAC</strong>, tu costo por kWh es el más alto y el ahorro solar es mayor.
                </p>
              </div>
            </div>
          </div>

          <!-- Results -->
          <div id="res1" class="relative overflow-hidden rounded-3xl bg-gradient-to-br from-navy-900 to-navy-950 p-6 shadow-2xl shadow-navy-900/25 sm:p-8">
            <div class="glow h-56 w-56 bg-solar-500/20 -right-16 -top-16"></div>
            <div class="relative">
              <p class="text-xs font-bold uppercase tracking-[0.18em] text-solar-400">Sistema recomendado</p>
              <div class="mt-2 flex items-baseline gap-2">
                <span class="font-display text-5xl font-extrabold text-white" id="c1-kw">3.7</span>
                <span class="font-display text-2xl font-bold text-slate-400">kW</span>
              </div>
              <p class="mt-1 text-sm text-slate-400">Cobertura estimada del <span class="font-semibold text-white" id="c1-cover">100%</span> de tu consumo</p>

              <div class="mt-7 grid grid-cols-2 gap-3">
                <div class="rounded-xl border border-white/10 bg-white/[0.05] p-4">
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Paneles de 580 W</p>
                  <p class="mt-1 font-display text-xl font-bold text-white"><span id="c1-panels">7</span></p>
                </div>
                <div class="rounded-xl border border-white/10 bg-white/[0.05] p-4">
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Área de techo</p>
                  <p class="mt-1 font-display text-xl font-bold text-white"><span id="c1-area">16</span> m²</p>
                </div>
                <div class="rounded-xl border border-white/10 bg-white/[0.05] p-4">
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Generación mensual</p>
                  <p class="mt-1 font-display text-xl font-bold text-solar-400"><span id="c1-gen">500</span> kWh</p>
                </div>
                <div class="rounded-xl border border-white/10 bg-white/[0.05] p-4">
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Inversión estimada</p>
                  <p class="mt-1 font-display text-xl font-bold text-white"><span id="c1-cost">$70k</span></p>
                </div>
              </div>

              <div class="mt-6 space-y-3">
                <div>
                  <div class="mb-1.5 flex justify-between text-xs font-medium text-slate-400">
                    <span>Consumo mensual actual</span><span id="c1-consumoLbl" class="font-semibold text-white">500 kWh</span>
                  </div>
                  <div class="h-2.5 overflow-hidden rounded-full bg-white/10">
                    <div id="c1-barConsumo" class="h-full rounded-full bg-gradient-to-r from-slate-500 to-slate-400 transition-all duration-700" style="width:100%"></div>
                  </div>
                </div>
                <div>
                  <div class="mb-1.5 flex justify-between text-xs font-medium text-slate-400">
                    <span>Generación del sistema</span><span id="c1-genLbl" class="font-semibold text-solar-400">500 kWh</span>
                  </div>
                  <div class="h-2.5 overflow-hidden rounded-full bg-white/10">
                    <div id="c1-barGen" class="h-full rounded-full bg-gradient-to-r from-solar-500 to-solar-400 transition-all duration-700" style="width:100%"></div>
                  </div>
                </div>
              </div>

              <div class="mt-7 space-y-3 border-t border-white/10 pt-6 text-sm">
                <div class="flex items-center justify-between">
                  <span class="text-slate-400">Ahorro anual estimado</span>
                  <span class="font-display text-base font-bold text-eco-400" id="c1-ahorro">$21,000</span>
                </div>
                <div class="flex items-center justify-between">
                  <span class="text-slate-400">Retorno de inversión</span>
                  <span class="font-display text-base font-bold text-white" id="c1-payback">3.3 años</span>
                </div>
                <div class="flex items-center justify-between">
                  <span class="text-slate-400">CO₂ evitado al año</span>
                  <span class="font-display text-base font-bold text-white" id="c1-co2">2.6 t</span>
                </div>
              </div>

              <a href="https://wa.me/524421234567?text=Hola%20SHELDA%2C%20hice%20el%20c%C3%A1lculo%20con%20mi%20recibo%20de%20luz%20y%20quiero%20una%20cotizaci%C3%B3n." target="_blank" rel="noopener"
                 class="mt-7 flex w-full items-center justify-center gap-2 rounded-xl bg-gradient-to-r from-solar-400 to-solar-500 px-6 py-4 text-sm font-bold text-navy-950 shadow-lg shadow-solar-500/25 transition hover:brightness-105">
                Enviar mi resultado por WhatsApp
              </a>
            </div>
          </div>
        </div>
      </div>

      <!-- Panel 2 -->
      <div id="panel2" class="mt-8 hidden">
        <div class="grid gap-6 lg:grid-cols-[1.1fr_0.9fr]">
          <!-- Inputs -->
          <div class="rounded-3xl border border-slate-200 bg-slate-50/70 p-6 sm:p-8">
            <div class="flex items-center gap-3">
              <span class="grid h-10 w-10 place-items-center rounded-xl bg-navy-900 text-solar-400">
                <svg viewBox="0 0 24 24" class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M5 17h14M6 17v3M18 17v3M4 13h16M6 13V7a2 2 0 012-2h8a2 2 0 012 2v6"/><circle cx="9" cy="10" r="1"/><circle cx="15" cy="10" r="1"/></svg>
              </span>
              <div>
                <h3 class="font-display text-base font-bold text-navy-900">Tus equipos de alto consumo</h3>
                <p class="text-xs text-slate-500">Autos eléctricos, aires acondicionados y carga base</p>
              </div>
            </div>

            <div class="mt-8 space-y-8">
              <div>
                <div class="flex items-end justify-between">
                  <label for="baseKwh" class="text-sm font-semibold text-navy-900">Consumo base del hogar (mensual)</label>
                  <span class="font-display text-lg font-extrabold text-solar-600"><span id="baseKwhOut">350</span> kWh</span>
                </div>
                <input id="baseKwh" type="range" min="100" max="2500" step="25" value="350" class="mt-4">
                <div class="mt-2 flex justify-between text-[11px] font-medium text-slate-400">
                  <span>100 kWh</span><span>2,500 kWh</span>
                </div>
              </div>

              <div class="h-px bg-slate-200"></div>

              <div>
                <div class="flex items-end justify-between">
                  <label for="evCount" class="text-sm font-semibold text-navy-900">Autos eléctricos o híbridos enchufables</label>
                  <span class="font-display text-lg font-extrabold text-solar-600"><span id="evCountOut">0</span></span>
                </div>
                <input id="evCount" type="range" min="0" max="6" step="1" value="0" class="mt-4">
                <div class="mt-2 flex justify-between text-[11px] font-medium text-slate-400">
                  <span>0</span><span>6 vehículos</span>
                </div>
                <p class="mt-3 text-xs text-slate-500">Se estiman <strong class="text-navy-900">250 kWh al mes</strong> por vehículo cargando en casa (aprox. 1,500 km).</p>
              </div>

              <div class="h-px bg-slate-200"></div>

              <div>
                <div class="flex items-end justify-between">
                  <label for="acCount" class="text-sm font-semibold text-navy-900">Equipos de aire acondicionado</label>
                  <span class="font-display text-lg font-extrabold text-solar-600"><span id="acCountOut">2</span></span>
                </div>
                <input id="acCount" type="range" min="0" max="12" step="1" value="2" class="mt-4">
                <div class="mt-2 flex justify-between text-[11px] font-medium text-slate-400">
                  <span>0</span><span>12 equipos</span>
                </div>
              </div>

              <div class="grid gap-5 sm:grid-cols-2">
                <div>
                  <label for="acSize" class="text-sm font-semibold text-navy-900">Capacidad por equipo</label>
                  <select id="acSize" class="mt-3 w-full rounded-xl border border-slate-200 bg-white px-4 py-3 text-sm font-medium text-navy-900 outline-none transition focus:border-solar-400 focus:ring-2 focus:ring-solar-200">
                    <option value="1.1">1 tonelada (12,000 BTU)</option>
                    <option value="1.6" selected>1.5 toneladas (18,000 BTU)</option>
                    <option value="2.1">2 toneladas (24,000 BTU)</option>
                  </select>
                </div>
                <div>
                  <div class="flex items-end justify-between">
                    <label for="acHours" class="text-sm font-semibold text-navy-900">Horas de uso al día</label>
                    <span class="font-display text-base font-extrabold text-solar-600"><span id="acHoursOut">6</span> h</span>
                  </div>
                  <input id="acHours" type="range" min="1" max="16" step="1" value="6" class="mt-5">
                </div>
              </div>

              <p class="rounded-xl bg-white px-4 py-3 text-xs leading-relaxed text-slate-500 ring-1 ring-slate-200">
                El cálculo de aire acondicionado aplica un factor del 75% por modulación de equipos inverter y estacionalidad anual.
              </p>
            </div>
          </div>

          <!-- Results -->
          <div id="res2" class="relative overflow-hidden rounded-3xl bg-gradient-to-br from-navy-900 to-navy-950 p-6 shadow-2xl shadow-navy-900/25 sm:p-8">
            <div class="glow h-56 w-56 bg-eco-500/20 -right-16 -top-16"></div>
            <div class="relative">
              <p class="text-xs font-bold uppercase tracking-[0.18em] text-solar-400">Sistema recomendado</p>
              <div class="mt-2 flex items-baseline gap-2">
                <span class="font-display text-5xl font-extrabold text-white" id="c2-kw">7.6</span>
                <span class="font-display text-2xl font-bold text-slate-400">kW</span>
              </div>
              <p class="mt-1 text-sm text-slate-400">Consumo total estimado: <span class="font-semibold text-white" id="c2-totalLbl">1,032 kWh/mes</span></p>

              <div class="mt-7 grid grid-cols-2 gap-3">
                <div class="rounded-xl border border-white/10 bg-white/[0.05] p-4">
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Paneles de 580 W</p>
                  <p class="mt-1 font-display text-xl font-bold text-white"><span id="c2-panels">14</span></p>
                </div>
                <div class="rounded-xl border border-white/10 bg-white/[0.05] p-4">
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Área de techo</p>
                  <p class="mt-1 font-display text-xl font-bold text-white"><span id="c2-area">32</span> m²</p>
                </div>
                <div class="rounded-xl border border-white/10 bg-white/[0.05] p-4">
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Generación mensual</p>
                  <p class="mt-1 font-display text-xl font-bold text-solar-400"><span id="c2-gen">1,026</span> kWh</p>
                </div>
                <div class="rounded-xl border border-white/10 bg-white/[0.05] p-4">
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Inversión estimada</p>
                  <p class="mt-1 font-display text-xl font-bold text-white"><span id="c2-cost">$144k</span></p>
                </div>
              </div>

              <div class="mt-6 space-y-3">
                <div>
                  <div class="mb-1.5 flex justify-between text-xs font-medium text-slate-400">
                    <span>Consumo mensual total</span><span id="c2-consumoLbl" class="font-semibold text-white">1,032 kWh</span>
                  </div>
                  <div class="h-2.5 overflow-hidden rounded-full bg-white/10">
                    <div id="c2-barConsumo" class="h-full rounded-full bg-gradient-to-r from-slate-500 to-slate-400 transition-all duration-700" style="width:100%"></div>
                  </div>
                </div>
                <div>
                  <div class="mb-1.5 flex justify-between text-xs font-medium text-slate-400">
                    <span>Generación del sistema</span><span id="c2-genLbl" class="font-semibold text-solar-400">1,026 kWh</span>
                  </div>
                  <div class="h-2.5 overflow-hidden rounded-full bg-white/10">
                    <div id="c2-barGen" class="h-full rounded-full bg-gradient-to-r from-solar-500 to-solar-400 transition-all duration-700" style="width:100%"></div>
                  </div>
                </div>
              </div>

              <div class="mt-7 grid grid-cols-3 gap-3 border-t border-white/10 pt-6 text-center">
                <div>
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Base</p>
                  <p class="mt-1 font-display text-sm font-bold text-white"><span id="c2-base">350</span> kWh</p>
                </div>
                <div>
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Autos</p>
                  <p class="mt-1 font-display text-sm font-bold text-white"><span id="c2-ev">0</span> kWh</p>
                </div>
                <div>
                  <p class="text-[10px] font-bold uppercase tracking-wider text-slate-400">Aires</p>
                  <p class="mt-1 font-display text-sm font-bold text-white"><span id="c2-ac">432</span> kWh</p>
                </div>
              </div>

              <div class="mt-6 space-y-3 border-t border-white/10 pt-6 text-sm">
                <div class="flex items-center justify-between">
                  <span class="text-slate-400">Ahorro anual estimado</span>
                  <span class="font-display text-base font-bold text-eco-400" id="c2-ahorro">$43,000</span>
                </div>
                <div class="flex items-center justify-between">
                  <span class="text-slate-400">Retorno de inversión</span>
                  <span class="font-display text-base font-bold text-white" id="c2-payback">3.4 años</span>
                </div>
                <div class="flex items-center justify-between">
                  <span class="text-slate-400">CO₂ evitado al año</span>
                  <span class="font-display text-base font-bold text-white" id="c2-co2">5.4 t</span>
                </div>
              </div>

              <a href="https://wa.me/524421234567?text=Hola%20SHELDA%2C%20calcul%C3%A9%20mi%20sistema%20por%20equipos%20y%20autos%20el%C3%A9ctricos%20y%20quiero%20una%20cotizaci%C3%B3n." target="_blank" rel="noopener"
                 class="mt-7 flex w-full items-center justify-center gap-2 rounded-xl bg-gradient-to-r from-solar-400 to-solar-500 px-6 py-4 text-sm font-bold text-navy-950 shadow-lg shadow-solar-500/25 transition hover:brightness-105">
                Enviar mi resultado por WhatsApp
              </a>
            </div>
          </div>
        </div>
      </div>

      <p class="mt-8 text-center text-xs leading-relaxed text-slate-400">
        * Estimaciones basadas en 4.5 kWh por kW instalado al día (Irradiancia promedio de Querétaro) y un factor de rendimiento del 78%.
        El resultado final se confirma con nuestro estudio energético sin costo.
      </p>
    </div>
  </div>
</section>

<!-- ================= PROCESO ================= -->
<section id="proceso" class="relative overflow-hidden bg-slate-50 py-20 lg:py-28">
  <div class="absolute inset-0 grid-lines-light"></div>
  <div class="relative mx-auto max-w-7xl px-5 sm:px-6">
    <div class="reveal mx-auto max-w-2xl text-center">
      <span class="text-xs font-bold uppercase tracking-[0.2em] text-solar-600">Cómo trabajamos</span>
      <h2 class="mt-3 font-display text-3xl font-extrabold tracking-tight text-navy-900 sm:text-4xl">
        Un proceso claro, de principio a fin
      </h2>
      <p class="mt-4 text-base leading-relaxed text-slate-600">
        Sin sorpresas, sin letras chiquitas. Sabes exactamente qué pasa en cada etapa y cuánto tiempo toma.
      </p>
    </div>

    <div class="mt-16 grid gap-6 md:grid-cols-2 lg:grid-cols-4">
      <div class="reveal relative rounded-2xl border border-slate-200 bg-white p-7 shadow-card">
        <span class="absolute -top-4 left-7 grid h-9 w-9 place-items-center rounded-xl bg-gradient-to-br from-solar-400 to-solar-600 font-display text-sm font-extrabold text-navy-950 shadow-lg shadow-solar-500/30">1</span>
        <h3 class="mt-5 font-display text-base font-bold text-navy-900">Estudio energético</h3>
        <p class="mt-2 text-sm leading-relaxed text-slate-600">Revisamos tus recibos, medimos el sitio, evaluamos sombreado y definimos tu perfil de consumo real.</p>
        <p class="mt-4 text-xs font-semibold uppercase tracking-wider text-solar-600">Día 1 – 3</p>
      </div>
      <div class="reveal relative rounded-2xl border border-slate-200 bg-white p-7 shadow-card" style="transition-delay:.08s">
        <span class="absolute -top-4 left-7 grid h-9 w-9 place-items-center rounded-xl bg-gradient-to-br from-solar-400 to-solar-600 font-display text-sm font-extrabold text-navy-950 shadow-lg shadow-solar-500/30">2</span>
        <h3 class="mt-5 font-display text-base font-bold text-navy-900">Diseño e ingeniería</h3>
        <p class="mt-2 text-sm leading-relaxed text-slate-600">Entregamos planos, memoria de cálculo, diagrama unifilar y proyección de generación y retorno.</p>
        <p class="mt-4 text-xs font-semibold uppercase tracking-wider text-solar-600">Día 4 – 7</p>
      </div>
      <div class="reveal relative rounded-2xl border border-slate-200 bg-white p-7 shadow-card" style="transition-delay:.16s">
        <span class="absolute -top-4 left-7 grid h-9 w-9 place-items-center rounded-xl bg-gradient-to-br from-solar-400 to-solar-600 font-display text-sm font-extrabold text-navy-950 shadow-lg shadow-solar-500/30">3</span>
        <h3 class="mt-5 font-display text-base font-bold text-navy-900">Instalación y trámite</h3>
        <p class="mt-2 text-sm leading-relaxed text-slate-600">Montaje, protecciones, puesta en marcha y gestión completa de la interconexión ante CFE.</p>
        <p class="mt-4 text-xs font-semibold uppercase tracking-wider text-solar-600">Día 8 – 20</p>
      </div>
      <div class="reveal relative rounded-2xl border border-slate-200 bg-white p-7 shadow-card" style="transition-delay:.24s">
        <span class="absolute -top-4 left-7 grid h-9 w-9 place-items-center rounded-xl bg-gradient-to-br from-solar-400 to-solar-600 font-display text-sm font-extrabold text-navy-950 shadow-lg shadow-solar-500/30">4</span>
        <h3 class="mt-5 font-display text-base font-bold text-navy-900">Monitoreo y soporte</h3>
        <p class="mt-2 text-sm leading-relaxed text-slate-600">Activamos el monitoreo remoto, capacitamos al usuario y programamos el mantenimiento anual.</p>
        <p class="mt-4 text-xs font-semibold uppercase tracking-wider text-solar-600">Permanente</p>
      </div>
    </div>
  </div>
</section>

<!-- ================= TESTIMONIOS ================= -->
<section class="bg-white py-20 lg:py-28">
  <div class="mx-auto max-w-7xl px-5 sm:px-6">
    <div class="reveal mx-auto max-w-2xl text-center">
      <span class="text-xs font-bold uppercase tracking-[0.2em] text-solar-600">Clientes</span>
      <h2 class="mt-3 font-display text-3xl font-extrabold tracking-tight text-navy-900 sm:text-4xl">
        Lo que dicen en Querétaro
      </h2>
    </div>

    <div class="mt-14 grid gap-6 lg:grid-cols-3">
      <div class="reveal rounded-2xl border border-slate-200 bg-slate-50/70 p-7 shadow-card">
        <div class="flex gap-1 text-solar-500">
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
        </div>
        <p class="mt-5 text-sm leading-relaxed text-slate-700">
          "Nos explicaron todo con números, no con promesas. Pasamos de pagar $4,200 bimestrales a prácticamente cero.
          La instalación fue limpia y ordenada, dejaron el techo mejor de como estaba."
        </p>
        <div class="mt-6 flex items-center gap-3 border-t border-slate-200 pt-5">
          <span class="grid h-10 w-10 place-items-center rounded-full bg-navy-900 font-display text-sm font-bold text-solar-400">MR</span>
          <div>
            <p class="text-sm font-semibold text-navy-900">María Robles</p>
            <p class="text-xs text-slate-500">Casa residencial · Juriquilla</p>
          </div>
        </div>
      </div>

      <div class="reveal rounded-2xl border border-slate-200 bg-slate-50/70 p-7 shadow-card" style="transition-delay:.08s">
        <div class="flex gap-1 text-solar-500">
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
        </div>
        <p class="mt-5 text-sm leading-relaxed text-slate-700">
          "Tengo dos autos eléctricos y el recibo se me disparó. SHELDA dimensionó el sistema considerando la carga de los
          vehículos y las minisplits. El ahorro fue inmediato desde el primer bimestre."
        </p>
        <div class="mt-6 flex items-center gap-3 border-t border-slate-200 pt-5">
          <span class="grid h-10 w-10 place-items-center rounded-full bg-navy-900 font-display text-sm font-bold text-solar-400">JL</span>
          <div>
            <p class="text-sm font-semibold text-navy-900">Jorge Landa</p>
            <p class="text-xs text-slate-500">Residencial + 2 EV · El Marqués</p>
          </div>
        </div>
      </div>

      <div class="reveal rounded-2xl border border-slate-200 bg-slate-50/70 p-7 shadow-card" style="transition-delay:.16s">
        <div class="flex gap-1 text-solar-500">
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M12 2l2.4 7.4H22l-6 4.4 2.3 7.4-6.3-4.6L5.7 21.2 8 13.8l-6-4.4h7.6z"/></svg>
        </div>
        <p class="mt-5 text-sm leading-relaxed text-slate-700">
          "Llevamos 4 años con ellos. Instalaron en nuestra nave y ahora el contrato de mantenimiento anual
          nos ha mantenido la generación por encima del 97%. Muy profesionales."
        </p>
        <div class="mt-6 flex items-center gap-3 border-t border-slate-200 pt-5">
          <span class="grid h-10 w-10 place-items-center rounded-full bg-navy-900 font-display text-sm font-bold text-solar-400">CA</span>
          <div>
            <p class="text-sm font-semibold text-navy-900">Comercializadora Alver</p>
            <p class="text-xs text-slate-500">Sistema comercial · Parque Industrial QRO</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ================= CTA ================= -->
<section class="relative overflow-hidden bg-gradient-to-br from-solar-500 via-solar-500 to-solar-600 py-16 lg:py-20">
  <div class="absolute inset-0 opacity-20" style="background-image: radial-gradient(circle at 20% 30%, #fff 0, transparent 40%), radial-gradient(circle at 80% 70%, #fff 0, transparent 40%);"></div>
  <div class="relative mx-auto max-w-5xl px-5 text-center sm:px-6">
    <h2 class="font-display text-3xl font-extrabold leading-tight tracking-tight text-navy-950 sm:text-4xl">
      Tu recibo de luz no tiene por qué subir cada año.
    </h2>
    <p class="mx-auto mt-4 max-w-2xl text-base leading-relaxed text-navy-900/80">
      Agenda tu estudio energético gratuito. Visitamos tu propiedad en Querétaro y te entregamos una propuesta
      técnica con números reales, sin compromiso.
    </p>
    <div class="mt-9 flex flex-col justify-center gap-3 sm:flex-row">
      <a href="https://wa.me/524421234567?text=Hola%20SHELDA%2C%20quiero%20agendar%20un%20estudio%20energ%C3%A9tico%20gratuito." target="_blank" rel="noopener"
         class="inline-flex items-center justify-center gap-2 rounded-xl bg-navy-950 px-8 py-4 text-sm font-bold text-white shadow-xl shadow-navy-900/25 transition hover:-translate-y-0.5 hover:bg-navy-900">
        <svg viewBox="0 0 24 24" class="h-5 w-5 text-eco-400" fill="currentColor"><path d="M17.47 14.38c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.48-.89-.79-1.48-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.13-.13.3-.35.44-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.08-.15-.67-1.62-.92-2.21-.24-.58-.49-.5-.67-.51-.17-.01-.37-.01-.57-.01-.2 0-.52.07-.79.37-.27.3-1.04 1.02-1.04 2.48 0 1.46 1.07 2.88 1.22 3.08.15.2 2.1 3.2 5.08 4.49.71.31 1.26.49 1.69.62.71.23 1.36.2 1.87.12.57-.08 1.76-.72 2.01-1.41.25-.7.25-1.29.17-1.42-.07-.13-.27-.2-.57-.35z"/><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.46 1.32 4.96L2 22l5.25-1.38a9.86 9.86 0 004.79 1.22h.01c5.46 0 9.9-4.45 9.9-9.91 0-2.65-1.03-5.14-2.9-7.01A9.82 9.82 0 0012.04 2zm0 18.13h-.01a8.2 8.2 0 01-4.18-1.14l-.3-.18-3.11.82.83-3.04-.2-.31a8.17 8.17 0 01-1.26-4.37c0-4.54 3.7-8.23 8.24-8.23a8.2 8.2 0 015.82 2.41 8.16 8.16 0 012.41 5.83c0 4.54-3.7 8.21-8.24 8.21z"/></svg>
        Agendar por WhatsApp
      </a>
      <a href="tel:+524421234567"
         class="inline-flex items-center justify-center gap-2 rounded-xl border-2 border-navy-950/25 px-8 py-4 text-sm font-bold text-navy-950 transition hover:border-navy-950/60 hover:bg-navy-950/5">
        <svg viewBox="0 0 24 24" class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07 19.5 19.5 0 01-6-6A19.79 19.79 0 012.12 4.18 2 2 0 014.11 2h3a2 2 0 012 1.72c.13.96.36 1.9.7 2.81a2 2 0 01-.45 2.11L8.09 9.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45c.91.34 1.85.57 2.81.7A2 2 0 0122 16.92z"/></svg>
        Llamar ahora
      </a>
    </div>
  </div>
</section>

<!-- ================= CONTACTO ================= -->
<section id="contacto" class="bg-white py-20 lg:py-28">
  <div class="mx-auto max-w-7xl px-5 sm:px-6">
    <div class="reveal mx-auto max-w-2xl text-center">
      <span class="text-xs font-bold uppercase tracking-[0.2em] text-solar-600">Contacto</span>
      <h2 class="mt-3 font-display text-3xl font-extrabold tracking-tight text-navy-900 sm:text-4xl">
        Hablemos de tu proyecto
      </h2>
      <p class="mt-4 text-base leading-relaxed text-slate-600">
        Elige el canal que más te acomode. Respondemos en horario de oficina y agendamos visita técnica en Querétaro y zona metropolitana.
      </p>
    </div>

    <div class="mt-14 grid gap-6 lg:grid-cols-3">
      <!-- WhatsApp -->
      <a href="https://wa.me/524421234567?text=Hola%20SHELDA%2C%20me%20interesa%20cotizar%20un%20sistema%20fotovoltaico." target="_blank" rel="noopener"
         class="reveal group relative overflow-hidden rounded-2xl border border-slate-200 bg-white p-8 shadow-card transition duration-300 hover:-translate-y-1.5 hover:border-eco-500/40 hover:shadow-soft">
        <div class="absolute -right-12 -top-12 h-36 w-36 rounded-full bg-eco-500/10 blur-2xl transition group-hover:bg-eco-500/20"></div>
        <div class="relative">
          <span class="grid h-14 w-14 place-items-center rounded-2xl bg-gradient-to-br from-eco-500 to-eco-600 shadow-lg shadow-eco-600/25">
            <svg viewBox="0 0 24 24" class="h-7 w-7 text-white" fill="currentColor"><path d="M17.47 14.38c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.48-.89-.79-1.48-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.13-.13.3-.35.44-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.08-.15-.67-1.62-.92-2.21-.24-.58-.49-.5-.67-.51-.17-.01-.37-.01-.57-.01-.2 0-.52.07-.79.37-.27.3-1.04 1.02-1.04 2.48 0 1.46 1.07 2.88 1.22 3.08.15.2 2.1 3.2 5.08 4.49.71.31 1.26.49 1.69.62.71.23 1.36.2 1.87.12.57-.08 1.76-.72 2.01-1.41.25-.7.25-1.29.17-1.42-.07-.13-.27-.2-.57-.35z"/><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.46 1.32 4.96L2 22l5.25-1.38a9.86 9.86 0 004.79 1.22h.01c5.46 0 9.9-4.45 9.9-9.91 0-2.65-1.03-5.14-2.9-7.01A9.82 9.82 0 0012.04 2zm0 18.13h-.01a8.2 8.2 0 01-4.18-1.14l-.3-.18-3.11.82.83-3.04-.2-.31a8.17 8.17 0 01-1.26-4.37c0-4.54 3.7-8.23 8.24-8.23a8.2 8.2 0 015.82 2.41 8.16 8.16 0 012.41 5.83c0 4.54-3.7 8.21-8.24 8.21z"/></svg>
          </span>
          <h3 class="mt-6 font-display text-lg font-bold text-navy-900">WhatsApp</h3>
          <p class="mt-2 text-sm leading-relaxed text-slate-600">La vía más rápida. Enviamos cotización y fotografías de proyectos similares.</p>
          <p class="mt-5 font-display text-base font-bold text-eco-600">+52 442 123 4567</p>
          <span class="mt-4 inline-flex items-center gap-1.5 text-sm font-semibold text-navy-900">
            Abrir chat
            <svg viewBox="0 0 24 24" class="h-4 w-4 transition-transform group-hover:translate-x-1" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
          </span>
        </div>
      </a>

      <!-- Teléfono -->
      <a href="tel:+524421234567"
         class="reveal group relative overflow-hidden rounded-2xl border border-slate-200 bg-white p-8 shadow-card transition duration-300 hover:-translate-y-1.5 hover:border-solar-400/50 hover:shadow-soft" style="transition-delay:.08s">
        <div class="absolute -right-12 -top-12 h-36 w-36 rounded-full bg-solar-400/10 blur-2xl transition group-hover:bg-solar-400/25"></div>
        <div class="relative">
          <span class="grid h-14 w-14 place-items-center rounded-2xl bg-gradient-to-br from-solar-400 to-solar-600 shadow-lg shadow-solar-600/25">
            <svg viewBox="0 0 24 24" class="h-7 w-7 text-navy-950" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07 19.5 19.5 0 01-6-6A19.79 19.79 0 012.12 4.18 2 2 0 014.11 2h3a2 2 0 012 1.72c.13.96.36 1.9.7 2.81a2 2 0 01-.45 2.11L8.09 9.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45c.91.34 1.85.57 2.81.7A2 2 0 0122 16.92z"/></svg>
          </span>
          <h3 class="mt-6 font-display text-lg font-bold text-navy-900">Llamada directa</h3>
          <p class="mt-2 text-sm leading-relaxed text-slate-600">Atención personalizada de lunes a viernes de 9:00 a 18:00 h y sábados de 9:00 a 14:00 h.</p>
          <p class="mt-5 font-display text-base font-bold text-solar-600">+52 442 123 4567</p>
          <span class="mt-4 inline-flex items-center gap-1.5 text-sm font-semibold text-navy-900">
            Marcar ahora
            <svg viewBox="0 0 24 24" class="h-4 w-4 transition-transform group-hover:translate-x-1" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
          </span>
        </div>
      </a>

      <!-- Correo -->
      <a href="mailto:contacto@shelda.com.mx?subject=Cotizaci%C3%B3n%20de%20sistema%20fotovoltaico&body=Hola%20SHELDA%2C%20me%20interesa%20cotizar%20un%20sistema%20fotovoltaico.%0A%0ANombre%3A%0AUbicaci%C3%B3n%3A%0AConsumo%20promedio%20bimestral%3A"
         class="reveal group relative overflow-hidden rounded-2xl border border-slate-200 bg-white p-8 shadow-card transition duration-300 hover:-translate-y-1.5 hover:border-navy-700/40 hover:shadow-soft" style="transition-delay:.16s">
        <div class="absolute -right-12 -top-12 h-36 w-36 rounded-full bg-navy-700/10 blur-2xl transition group-hover:bg-navy-700/20"></div>
        <div class="relative">
          <span class="grid h-14 w-14 place-items-center rounded-2xl bg-gradient-to-br from-navy-800 to-navy-950 shadow-lg shadow-navy-900/25">
            <svg viewBox="0 0 24 24" class="h-7 w-7 text-solar-400" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M22 6l-10 7L2 6"/></svg>
          </span>
          <h3 class="mt-6 font-display text-lg font-bold text-navy-900">Correo electrónico</h3>
          <p class="mt-2 text-sm leading-relaxed text-slate-600">Para licitaciones, proyectos comerciales, facturación y documentación técnica.</p>
          <p class="mt-5 break-all font-display text-base font-bold text-navy-800">contacto@shelda.com.mx</p>
          <span class="mt-4 inline-flex items-center gap-1.5 text-sm font-semibold text-navy-900">
            Escribir correo
            <svg viewBox="0 0 24 24" class="h-4 w-4 transition-transform group-hover:translate-x-1" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
          </span>
        </div>
      </a>
    </div>

    <div class="reveal mt-8 grid gap-4 rounded-2xl border border-slate-200 bg-slate-50/70 p-6 sm:grid-cols-3 sm:p-8">
      <div class="flex items-start gap-3">
        <svg viewBox="0 0 24 24" class="mt-0.5 h-5 w-5 shrink-0 text-solar-600" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
        <div>
          <p class="text-sm font-semibold text-navy-900">Cobertura</p>
          <p class="mt-1 text-sm text-slate-600">Querétaro, Corregidora, El Marqués, Apaseo el Grande y todo el Bajío.</p>
        </div>
      </div>
      <div class="flex items-start gap-3">
        <svg viewBox="0 0 24 24" class="mt-0.5 h-5 w-5 shrink-0 text-solar-600" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><path d="M12 6v6l4 2"/></svg>
        <div>
          <p class="text-sm font-semibold text-navy-900">Horario</p>
          <p class="mt-1 text-sm text-slate-600">Lun – Vie 9:00 a 18:00 h · Sáb 9:00 a 14:00 h</p>
        </div>
      </div>
      <div class="flex items-start gap-3">
        <svg viewBox="0 0 24 24" class="mt-0.5 h-5 w-5 shrink-0 text-solar-600" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
        <div>
          <p class="text-sm font-semibold text-navy-900">Garantía</p>
          <p class="mt-1 text-sm text-slate-600">5 años en instalación y hasta 25 años en paneles, por escrito.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ================= FOOTER ================= -->
<footer class="bg-navy-950 pt-16 pb-8">
  <div class="mx-auto max-w-7xl px-5 sm:px-6">
    <div class="grid gap-10 pb-12 lg:grid-cols-[1.4fr_1fr_1fr_1fr]">
      <div>
        <div class="flex items-center gap-3">
          <span class="grid h-10 w-10 place-items-center rounded-xl bg-gradient-to-br from-solar-400 to-solar-600">
            <svg viewBox="0 0 24 24" class="h-6 w-6 text-navy-950" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round">
              <circle cx="12" cy="12" r="4" fill="currentColor" stroke="none"/>
              <path d="M12 2v2M12 20v2M4.9 4.9l1.4 1.4M17.7 17.7l1.4 1.4M2 12h2M20 12h2M4.9 19.1l1.4-1.4M17.7 6.3l1.4-1.4"/>
            </svg>
          </span>
          <div>
            <p class="font-display text-lg font-extrabold tracking-tight text-white">SHELDA</p>
            <p class="text-[10px] font-semibold uppercase tracking-[0.18em] text-solar-400/90">Sistemas Fotovoltaicos</p>
          </div>
        </div>
        <p class="mt-5 max-w-xs text-sm leading-relaxed text-slate-400">
          12 años diseñando, instalando y manteniendo sistemas solares en Querétaro.
          Ingeniería propia, resultados verificables.
        </p>
        <div class="mt-6 flex gap-3">
          <a href="https://wa.me/524421234567" target="_blank" rel="noopener" aria-label="WhatsApp"
             class="grid h-10 w-10 place-items-center rounded-xl border border-white/10 bg-white/5 text-slate-300 transition hover:border-eco-500/40 hover:bg-eco-500/10 hover:text-eco-400">
            <svg viewBox="0 0 24 24" class="h-4 w-4" fill="currentColor"><path d="M17.47 14.38c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.48-.89-.79-1.48-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.13-.13.3-.35.44-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.08-.15-.67-1.62-.92-2.21-.24-.58-.49-.5-.67-.51-.17-.01-.37-.01-.57-.01-.2 0-.52.07-.79.37-.27.3-1.04 1.02-1.04 2.48 0 1.46 1.07 2.88 1.22 3.08.15.2 2.1 3.2 5.08 4.49.71.31 1.26.49 1.69.62.71.23 1.36.2 1.87.12.57-.08 1.76-.72 2.01-1.41.25-.7.25-1.29.17-1.42-.07-.13-.27-.2-.57-.35z"/><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.46 1.32 4.96L2 22l5.25-1.38a9.86 9.86 0 004.79 1.22h.01c5.46 0 9.9-4.45 9.9-9.91 0-2.65-1.03-5.14-2.9-7.01A9.82 9.82 0 0012.04 2zm0 18.13h-.01a8.2 8.2 0 01-4.18-1.14l-.3-.18-3.11.82.83-3.04-.2-.31a8.17 8.17 0 01-1.26-4.37c0-4.54 3.7-8.23 8.24-8.23a8.2 8.2 0 015.82 2.41 8.16 8.16 0 012.41 5.83c0 4.54-3.7 8.21-8.24 8.21z"/></svg>
          </a>
          <a href="tel:+524421234567" aria-label="Teléfono"
             class="grid h-10 w-10 place-items-center rounded-xl border border-white/10 bg-white/5 text-slate-300 transition hover:border-solar-400/40 hover:bg-solar-400/10 hover:text-solar-400">
            <svg viewBox="0 0 24 24" class="h-4 w-4" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07 19.5 19.5 0 01-6-6A19.79 19.79 0 012.12 4.18 2 2 0 014.11 2h3a2 2 0 012 1.72c.13.96.36 1.9.7 2.81a2 2 0 01-.45 2.11L8.09 9.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45c.91.34 1.85.57 2.81.7A2 2 0 0122 16.92z"/></svg>
          </a>
          <a href="mailto:contacto@shelda.com.mx" aria-label="Correo"
             class="grid h-10 w-10 place-items-center rounded-xl border border-white/10 bg-white/5 text-slate-300 transition hover:border-solar-400/40 hover:bg-solar-400/10 hover:text-solar-400">
            <svg viewBox="0 0 24 24" class="h-4 w-4" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M22 6l-10 7L2 6"/></svg>
          </a>
        </div>
      </div>

      <div>
        <p class="font-display text-sm font-bold uppercase tracking-wider text-white">Servicios</p>
        <ul class="mt-5 space-y-3 text-sm text-slate-400">
          <li><a href="#servicios" class="transition hover:text-solar-400">Venta de equipo</a></li>
          <li><a href="#servicios" class="transition hover:text-solar-400">Instalación certificada</a></li>
          <li><a href="#servicios" class="transition hover:text-solar-400">Mantenimiento</a></li>
          <li><a href="#servicios" class="transition hover:text-solar-400">Estudio energético</a></li>
          <li><a href="#calculadora" class="transition hover:text-solar-400">Calculadora solar</a></li>
        </ul>
      </div>

      <div>
        <p class="font-display text-sm font-bold uppercase tracking-wider text-white">Empresa</p>
        <ul class="mt-5 space-y-3 text-sm text-slate-400">
          <li><a href="#nosotros" class="transition hover:text-solar-400">Sobre SHELDA</a></li>
          <li><a href="#proceso" class="transition hover:text-solar-400">Nuestro proceso</a></li>
          <li><a href="#contacto" class="transition hover:text-solar-400">Contacto</a></li>
          <li><a href="#inicio" class="transition hover:text-solar-400">Inicio</a></li>
        </ul>
      </div>

      <div>
        <p class="font-display text-sm font-bold uppercase tracking-wider text-white">Contacto</p>
        <ul class="mt-5 space-y-4 text-sm">
          <li>
            <a href="https://wa.me/524421234567" target="_blank" rel="noopener" class="flex items-start gap-2.5 text-slate-400 transition hover:text-eco-400">
              <svg viewBox="0 0 24 24" class="mt-0.5 h-4 w-4 shrink-0" fill="currentColor"><path d="M17.47 14.38c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.48-.89-.79-1.48-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.13-.13.3-.35.44-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.08-.15-.67-1.62-.92-2.21-.24-.58-.49-.5-.67-.51-.17-.01-.37-.01-.57-.01-.2 0-.52.07-.79.37-.27.3-1.04 1.02-1.04 2.48 0 1.46 1.07 2.88 1.22 3.08.15.2 2.1 3.2 5.08 4.49.71.31 1.26.49 1.69.62.71.23 1.36.2 1.87.12.57-.08 1.76-.72 2.01-1.41.25-.7.25-1.29.17-1.42-.07-.13-.27-.2-.57-.35z"/><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.46 1.32 4.96L2 22l5.25-1.38a9.86 9.86 0 004.79 1.22h.01c5.46 0 9.9-4.45 9.9-9.91 0-2.65-1.03-5.14-2.9-7.01A9.82 9.82 0 0012.04 2zm0 18.13h-.01a8.2 8.2 0 01-4.18-1.14l-.3-.18-3.11.82.83-3.04-.2-.31a8.17 8.17 0 01-1.26-4.37c0-4.54 3.7-8.23 8.24-8.23a8.2 8.2 0 015.82 2.41 8.16 8.16 0 012.41 5.83c0 4.54-3.7 8.21-8.24 8.21z"/></svg>
              <span>+52 442 123 4567</span>
            </a>
          </li>
          <li>
            <a href="tel:+524421234567" class="flex items-start gap-2.5 text-slate-400 transition hover:text-solar-400">
              <svg viewBox="0 0 24 24" class="mt-0.5 h-4 w-4 shrink-0" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07 19.5 19.5 0 01-6-6A19.79 19.79 0 012.12 4.18 2 2 0 014.11 2h3a2 2 0 012 1.72c.13.96.36 1.9.7 2.81a2 2 0 01-.45 2.11L8.09 9.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45c.91.34 1.85.57 2.81.7A2 2 0 0122 16.92z"/></svg>
              <span>Llamar: +52 442 123 4567</span>
            </a>
          </li>
          <li>
            <a href="mailto:contacto@shelda.com.mx" class="flex items-start gap-2.5 break-all text-slate-400 transition hover:text-solar-400">
              <svg viewBox="0 0 24 24" class="mt-0.5 h-4 w-4 shrink-0" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M22 6l-10 7L2 6"/></svg>
              <span>contacto@shelda.com.mx</span>
            </a>
          </li>
        </ul>
      </div>
    </div>

    <div class="flex flex-col items-center justify-between gap-4 border-t border-white/10 pt-8 sm:flex-row">
      <p class="text-xs text-slate-500">© <span id="year">2024</span> SHELDA Sistemas Fotovoltaicos. Todos los derechos reservados.</p>
      <p class="text-xs text-slate-600">Sitio demostrativo · Querétaro, México</p>
    </div>
  </div>
</footer>

<!-- ================= FLOATING WHATSAPP ================= -->
<a href="https://wa.me/524421234567?text=Hola%20SHELDA%2C%20me%20interesa%20cotizar%20un%20sistema%20fotovoltaico." target="_blank" rel="noopener" aria-label="WhatsApp"
   class="wa-pulse fixed bottom-5 right-5 z-50 grid h-14 w-14 place-items-center rounded-full bg-[#25D366] text-white shadow-2xl shadow-black/30 transition hover:scale-105">
  <svg viewBox="0 0 24 24" class="h-7 w-7" fill="currentColor"><path d="M17.47 14.38c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 1.17-.17.2-.35.22-.65.07-.3-.15-1.26-.46-2.4-1.48-.89-.79-1.48-1.77-1.66-2.07-.17-.3-.02-.46.13-.61.13-.13.3-.35.44-.52.15-.17.2-.3.3-.5.1-.2.05-.37-.02-.52-.08-.15-.67-1.62-.92-2.21-.24-.58-.49-.5-.67-.51-.17-.01-.37-.01-.57-.01-.2 0-.52.07-.79.37-.27.3-1.04 1.02-1.04 2.48 0 1.46 1.07 2.88 1.22 3.08.15.2 2.1 3.2 5.08 4.49.71.31 1.26.49 1.69.62.71.23 1.36.2 1.87.12.57-.08 1.76-.72 2.01-1.41.25-.7.25-1.29.17-1.42-.07-.13-.27-.2-.57-.35z"/><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.46 1.32 4.96L2 22l5.25-1.38a9.86 9.86 0 004.79 1.22h.01c5.46 0 9.9-4.45 9.9-9.91 0-2.65-1.03-5.14-2.9-7.01A9.82 9.82 0 0012.04 2zm0 18.13h-.01a8.2 8.2 0 01-4.18-1.14l-.3-.18-3.11.82.83-3.04-.2-.31a8.17 8.17 0 01-1.26-4.37c0-4.54 3.7-8.23 8.24-8.23a8.2 8.2 0 015.82 2.41 8.16 8.16 0 012.41 5.83c0 4.54-3.7 8.21-8.24 8.21z"/></svg>
</a>

<script>
(function () {
  'use strict';

  /* ============ Constantes técnicas ============ */
  const KWH_POR_KW_MES = 135;      // Querétaro: ~4.5 kWh/kW/día
  const POTENCIA_PANEL = 580;      // W
  const AREA_PANEL = 2.3;          // m²
  const COSTO_KW_MIN = 16000;      // MXN
  const COSTO_KW_MAX = 22000;      // MXN
  const CO2_KG_KWH = 0.435;        // Factor de emisión red eléctrica MX

  const mxn = new Intl.NumberFormat('es-MX', { style: 'currency', currency: 'MXN', maximumFractionDigits: 0 });
  const num = new Intl.NumberFormat('es-MX', { maximumFractionDigits: 0 });
  const num1 = new Intl.NumberFormat('es-MX', { minimumFractionDigits: 1, maximumFractionDigits: 1 });

  const $ = (id) => document.getElementById(id);

  /* ============ Menú móvil ============ */
  const menuBtn = $('menuBtn');
  const mobileMenu = $('mobileMenu');
  menuBtn.addEventListener('click', function () {
    mobileMenu.classList.toggle('hidden');
  });
  document.querySelectorAll('.mobile-link').forEach(function (a) {
    a.addEventListener('click', function () { mobileMenu.classList.add('hidden'); });
  });

  /* ============ Tabs calculadora ============ */
  const tabBtn1 = $('tabBtn1');
  const tabBtn2 = $('tabBtn2');
  const panel1 = $('panel1');
  const panel2 = $('panel2');

  function setTab(n) {
    const active = 'tab-active';
    const inactive = ['text-slate-600', 'hover:text-navy-900'];
    if (n === 1) {
      tabBtn1.classList.add(active);
      tabBtn1.classList.remove('text-slate-600', 'hover:text-navy-900');
      tabBtn2.classList.remove(active);
      tabBtn2.classList.add('text-slate-600', 'hover:text-navy-900');
      panel1.classList.remove('hidden');
      panel2.classList.add('hidden');
    } else {
      tabBtn2.classList.add(active);
      tabBtn2.classList.remove('text-slate-600', 'hover:text-navy-900');
      tabBtn1.classList.remove(active);
      tabBtn1.classList.add('text-slate-600', 'hover:text-navy-900');
      panel2.classList.remove('hidden');
      panel1.classList.add('hidden');
    }
  }
  tabBtn1.addEventListener('click', function () { setTab(1); });
  tabBtn2.addEventListener('click', function () { setTab(2); });

  /* ============ Calculadora 1: Recibo de luz ============ */
  const billAmount = $('billAmount');
  const billRate = $('billRate');

  function calcBill() {
    const montoBimestral = parseFloat(billAmount.value) || 0;
    const tarifa = parseFloat(billRate.value) || 3.5;

    $('billAmountOut').textContent = mxn.format(montoBimestral);
    $('billRateOut').textContent = '$' + num1.format(tarifa);

    const kwhBimestral = tarifa > 0 ? (montoBimestral / tarifa) : 0;
    const kwhMensual = kwhBimestral / 2;

    if (kwhMensual < 10) {
      $('c1-kw').textContent = '—';
      $('c1-panels').textContent = '—';
      $('c1-area').textContent = '—';
      $('c1-gen').textContent = '—';
      $('c1-cost').textContent = '—';
      $('c1-ahorro').textContent = '—';
      $('c1-payback').textContent = '—';
      $('c1-co2').textContent = '—';
      $('c1-consumoLbl').textContent = '0 kWh';
      $('c1-genLbl').textContent = '0 kWh';
      $('c1-barConsumo').style.width = '0%';
      $('c1-barGen').style.width = '0%';
      return;
    }

    let kw = kwhMensual / KWH_POR_KW_MES;
    kw = Math.round(kw * 10) / 10;
    if (kw < 0.5) kw = 0.5;

    const paneles = Math.ceil((kw * 1000) / POTENCIA_PANEL);
    const area = Math.round(paneles * AREA_PANEL);
    const generacionMensual = Math.round(kw * KWH_POR_KW_MES);
    const costoMin = kw * COSTO_KW_MIN;
    const costoMax = kw * COSTO_KW_MAX;
    const costoMedio = (costoMin + costoMax) / 2;

    const ahorroAnual = generacionMensual * 12 * tarifa;
    const payback = ahorroAnual > 0 ? (costoMedio / ahorroAnual) : 0;
    const co2 = (generacionMensual * 12 * CO2_KG_KWH) / 1000;

    const maxVal = Math.max(kwhMensual, generacionMensual, 1);

    $('c1-kw').textContent = num1.format(kw);
    $('c1-panels').textContent = paneles;
    $('c1-area').textContent = area;
    $('c1-gen').textContent = num.format(generacionMensual);
    $('c1-cost').textContent = '$' + num.format(costoMedio / 1000) + 'k';
    $('c1-ahorro').textContent = mxn.format(ahorroAnual);
    $('c1-payback').textContent = num1.format(payback) + ' años';
    $('c1-co2').textContent = num1.format(co2) + ' t';

    const cobertura = Math.min(100, Math.round((generacionMensual / kwhMensual) * 100));
    $('c1-cover').textContent = cobertura + '%';

    $('c1-consumoLbl').textContent = num.format(kwhMensual) + ' kWh';
    $('c1-genLbl').textContent = num.format(generacionMensual) + ' kWh';
    $('c1-barConsumo').style.width = Math.round((kwhMensual / maxVal) * 100) + '%';
    $('c1-barGen').style.width = Math.round((generacionMensual / maxVal) * 100) + '%';
  }

  billAmount.addEventListener('input', calcBill);
  billRate.addEventListener('input', calcBill);

  /* ============ Calculadora 2: Equipos y autos ============ */
  const baseKwh = $('baseKwh');
  const evCount = $('evCount');
  const acCount = $('acCount');
  const acSize = $('acSize');
  const acHours = $('acHours');

  const KWH_POR_EV_MES = 250;
  const FACTOR_AC = 0.75;

  function calcLoads() {
    const base = parseFloat(baseKwh.value) || 0;
    const evs = parseInt(evCount.value, 10) || 0;
    const aires = parseInt(acCount.value, 10) || 0;
    const potenciaAC = parseFloat(acSize.value) || 1.6;
    const horas = parseFloat(acHours.value) || 0;

    $('baseKwhOut').textContent = num.format(base);
    $('evCountOut').textContent = evs;
    $('acCountOut').textContent = aires;
    $('acHoursOut').textContent = horas;

    const kwhEV = evs * KWH_POR_EV_MES;
    const kwhAC = aires * potenciaAC * horas * 30 * FACTOR_AC;
    const total = base + kwhEV + kwhAC;

    if (total < 10) {
      $('c2-kw').textContent = '—';
      $('c2-panels').textContent = '—';
      $('c2-area').textContent = '—';
      $('c2-gen').textContent = '—';
      $('c2-cost').textContent = '—';
      $('c2-ahorro').textContent = '—';
      $('c2-payback').textContent = '—';
      $('c2-co2').textContent = '—';
      $('c2-totalLbl').textContent = '0 kWh/mes';
      $('c2-consumoLbl').textContent = '0 kWh';
      $('c2-genLbl').textContent = '0 kWh';
      $('c2-barConsumo').style.width = '0%';
      $('c2-barGen').style.width = '0%';
      return;
    }

    let kw = total / KWH_POR_KW_MES;
    kw = Math.round(kw * 10) / 10;
    if (kw < 0.5) kw = 0.5;

    const paneles = Math.ceil((kw * 1000) / POTENCIA_PANEL);
    const area = Math.round(paneles * AREA_PANEL);
    const generacionMensual = Math.round(kw * KWH_POR_KW_MES);
    const costoMin = kw * COSTO_KW_MIN;
    const costoMax = kw * COSTO_KW_MAX;
    const costoMedio = (costoMin + costoMax) / 2;

    const tarifaRef = 3.5;
    const ahorroAnual = generacionMensual * 12 * tarifaRef;
    const payback = ahorroAnual > 0 ? (costoMedio / ahorroAnual) : 0;
    const co2 = (generacionMensual * 12 * CO2_KG_KWH) / 1000;

    const maxVal = Math.max(total, generacionMensual, 1);

    $('c2-kw').textContent = num1.format(kw);
    $('c2-panels').textContent = paneles;
    $('c2-area').textContent = area;
    $('c2-gen').textContent = num.format(generacionMensual);
    $('c2-cost').textContent = '$' + num.format(costoMedio / 1000) + 'k';
    $('c2-ahorro').textContent = mxn.format(ahorroAnual);
    $('c2-payback').textContent = num1.format(payback) + ' años';
    $('c2-co2').textContent = num1.format(co2) + ' t';

    $('c2-totalLbl').textContent = num.format(total) + ' kWh/mes';
    $('c2-consumoLbl').textContent = num.format(total) + ' kWh';
    $('c2-genLbl').textContent = num.format(generacionMensual) + ' kWh';
    $('c2-base').textContent = num.format(base);
    $('c2-ev').textContent = num.format(kwhEV);
    $('c2-ac').textContent = num.format(Math.round(kwhAC));
    $('c2-barConsumo').style.width = Math.round((total / maxVal) * 100) + '%';
    $('c2-barGen').style.width = Math.round((generacionMensual / maxVal) * 100) + '%';
  }

  [baseKwh, evCount, acCount, acSize, acHours].forEach(function (el) {
    el.addEventListener('input', calcLoads);
    el.addEventListener('change', calcLoads);
  });

  /* ============ Reveal on scroll ============ */
  const revealEls = document.querySelectorAll('.reveal');
  if ('IntersectionObserver' in window) {
    const io = new IntersectionObserver(function (entries) {
      entries.forEach(function (entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('in');
          io.unobserve(entry.target);
        }
      });
    }, { threshold: 0.12, rootMargin: '0px 0px -40px 0px' });
    revealEls.forEach(function (el) { io.observe(el); });
  } else {
    revealEls.forEach(function (el) { el.classList.add('in'); });
  }

  /* ============ Header shadow on scroll ============ */
  const header = document.querySelector('header');
  window.addEventListener('scroll', function () {
    if (window.scrollY > 20) {
      header.classList.add('scrolled');
    } else {
      header.classList.remove('scrolled');
    }
  }, { passive: true });

  /* ============ Contador héroe ============ */
  const heroMetric = $('heroMetric1');
  if (heroMetric) {
    let baseVal = 28.4;
    setInterval(function () {
      baseVal = 26 + Math.random() * 6;
      heroMetric.textContent = num1.format(baseVal);
    }, 3200);
  }

  /* ============ Año dinámico ============ */
  $('year').textContent = new Date().getFullYear();

  /* ============ Inicialización ============ */
  calcBill();
  calcLoads();
})();
</script>
</body>
</html>
