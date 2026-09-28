---
status: draft
opportunity: decisiones-perdidas-en-reuniones
channel: encuesta in-product en Teams
launch: solo si la oportunidad pasa el go/no-go del 18 oct 2026
beliefs: "#5 (value); #2 (value, reformulada tras el research)"
---

# Encuesta: lo decidido en reuniones grandes

- **Objetivos de aprendizaje**
  - **G1. Magnitud (creencia #5).** ¿Cuántas horas por semana dedican quienes conducen reuniones de 8+ a reconstruir o perseguir lo decidido, y con qué frecuencia se vuelve a decidir un tema? → *Decide:* si el problema alcanza el umbral de la creencia (≥2 h/semana, ≥1 tema re-decidido por semana) y justifica pasar a `/clarify-idea`, o si la oportunidad se achica.
  - **G2. Registro actual y acceso (#2 reformulada).** ¿Dónde queda hoy registrado lo decidido, y quiénes tienen el recap con IA disponible y lo usan? → *Decide:* si el hueco es de **acceso** (licencia/plan), de **adopción** (lo tienen y no lo usan) o de **encaje** (lo usan y igual recurren a Notion/Jira/Miro).
  - **G3. Dónde se rompe el ciclo.** ¿Se pierde en la captura (qué se decidió), en la asignación (quién) o en el seguimiento (si se cumplió)? → *Decide:* qué eslabón ataca una eventual solución; si es el seguimiento, compite con Fellow/Loom+Rovo, no con el recap.
  - **G4. Lado receptor (Julián Correa).** ¿Cuánto le cuesta al participante-ejecutor enterarse de lo que quedó a su cargo, y cuán seguido le asignan cosas que no aceptó? → *Decide:* si el receptor es un usuario a diseñar desde el inicio (y el riesgo de "herramienta de control" es real) o un efecto secundario.
- **Encuestados:** usuarios de cuentas Microsoft 365 con 100+ licencias que en las últimas 2 semanas estuvieron en al menos 1 reunión de Teams de 8+ participantes. Dos ramas según rol: **A — conducen** (Carolina Ferreyra) y **B — participan** (Julián Correa). Se excluye a invitados externos (Tomás Aldao).
- **Segmentación por telemetría (campos ocultos, no se preguntan):** tamaño de cuenta (100–1.000 / 1.000+), plan (Standard / Premium / Max), Teams Premium o Copilot asignado (sí/no), transcripción habilitada por política (sí/no), reuniones de 8+ en las últimas 2 semanas. Permiten cortar por acceso real y contrastar con la percepción de A4/B6.
- **Largo estimado:** 2 de screening + 7 de la rama + 3 de cierre = 12 ítems, ~4 min.

## Screening

S1. En las últimas 2 semanas, ¿en cuántas reuniones de Teams con 8 o más participantes estuviste? [opción única]
   - Ninguna → **fin de la encuesta**
   - 1 o 2
   - 3 a 5
   - 6 a 10
   - Más de 10
   > Goal: califica el perfil (reuniones de 8+); la frecuencia sirve de corte en todos los objetivos.

S2. En esas reuniones, ¿cuál es tu rol habitual? [opción única]
   - Las convoco o conduzco yo en la mayoría → **Rama A**
   - Participo; a veces conduzco alguna → **Rama A**
   - Participo; casi nunca las conduzco → **Rama B**
   - Participo como invitado de otra organización → **fin de la encuesta**
   > Goal: ruteo entre G1–G3 (conducen) y G4 (reciben).

## Rama A — quienes conducen

A1. Pensá en tu última semana laboral completa. Fuera de las reuniones, ¿cuánto tiempo dedicaste a reconstruir o perseguir lo que se decidió en reuniones de 8 o más personas? (por ejemplo: releer notas o el chat, volver a escuchar la grabación, preguntar qué quedó, recordarle a alguien un pendiente) [opción única]
   - Nada
   - Menos de 30 minutos
   - Entre 30 minutos y 1 hora
   - Entre 1 y 2 horas
   - Entre 2 y 4 horas
   - Más de 4 horas
   - No sé
   > Goal: G1 — la frontera 2 h coincide con el umbral de la creencia #5.

A2. En el último mes, ¿cuántas veces un tema que ya se había decidido en una reunión se volvió a discutir o decidir porque no había un registro claro de la decisión? [opción única]
   - Ninguna
   - 1 vez
   - 2 o 3 veces
   - 4 a 7 veces
   - 8 veces o más
   - No sé
   > Goal: G1 — "4 o más" ≈ 1 por semana, la segunda mitad de la creencia #5.

A3. En la última reunión de 8 o más personas que condujiste, ¿dónde quedaron registrados lo decidido y los responsables? Elegí todas las que correspondan. [opción múltiple]
   - Resumen automático de Teams con IA (recap, Copilot o Facilitator)
   - Notas de reunión de Teams escritas por alguien
   - Un documento propio (OneNote, Word, Loop, etc.)
   - Notion o Confluence
   - Una herramienta de tareas (Jira, Planner, Asana, etc.)
   - Un tablero (Miro, Mural, FigJam, Whiteboard)
   - Un mail de resumen
   - El chat de la reunión
   - En ningún lado
   - Otro: ______
   > Goal: G2 — mapa del registro actual; última reunión concreta en vez de "normalmente" para reducir sesgo de memoria.

A4. En tus reuniones, ¿tenés disponible el resumen automático con IA de Teams (intelligent recap o Copilot)? [opción única]
   - Sí, y lo uso en la mayoría de mis reuniones grandes
   - Sí, pero lo uso poco o nada
   - No lo tengo disponible
   - No sé si lo tengo
   > Goal: G2 — acceso vs. adopción; cruzar con la telemetría de licencia para separar "no lo tengo" de "no sé que lo tengo".

A5. Pensando en tus reuniones de 8 o más personas del último mes, ¿con qué frecuencia pasó cada una de estas situaciones? [matriz, frecuencia-5: Nunca · Rara vez · A veces · Seguido · Casi siempre]
   - a) Al terminar, no quedaba claro qué se había decidido.
   - b) Lo decidido estaba claro, pero no quién era responsable.
   - c) Había responsable, pero la tarea no avanzó y nadie lo notó hasta la reunión siguiente.
   - d) Alguien dijo no haberse enterado de que algo quedó a su cargo.
   > Goal: G3 — captura (a) vs. asignación (b) vs. seguimiento (c); (d) conecta con G4 desde el lado del conductor.

A6. En tus reuniones de 8 o más personas, ¿quién suele registrar lo que se decide? [opción única]
   - Yo, mientras conduzco
   - Otra persona designada
   - Cada participante anota lo suyo
   - El resumen automático con IA
   - Nadie en particular
   - Otro: ______
   > Goal: G2/G3 — confirma el síntoma de Carolina (modera y anota a la vez) y quién carga el costo.

A7. ¿Qué es lo más difícil de lograr que lo que se decide en una reunión grande efectivamente se cumpla? [abierta, opcional]
   > Goal: G3 — abre causas que las opciones no cubren; insumo principal para la guía de entrevista.

## Rama B — quienes participan

B1. Pensá en tu última semana laboral completa. ¿Cuánto tiempo dedicaste a averiguar qué quedó a tu cargo después de reuniones de 8 o más personas? (por ejemplo: volver a escuchar la grabación, preguntar por chat, revisar notas o mails) [opción única]
   - Nada
   - Menos de 30 minutos
   - Entre 30 minutos y 1 hora
   - Entre 1 y 2 horas
   - Más de 2 horas
   - No sé
   > Goal: G4 — magnitud del costo del receptor (persona: ~1,5 h/semana, sintético).

B2. En el último mes, ¿cuántas veces te enteraste de que algo había quedado a tu cargo recién cuando te lo reclamaron? [opción única]
   - Ninguna
   - 1 vez
   - 2 o 3 veces
   - 4 veces o más
   - No sé
   > Goal: G4 — frecuencia del síntoma principal de Julián.

B3. ¿Por dónde te enterás habitualmente de lo que quedó a tu cargo en una reunión grande? Elegí todas las que correspondan. [opción múltiple]
   - Lo anoto yo durante la reunión
   - Resumen automático de Teams con IA (recap, Copilot o Facilitator)
   - Notas que escribe quien conduce
   - El chat de la reunión
   - Un ticket o tarea (Jira, Planner, etc.)
   - Un mail posterior
   - Me lo recuerdan más adelante
   - Otro: ______
   > Goal: G2 + G4 — canales dispersos del lado receptor.

B4. ¿Dónde llevás la lista de lo que te comprometiste a hacer? [opción única]
   - Microsoft To Do o Planner
   - Jira u otra herramienta del equipo
   - Notas propias (OneNote, bloc de notas, etc.)
   - Papel o libreta
   - No llevo una lista
   - Otro: ______
   > Goal: G4 — workaround actual; si domina To Do/Planner, hay una integración nativa obvia.

B5. En el último mes, ¿alguna vez quedó registrado como tarea tuya algo que no habías aceptado explícitamente? [opción única]
   - Nunca
   - 1 vez
   - Varias veces
   - No sé
   > Goal: G4 — frecuencia del riesgo "me anotaron algo que no acepté" (escepticismo de Julián); pregunta de conducta, no de opinión sobre la IA.

B6. En tus reuniones, ¿tenés disponible el resumen automático con IA de Teams (intelligent recap o Copilot)? [opción única]
   - Sí, y lo consulto después de la mayoría de las reuniones grandes
   - Sí, pero lo consulto poco o nada
   - No lo tengo disponible
   - No sé si lo tengo
   > Goal: G2 — mismo corte de acceso vs. adopción, desde el receptor.

B7. ¿Qué es lo más difícil de saber qué quedó a tu cargo después de una reunión grande? [abierta, opcional]
   > Goal: G4 — causas del lado receptor; insumo para la guía de entrevista.

## Screening + opt-in (reclutamiento para entrevistas)

R1. ¿Trabajás en una empresa que desarrolla o vende software de reuniones, colaboración o productividad? [sí / no]
   → no es candidato si responde **sí**. Además, para entrevista se requiere S1 = "3 a 5" o más (perfil más estrecho que el de la encuesta).
   > Goal: excluir competidores y quedarse con quienes viven reuniones de 8+ seguido.

R2. ¿Aceptarías una conversación de 30 minutos con el equipo de producto sobre cómo manejan lo que se decide en las reuniones? [sí / no, opcional]
   > Goal: consentimiento para `/design-interview`.

R3. Si respondiste que sí, ¿cómo te contactamos? (mail o usuario de Teams) [abierta, opcional; visible solo si R2 = sí]
   > Goal: contacto del pool de reclutamiento.

## Notas para el análisis

- **Priorizar para entrevistas a quienes contradicen la creencia #5:** Rama A con A1 ≤ "30 min–1 h" y A2 ≤ "1 vez"; y quienes tienen recap (A4/B6 = "Sí, y lo uso") pero igual registran en Notion/Jira/Miro (A3/B3) — son los que explican la nueva forma de #2.
- **Cortes clave:** acceso real a Premium/Copilot (telemetría) × A1/A2; tamaño de cuenta; conductores vs. participantes.
- **Límites conocidos:** A1/B1 son estimaciones de memoria de una semana (ruidosas; leer como rangos, no promedios). La muestra in-product se autoselecciona hacia usuarios más comprometidos. Si la rama B junta pocas respuestas, activar una cuota o un segundo disparo solo para participantes.
