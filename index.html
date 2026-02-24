import { useState } from "react";

const STYLES = {
  competir:    { label: "Competir",    color: "#ef4444", bg: "#fef2f2", postit: "🔴 ROJO",     emoji: "⚔️", desc: "Defiendes tus posiciones con claridad. Eres directo y asertivo ante el conflicto. Tu red te percibe como resolutivo, aunque a veces como poco flexible.", tip: "Úsalo cuando haya un límite ético claro. Evítalo cuando necesites que la otra persona colabore de forma sostenida." },
  colaborar:   { label: "Colaborar",   color: "#22c55e", bg: "#f0fdf4", postit: "🟢 VERDE",    emoji: "🤝", desc: "Buscas soluciones que funcionen para todos. Inviertes tiempo en entender la perspectiva del otro antes de actuar.", tip: "Es el estilo más poderoso a largo plazo, pero requiere tiempo y voluntad mutua. No siempre es posible en caliente." },
  comprometer: { label: "Comprometer", color: "#f59e0b", bg: "#fffbeb", postit: "🟡 AMARILLO", emoji: "⚖️", desc: "Buscas un punto medio razonable. Eres pragmático: algo cedes, algo ganas. Tu red te percibe como justo y equilibrado.", tip: "Ideal para disputas de honorarios o situaciones sin solución perfecta. Cuidado con usarlo como salida fácil cuando la situación requiere más profundidad." },
  evitar:      { label: "Evitar",      color: "#3b82f6", bg: "#eff6ff", postit: "🔵 AZUL",     emoji: "🚪", desc: "Prefieres no abordar el conflicto directamente. Esperas a que las cosas se calmen antes de actuar.", tip: "Útil cuando el momento no es el adecuado. Peligroso si se convierte en tu estilo por defecto — los conflictos ignorados se convierten en cultura." },
  acomodar:    { label: "Acomodar",    color: "#a855f7", bg: "#faf5ff", postit: "🟣 MORADO",   emoji: "🕊️", desc: "Cedes para preservar la relación. Priorizas la armonía del equipo sobre tener razón.", tip: "Válido cuando la relación vale más que el resultado puntual. Riesgo: el resentimiento acumulado acaba siendo más costoso que el conflicto original." },
};

const QUESTIONS = [
  { a: { text: "Prefiero hablar directamente sobre el problema y llegar a una solución que funcione para los dos.", style: "colaborar" }, b: { text: "Evito el conflicto si creo que con el tiempo se resolverá solo.", style: "evitar" } },
  { a: { text: "Cuando hay un desacuerdo, defiendo mi posición con claridad aunque genere tensión.", style: "competir" }, b: { text: "Intento encontrar un término medio que satisfaga a las dos partes.", style: "comprometer" } },
  { a: { text: "Si la otra persona tiene un punto válido, cedo con facilidad.", style: "acomodar" }, b: { text: "Prefiero buscar una solución que integre los intereses de los dos.", style: "colaborar" } },
  { a: { text: "En situaciones de conflicto, intento no tomar partido y mantenerme al margen.", style: "evitar" }, b: { text: "Dejo claro lo que espero y no me muevo hasta que se cumple.", style: "competir" } },
  { a: { text: "Me parece bien ceder en algo si la otra persona también cede.", style: "comprometer" }, b: { text: "Me siento mal si la relación queda dañada, aunque yo tuviera razón.", style: "acomodar" } },
  { a: { text: "Prefiero esperar el momento adecuado antes de abordar una situación difícil.", style: "evitar" }, b: { text: "Busco entender en profundidad la posición del otro antes de dar mi opinión.", style: "colaborar" } },
  { a: { text: "Cuando defiendo algo importante, no me importa que haya tensión temporal.", style: "competir" }, b: { text: "Me incomoda el conflicto abierto y prefiero suavizarlo.", style: "acomodar" } },
  { a: { text: "Ante una disputa, propongo dividir las diferencias a partes iguales.", style: "comprometer" }, b: { text: "Prefiero dejar pasar el tema antes que entrar en una discusión.", style: "evitar" } },
  { a: { text: "Priorizo mantener la relación aunque eso signifique no conseguir lo que quería.", style: "acomodar" }, b: { text: "Me aseguro de que mis intereses queden protegidos en cualquier acuerdo.", style: "competir" } },
  { a: { text: "Creo que la mejor solución se consigue cuando las dos partes exploran el problema juntas.", style: "colaborar" }, b: { text: "Acepto una solución intermedia para cerrar el tema.", style: "comprometer" } },
  { a: { text: "Cuando hay un conflicto, espero a que la otra persona dé el primer paso.", style: "evitar" }, b: { text: "Adapto mi posición si eso ayuda a mantener una buena relación.", style: "acomodar" } },
  { a: { text: "En una disputa, lo que más me importa es llegar a un acuerdo justo para los dos.", style: "comprometer" }, b: { text: "Prefiero afrontar los desacuerdos directamente y en el momento.", style: "colaborar" } },
  { a: { text: "Cuando creo que estoy en lo correcto, lo defiendo aunque genere fricción.", style: "competir" }, b: { text: "Si el tema no es crítico, prefiero no generar conflicto.", style: "evitar" } },
  { a: { text: "Me esfuerzo por entender las preocupaciones del otro aunque no las comparta.", style: "colaborar" }, b: { text: "Suelo ceder para no crear un ambiente tenso.", style: "acomodar" } },
  { a: { text: "Cuando hay desacuerdo, lo que quiero es que cada parte consiga algo.", style: "comprometer" }, b: { text: "Si hay algo en juego importante, no cedo aunque haya presión.", style: "competir" } },
];

export default function TKIApp() {
  const [screen, setScreen] = useState("intro");
  const [current, setCurrent] = useState(0);
  const [answers, setAnswers] = useState([]);
  const [scores, setScores] = useState(null);
  const [selected, setSelected] = useState(null);

  const handleAnswer = (style) => {
    setSelected(style);
    setTimeout(() => {
      const newAnswers = [...answers, style];
      if (current + 1 >= QUESTIONS.length) {
        const s = { competir: 0, colaborar: 0, comprometer: 0, evitar: 0, acomodar: 0 };
        newAnswers.forEach(st => s[st]++);
        setScores(s);
        setScreen("result");
      } else {
        setCurrent(c => c + 1);
        setAnswers(newAnswers);
        setSelected(null);
      }
    }, 350);
  };

  const restart = () => {
    setScreen("intro"); setCurrent(0); setAnswers([]); setScores(null); setSelected(null);
  };

  const dominant = scores ? Object.entries(scores).sort((a, b) => b[1] - a[1])[0][0] : null;
  const style = dominant ? STYLES[dominant] : null;
  const progress = (current / QUESTIONS.length) * 100;

  return (
    <div style={{ minHeight: "100vh", background: "#0f172a", display: "flex", alignItems: "center", justifyContent: "center", fontFamily: "'Segoe UI', sans-serif", padding: 16 }}>

      {/* ── INTRO ── */}
      {screen === "intro" && (
        <div style={{ maxWidth: 500, width: "100%", textAlign: "center" }}>
          <div style={{ fontSize: 56, marginBottom: 16 }}>🎯</div>
          <div style={{ color: "#e94560", fontSize: 11, fontWeight: 700, letterSpacing: 3, marginBottom: 10 }}>IAD · MANAGERS PLATINO</div>
          <h1 style={{ color: "white", fontSize: 30, fontWeight: 800, marginBottom: 14, lineHeight: 1.2 }}>
            ¿Cómo gestionas el conflicto<br />de forma natural?
          </h1>
          <p style={{ color: "#94a3b8", fontSize: 15, lineHeight: 1.8, marginBottom: 12 }}>
            Todos tenemos una forma instintiva de responder cuando aparece un conflicto. Ni buena ni mala — simplemente la nuestra.
          </p>
          <p style={{ color: "#64748b", fontSize: 14, lineHeight: 1.7, marginBottom: 36 }}>
            15 preguntas para descubrir tu estilo predominante.<br />
            <strong style={{ color: "#e2e8f0" }}>Responde según cómo actúas, no según cómo querrías actuar.</strong>
          </p>
          <button
            onClick={() => setScreen("test")}
            style={{ background: "#e94560", color: "white", border: "none", borderRadius: 14, padding: "16px 0", fontSize: 17, fontWeight: 700, cursor: "pointer", width: "100%", marginBottom: 12 }}
          >
            Descubrir mi estilo →
          </button>
          <p style={{ color: "#334155", fontSize: 12 }}>~4 minutos · Sin respuestas correctas ni incorrectas</p>
        </div>
      )}

      {/* ── TEST ── */}
      {screen === "test" && (
        <div style={{ maxWidth: 580, width: "100%" }}>
          <div style={{ marginBottom: 24 }}>
            <div style={{ display: "flex", justifyContent: "space-between", color: "#475569", fontSize: 12, marginBottom: 6 }}>
              <span>Pregunta {current + 1} de {QUESTIONS.length}</span>
              <span>{Math.round(progress)}%</span>
            </div>
            <div style={{ background: "#1e293b", borderRadius: 4, height: 5 }}>
              <div style={{ background: "#e94560", height: 5, borderRadius: 4, width: `${progress}%`, transition: "width 0.3s" }} />
            </div>
          </div>

          <div style={{ background: "#1e293b", borderRadius: 18, padding: "28px 24px" }}>
            <p style={{ color: "#64748b", fontSize: 13, marginBottom: 18 }}>¿Cuál de estas dos opciones te describe mejor?</p>
            <div style={{ display: "flex", flexDirection: "column", gap: 14 }}>
              {["a", "b"].map(opt => {
                const q = QUESTIONS[current][opt];
                const isSelected = selected === q.style;
                return (
                  <button
                    key={opt}
                    onClick={() => !selected && handleAnswer(q.style)}
                    style={{
                      background: isSelected ? "rgba(233,69,96,0.12)" : "rgba(255,255,255,0.04)",
                      border: `2px solid ${isSelected ? "#e94560" : "rgba(255,255,255,0.09)"}`,
                      borderRadius: 12,
                      padding: "18px 20px",
                      color: isSelected ? "white" : "#cbd5e1",
                      fontSize: 15,
                      textAlign: "left",
                      cursor: selected ? "default" : "pointer",
                      lineHeight: 1.55,
                      fontWeight: isSelected ? 600 : 400,
                      transition: "all 0.2s",
                    }}
                  >
                    <span style={{ fontWeight: 700, marginRight: 10, color: isSelected ? "#e94560" : "#475569" }}>{opt.toUpperCase()}.</span>
                    {q.text}
                  </button>
                );
              })}
            </div>
          </div>
        </div>
      )}

      {/* ── RESULT ── */}
      {screen === "result" && style && scores && (
        <div style={{ maxWidth: 580, width: "100%" }}>

          {/* Resultado principal */}
          <div style={{ textAlign: "center", marginBottom: 24 }}>
            <div style={{ fontSize: 60, marginBottom: 10 }}>{style.emoji}</div>
            <div style={{ color: "#64748b", fontSize: 11, fontWeight: 700, letterSpacing: 3, marginBottom: 8 }}>TU ESTILO NATURAL ES</div>
            <h1 style={{ color: style.color, fontSize: 42, fontWeight: 800, marginBottom: 16 }}>{style.label}</h1>

            {/* Post-it */}
            <div style={{
              display: "inline-flex", alignItems: "center", gap: 10,
              background: style.bg, border: `2px solid ${style.color}`,
              borderRadius: 12, padding: "12px 28px",
              boxShadow: `0 0 24px ${style.color}33`
            }}>
              <span style={{ fontSize: 22 }}>{style.postit.split(" ")[0]}</span>
              <div style={{ textAlign: "left" }}>
                <div style={{ color: style.color, fontSize: 11, fontWeight: 700, letterSpacing: 1 }}>COGE EL POST-IT</div>
                <div style={{ color: style.color, fontSize: 16, fontWeight: 800 }}>{style.postit.split(" ").slice(1).join(" ")}</div>
              </div>
            </div>
          </div>

          {/* Descripción */}
          <div style={{ background: "#1e293b", borderRadius: 16, padding: "22px 24px", marginBottom: 14 }}>
            <p style={{ color: "#e2e8f0", fontSize: 15, lineHeight: 1.75, marginBottom: 14 }}>{style.desc}</p>
            <div style={{ background: "rgba(233,69,96,0.08)", border: "1px solid rgba(233,69,96,0.25)", borderRadius: 10, padding: "14px 16px" }}>
              <div style={{ color: "#e94560", fontSize: 10, fontWeight: 700, letterSpacing: 1.5, marginBottom: 6 }}>PARA TENER EN CUENTA</div>
              <p style={{ color: "#94a3b8", fontSize: 13, lineHeight: 1.65, margin: 0 }}>{style.tip}</p>
            </div>
          </div>

          {/* Barras de todos los estilos */}
          <div style={{ background: "#1e293b", borderRadius: 16, padding: "20px 24px", marginBottom: 18 }}>
            <div style={{ color: "#334155", fontSize: 10, fontWeight: 700, letterSpacing: 1.5, marginBottom: 14 }}>TUS PUNTUACIONES</div>
            {Object.entries(scores).sort((a, b) => b[1] - a[1]).map(([key, val]) => {
              const s = STYLES[key];
              const isDom = key === dominant;
              return (
                <div key={key} style={{ marginBottom: 12 }}>
                  <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 5 }}>
                    <span style={{ color: isDom ? "white" : "#475569", fontSize: 13, fontWeight: isDom ? 700 : 400 }}>
                      {isDom ? "→ " : ""}{s.label}
                    </span>
                    <span style={{ color: isDom ? s.color : "#334155", fontSize: 13, fontWeight: 600 }}>{val}/15</span>
                  </div>
                  <div style={{ background: "#0f172a", borderRadius: 4, height: 7 }}>
                    <div style={{ background: isDom ? s.color : "#1e3a5f", height: 7, borderRadius: 4, width: `${(val / 15) * 100}%`, transition: "width 0.6s ease" }} />
                  </div>
                </div>
              );
            })}
          </div>

          <button onClick={restart} style={{ width: "100%", background: "transparent", color: "#475569", border: "1px solid #1e293b", borderRadius: 10, padding: "12px", fontSize: 14, cursor: "pointer" }}>
            Repetir test
          </button>
        </div>
      )}
    </div>
  );
}
