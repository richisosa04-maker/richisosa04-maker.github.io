// Archivo: app/page.jsx (Next.js App Router)
// ✅ Versión SIN shadcn/ui ni librerías extra. Solo Tailwind + React.
// Copiá este contenido en app/page.jsx una vez que tengas Tailwind configurado.

const BUSINESS = {
  name: "EVEREST",
  slogan: "Tu confort en buenas manos",
  phoneE164: "5491123456789", // 54 + área sin 0 + número sin 15
  email: "contacto@everest.com.ar",
  city: "Zona Sur GBA",
};

const WHATSAPP_LINK = `https://wa.me/${BUSINESS.phoneE164}?text=${encodeURIComponent(
  "Hola, vengo desde la web. Me gustaría pedir un presupuesto para instalación/mantenimiento."
)}`;

const servicios = [
  { title: "Instalación de Aire Acondicionado", desc: "Montaje profesional y prolijo de minisplits hasta 6000 frigorías.", icon: "❄️" },
  { title: "Mantenimiento de Equipos", desc: "Limpieza integral, control de gas, vacío y chequeos de rendimiento.", icon: "🧰" },
  { title: "Instalaciones Eléctricas", desc: "Circuitos dedicados, térmicas, disyuntor y puesta a tierra.", icon: "⚡" },
];

const trabajos = [
  { title: "Instalación 3000 fg – Dormitorio", img: "https://images.unsplash.com/photo-1603715749720-901ac53c3e56?q=80&w=1200&auto=format&fit=crop" },
  { title: "Mantenimiento full – Living", img: "https://images.unsplash.com/photo-1598300183690-5b7b29f2c1b1?q=80&w=1200&auto=format&fit=crop" },
  { title: "Circuito dedicado + térmica", img: "https://images.unsplash.com/photo-1509395176047-4a66953fd231?q=80&w=1200&auto=format&fit=crop" },
];

export default function Page() {
  return (
    <div className="min-h-screen bg-white text-gray-800">
      {/* Header */}
      <header className="sticky top-0 z-40 w-full border-b bg-white/80 backdrop-blur">
        <div className="mx-auto flex h-16 max-w-6xl items-center justify-between px-4">
          <div className="flex items-center gap-2">
            <span className="inline-flex h-7 w-7 items-center justify-center rounded bg-blue-600 text-white">▲</span>
            <span className="font-extrabold tracking-widest">{BUSINESS.name}</span>
          </div>
          <nav className="hidden gap-6 md:flex text-sm font-medium">
            <a href="#servicios" className="hover:text-blue-600">Servicios</a>
            <a href="#portfolio" className="hover:text-blue-600">Trabajos</a>
            <a href="#por-que" className="hover:text-blue-600">Por qué</a>
            <a href="#contacto" className="hover:text-blue-600">Contacto</a>
          </nav>
          <a href={WHATSAPP_LINK} target="_blank" rel="noreferrer" className="rounded-2xl bg-blue-600 px-4 py-2 text-sm font-semibold text-white hover:bg-blue-700">
            Pedir presupuesto
          </a>
        </div>
      </header>

      {/* Hero */}
      <section className="relative">
        <div className="mx-auto grid max-w-6xl grid-cols-1 items-center gap-10 px-4 py-14 md:grid-cols-2">
          <div>
            <h1 className="text-4xl font-extrabold leading-tight md:text-5xl">
              Soluciones integrales en <span className="text-blue-600">climatización</span> y <span className="text-blue-600">electricidad</span>
            </h1>
            <p className="mt-4 text-gray-600">
              Instalación y mantenimiento de aire acondicionado. Circuitos eléctricos seguros para tu hogar o negocio en {BUSINESS.city}.
            </p>
            <div className="mt-6 flex flex-wrap gap-3">
              <a href={WHATSAPP_LINK} target="_blank" rel="noreferrer" className="rounded-2xl bg-blue-600 px-5 py-3 text-sm font-semibold text-white hover:bg-blue-700">Contactar por WhatsApp</a>
              <a href="#servicios" className="rounded-2xl border px-5 py-3 text-sm font-semibold hover:bg-gray-50">Ver servicios</a>
            </div>
            <div className="mt-3 text-xs text-gray-500">Atención Lun-Dom 8–20h</div>
          </div>
          <div>
            <img src="https://images.unsplash.com/photo-1598300183725-c9a28d88e55a?q=80&w=1200&auto=format&fit=crop" alt="Técnico instalando aire" className="h-[360px] w-full rounded-2xl object-cover shadow-xl" />
          </div>
        </div>
      </section>

      {/* Servicios */}
      <section id="servicios" className="bg-gray-50 py-14">
        <div className="mx-auto max-w-6xl px-4">
          <h2 className="text-center text-3xl font-bold">Servicios</h2>
          <p className="mx-auto mt-2 max-w-2xl text-center text-gray-600">Trabajo prolijo, herramientas profesionales y garantía escrita.</p>
          <div className="mt-8 grid grid-cols-1 gap-6 md:grid-cols-3">
            {servicios.map((s) => (
              <div key={s.title} className="rounded-2xl border bg-white p-6 shadow-sm">
                <div className="flex items-center gap-3 text-lg font-semibold">
                  <span className="inline-flex h-10 w-10 items-center justify-center rounded-full bg-blue-50 text-2xl">{s.icon}</span>
                  {s.title}
                </div>
                <p className="mt-3 text-sm text-gray-600">{s.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Por qué elegirnos */}
      <section id="por-que" className="py-14">
        <div className="mx-auto grid max-w-6xl grid-cols-1 items-center gap-10 px-4 md:grid-cols-2">
          <div>
            <h2 className="text-3xl font-bold">¿Por qué elegir {BUSINESS.name}?</h2>
            <ul className="mt-6 space-y-3 text-gray-700">
              <li className="flex gap-2"><span>✅</span><span>Presupuesto por WhatsApp en 5 minutos</span></li>
              <li className="flex gap-2"><span>✅</span><span>Garantía escrita y factura</span></li>
              <li className="flex gap-2"><span>✅</span><span>Herramental profesional (vacuum gauge, nitrógeno)</span></li>
              <li className="flex gap-2"><span>✅</span><span>Imagen prolija y seguridad en altura</span></li>
            </ul>
          </div>
          <div>
            <img src="https://images.unsplash.com/photo-1603715749720-901ac53c3e56?q=80&w=1200&auto=format&fit=crop" alt="Trabajo prolijo" className="h-[360px] w-full rounded-2xl object-cover shadow-xl" />
          </div>
        </div>
      </section>

      {/* Portfolio */}
      <section id="portfolio" className="bg-gray-50 py-14">
        <div className="mx-auto max-w-6xl px-4">
          <h2 className="text-center text-3xl font-bold">Portfolio</h2>
          <p className="mx-auto mt-2 max-w-2xl text-center text-gray-600">Algunos trabajos recientes.</p>
          <div className="mt-8 grid grid-cols-1 gap-6 md:grid-cols-3">
            {trabajos.map((t) => (
              <div key={t.title} className="overflow-hidden rounded-2xl border bg-white shadow-sm">
                <img src={t.img} alt={t.title} className="h-48 w-full object-cover" />
                <div className="p-4 text-base font-semibold">{t.title}</div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* CTA */}
      <section className="py-14">
        <div className="mx-auto max-w-6xl rounded-3xl bg-gradient-to-tr from-blue-50 to-white px-6 py-10 shadow-sm">
          <div className="flex flex-col items-center text-center">
            <h3 className="text-2xl font-bold">¿Listo para mejorar tu climatización?</h3>
            <p className="mt-2 max-w-2xl text-gray-600">Escribinos y te damos un estimado inmediato. Si compartís fotos del lugar, ajustamos el presupuesto antes de la visita.</p>
            <div className="mt-5 flex flex-wrap items-center justify-center gap-3">
              <a href={WHATSAPP_LINK} target="_blank" rel="noreferrer" className="rounded-2xl bg-blue-600 px-5 py-3 text-sm font-semibold text-white hover:bg-blue-700">Hablar por WhatsApp</a>
              <a href={`mailto:${BUSINESS.email}`} className="rounded-2xl border px-5 py-3 text-sm font-semibold hover:bg-gray-50">Enviar email</a>
            </div>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer id="contacto" className="border-t py-10">
        <div className="mx-auto max-w-6xl px-4">
          <div className="grid grid-cols-1 gap-8 md:grid-cols-3">
            <div>
              <div className="flex items-center gap-2">
                <span className="inline-flex h-7 w-7 items-center justify-center rounded bg-blue-600 text-white">▲</span>
                <span className="font-extrabold tracking-widest">{BUSINESS.name}</span>
              </div>
              <p className="mt-2 text-sm text-gray-600">{BUSINESS.slogan}</p>
            </div>
            <div>
              <h4 className="font-semibold">Contacto</h4>
              <ul className="mt-3 space-y-2 text-sm text-gray-600">
                <li><a className="hover:underline" href={WHATSAPP_LINK} target="_blank" rel="noreferrer">WhatsApp</a></li>
                <li><a className="hover:underline" href={`mailto:${BUSINESS.email}`}>{BUSINESS.email}</a></li>
                <li>{BUSINESS.city}</li>
              </ul>
            </div>
            <div>
              <h4 className="font-semibold">Links rápidos</h4>
              <ul className="mt-3 space-y-2 text-sm text-gray-600">
                <li><a className="hover:underline" href="#servicios">Servicios</a></li>
                <li><a className="hover:underline" href="#portfolio">Trabajos</a></li>
                <li><a className="hover:underline" href="#por-que">Por qué</a></li>
                <li><a className="hover:underline" href="#contacto">Contacto</a></li>
              </ul>
            </div>
          </div>
          <div className="mt-8 border-t pt-6 text-center text-xs text-gray-500">© {new Date().getFullYear()} {BUSINESS.name}. Todos los derechos reservados.</div>
        </div>
      </footer>
    </div>
  );
}
