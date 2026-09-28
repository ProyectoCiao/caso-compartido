---
source: secondary
method: web
date: 2026-09-27
question: ¿Es real y costoso el problema de las decisiones y compromisos perdidos en reuniones grandes? ¿Quién lo resuelve hoy, a qué precio, y hay evidencia de que las herramientas externas de registro empujen bajas de licencia?
opportunity: decisiones-perdidas-en-reuniones
---

# Research: decisiones perdidas en reuniones

Hay tres hallazgos que cambian decisiones:

1. **La capacidad ya existe dentro de Microsoft, pero detrás de un pago.** Teams ya genera notas y tareas con IA de tres formas, todas en disponibilidad general (GA): intelligent recap, Copilot en la reunión y el agente Facilitator. Las tres requieren Teams Premium (USD 10) o M365 Copilot (USD 18–30), y Copilot llega a ~6,5% de los asientos comerciales. La idea candidata del brief, "herramientas colaborativas integradas en la reunión", en buena parte ya está construida. Lo que queda abierto es otra cosa: **cuánta gente accede, si lo que captura es correcto y si el ciclo se cierra hasta el seguimiento**. El seguimiento con Planner sigue en preview.
2. **El síntoma está muy extendido; la magnitud no está medida.** Alrededor de la mitad de los trabajadores sale de las reuniones sin próximos pasos claros ni un responsable (55% según Microsoft; 54% según Atlassian). Ninguna fuente mide horas por semana reconstruyendo lo decidido, temas que se vuelven a decidir, ni un corte por reuniones de 8+. La creencia #5 no queda ni apoyada ni contradicha en su cuantificación.
3. **El diferencial de los competidores es llevar lo decidido al sistema donde vive el trabajo** (Jira, CRM, Notion), no el resumen en sí. Al mismo tiempo, desde mayo de 2026 Teams bloquea los bots externos y hay litigios contra notetakers, lo que juega a favor de una solución nativa y dentro de la gobernanza de M365. Sin embargo, las notas de Facilitator todavía no heredan etiquetas de sensibilidad ni entran en eDiscovery.

> Límite: esto es evidencia sobre el **mercado**. No verifica nada sobre los usuarios de Teams ni sobre la causalidad a nivel cuenta.

## Lane 1: el costo del problema (Q1)

| Hallazgo | Fuente / sponsor / n / año | Label |
|---|---|---|
| 55%: los próximos pasos no quedan claros al terminar la reunión. 56% tiene dificultad para resumirla. | Microsoft Work Trend Index (Edelman para Microsoft; con sesgo de vendor), n=31.000, 2023 | [verificado: https://www.microsoft.com/en-us/worklab/work-trend-index/will-ai-fix-work — 2026-09-27] |
| 54% sale seguido de reuniones sin próximos pasos ni responsable. 77% sale con un "agendemos otra". 75% dice que las reuniones no sirven para decidir. | Atlassian "Workplace Woes: Meetings" (vendor), n=5.000, 2024, metodología no publicada | [verificado: https://www.atlassian.com/blog/workplace-woes-meetings — 2026-09-27] |
| Se pierde el 25% del tiempo buscando respuestas (no es específico de reuniones). | Atlassian State of Teams 2025 (vendor), n=12.000 | [verificado: https://www.atlassian.com/blog/state-of-teams-2025 — 2026-09-27] |
| 2,8 h/semana en reuniones innecesarias (3,6 h en senior leaders). | Asana Anatomy of Work 2023 (vendor), n=9.615 | [verificado: https://investors.asana.com/news-releases/news-release-details/asana-anatomy-work-global-index-2023-smart-collaboration-and — 2026-09-27] |
| El 71% se saltearía una reunión si recibiera buenas notas a tiempo. | Otter.ai + Rogelberg (vendor), n=632, 2022, muestra débil | [verificado: https://otter.ai/blog/one-third-of-meetings-are-unnecessary-costing-companies-millions-and-no-one-is-happy-about-it — 2026-09-27] |
| Las reuniones que giran alrededor de un documento cumplieron su objetivo en 85% de los casos, contra 69% del grupo de control. | Experimento interno de Atlassian, n=104, 2024 | [verificado: https://www.atlassian.com/blog/productivity/page-led-meetings — 2026-09-27] |
| "Regla de 7": a partir de 7 personas, cada miembro extra resta ~10% de efectividad en la decisión. | Bain, 2010. Es una heurística, n desconocido | [verificado: https://www.bain.com/insights/effective-decision-making-and-the-rule-of-7/ — 2026-09-27] |
| Las reuniones de 65+ asistentes son el tipo de reunión que más crece. | Telemetría de M365, 2025 | [verificado: https://www.microsoft.com/en-us/worklab/work-trend-index/breaking-down-infinite-workday — 2026-09-27] |

**Desconocido:** horas por semana reconstruyendo o persiguiendo decisiones; tasa de cumplimiento de los action items; frecuencia de temas que se vuelven a decidir; cualquier corte por reuniones de 8+ o por mandos medios en cuentas de 100+.

## Lane 2: competidores y alternativas (Q2)

| Jugador | Qué hace con decisiones y action items | ¿Funciona en Teams? | Estado / licencia | Label |
|---|---|---|---|---|
| **Intelligent recap (Teams)** | Notas con IA, tareas recomendadas, capítulos. No aparecen campos de "decisión" ni de "responsable". | Nativo | GA; requiere Premium o Copilot, y la transcripción activada | [verificado: https://learn.microsoft.com/en-us/microsoftteams/intelligent-recap-calls-meetings — 2026-09-27] |
| **Copilot en la reunión** | Responde preguntas en vivo o después: decisiones clave, tareas | Nativo | Licencia Copilot; ~30M de asientos, ~6,5% del total comercial (FY26 Q4) | [verificado: learn.microsoft.com (módulo de training) + https://2-data.com/knowledge-hub/microsoft-365-copilot-passed-30-million-seats-what-the-fy26-numbers-actually-tell-enterprise-buyers/ (fuente secundaria) — 2026-09-27] |
| **Facilitator (agente)** | Notas colaborativas en tiempo real y captura de action items. El seguimiento con Planner está en **preview**. | Nativo. No funciona en chats 1:1, grupales ni externos | GA con Copilot. Las notas **no heredan etiquetas de sensibilidad ni entran en eDiscovery**. Pasa de Loop a Word desde el 31/07/2026 | [verificado: https://learn.microsoft.com/en-us/microsoftteams/facilitator-teams — 2026-09-27] |
| **Google Meet "Take notes for me"** | Próximos pasos editables y asignables a una persona | No | Workspace Business/Enterprise | [verificado: https://workspaceupdates.googleblog.com/2025/02/google-meet-take-notes-for-me-next-steps.html — 2026-09-27] |
| **Zoom AI Companion / ZoomMate** | Resumen con próximos pasos | Sí (bot o captura local) | Básico incluido; add-on pago | [verificado: fuente secundaria kb.adampulse.us — 2026-09-27] |
| **Otter, Fireflies, Fathom, Read.ai, tl;dv** | Resúmenes y action items (la captura de Otter y tl;dv se califica de "básica") | Sí, como bot | Tienen free; planes de ~USD 15–29 | [verificado: comparativa de vendor, https://www.cirrusinsight.com/blog/microsoft-teams-ai-meeting-assistants-notetakers — 2026-09-27] |
| **Fellow** | Seguimiento de action items **entre** reuniones (es su diferencial) | Sí | USD 7–15 según la comparativa (ver precios) | [verificado: misma fuente — 2026-09-27] |
| **Notion AI Meeting Notes** | Puntos clave y action items dentro de Notion | Sí, **sin bot** (captura el audio del sistema) | Plan Business | [verificado: https://www.notion.com/help/ai-meeting-notes — 2026-09-27] |
| **Atlassian Loom + Rovo** | Convierte decisiones y action items en actualizaciones de Jira (estado, asignado); un humano las aplica. Lanzado el 27/07/2026 | Solo desde Loom; no se menciona Teams | Jira Standard+ con Rovo | [verificado: https://jirareleases.atlassian.com/announcements/your-meeting-decisions-already-updated-in-jira — 2026-09-27] |
| **Slack huddle notes** | Canvas con temas y action items; si asigna responsable: desconocido | No | Planes pagos | [verificado: https://slack.com/help/articles/31377193680019-Use-AI-to-take-huddle-notes-in-Slack — 2026-09-27] |
| **Miro** | Tableros y resúmenes con IA; sobre action items: desconocido | Tiene app en Teams | desconocido | [conocimiento del modelo — verificar] |
| **No consumo** (notas a mano, doc compartido, mail, nada) | — | — | Prevalencia desconocida | — |

**Otras señales:**

- **Bots externos:** desde mayo de 2026, Teams detecta los bots externos, los manda al lobby como "no verificados" y el admin puede bloquearlos (`ExternalBotAccessMode`). [verificado: https://blog-en.topedia.com/2026/05/meeting-bot-detection-in-microsoft-teams/ — 2026-09-27]
- **Riesgo legal:** hay litigios de privacidad contra Otter y demandas bajo BIPA contra Fireflies, y algunas universidades bloquean bots que no son nativos. [verificado: https://www.uctoday.com/security-compliance-risk/ai-meeting-bots-controls-microsoft-zoom-google/ — 2026-09-27]
- **Adopción en EE.UU.:** 33,4% de los trabajadores tuvo un notetaker de IA en sus reuniones, y solo al 34,7% se le pidió permiso de forma consistente (Kolmogorov Law/Pollfish, n=500, julio 2026). [verificado: https://abc17news.com/stacker-business-economy/2026/07/17/ai-notetakers-have-sat-in-on-1-in-3-us-workers-meetings-but-only-a-third-say-they-were-asked-first/ — 2026-09-27]
- **Precisión de los action items y de la detección de decisiones en reuniones grandes:** desconocido.

**Qué prueba la existencia de estos jugadores:** que hay demanda pagada por capturar action items, en todas las plataformas. **Qué no prueba:** que los compromisos se cumplan, que las decisiones se detecten bien con 8+ participantes, ni que el segmento de Teams vaya a cambiar su forma de trabajar.

## Lane 3: precios y modelos (Q3)

| Jugador | Modelo | Free | Business/Enterprise (USD/usuario/mes) | Action items | Label |
|---|---|---|---|---|---|
| M365 Copilot | Add-on | Copilot Chat sin costo, pero **sin recap** | Business 18 anual / 25,20 mensual; Enterprise 30 / 31,50 | Sí | [verificado: microsoft.com/…/copilot/business y /enterprise; support.microsoft.com — 2026-09-27] |
| Teams Premium | Add-on | Trial de 1 mes | 10 anual; mensual desconocido | Sí (recap) | [verificado: microsoft.com/en-us/microsoft-teams/premium — 2026-09-27] |
| Google Workspace | IA incluida en el plan | No | Starter 7 / Standard 14 / Plus 22; Gemini en Meet desde Standard | Sí | [verificado: workspace.google.com/pricing (planes) + itechguides.com (precios, fuente de terceros) — 2026-09-27] |
| Zoom (ZoomMate) | Básico incluido + add-on | 3 resúmenes al mes | 16,67 anual / 20 mensual | No lo dice explícitamente | [verificado: zoom.us/pricing/aic — 2026-09-27] |
| Otter.ai | Independiente | Sí | Business 19,99 / 30 | Sí | [verificado: otter.ai/pricing — 2026-09-27] |
| Fireflies.ai | Independiente | Sí, sin action items | Business 19 / 29; Enterprise 39 | Sí, desde Pro | [verificado: fireflies.ai/pricing — 2026-09-27] |
| Read.ai | Independiente | 5 reuniones al mes | 22,50 / 29,75 | Sí | [verificado: read.ai/plans-pricing — 2026-09-27] |
| Fathom | Independiente | Sí, sin action items | Team 15 / 19; Business 25 / 34 | Sí | [verificado: fathom.ai/pricing — 2026-09-27] |
| Fellow | Independiente | 5 notas en total | Business 15 / 23; Enterprise 25 | Sí | [verificado: fellow.ai/pricing — 2026-09-27] |
| Avoma | Independiente | Trial | 24 / 39 | Sí | [verificado: avoma.com/pricing — 2026-09-27] |
| tl;dv | Independiente | 10 notas al mes | Pro 18; Business 59 | desconocido | [verificado: g2.com (terceros) — 2026-09-27] |
| Notion | IA incluida en el plan | Trial | Business 20 mensual; anual inconsistente | Sí | [verificado: notion.com/pricing — 2026-09-27] |
| Loom | Plan con IA aparte | Starter | Business 18; Business + AI 24 | Recaps | [verificado: atlassian.com/software/loom/pricing — 2026-09-27] |

**Anclas de precio:**

- **Las herramientas independientes cobran USD 15–25/usuario/mes** (anual) con los action items incluidos.
- **Google incluye la IA en el plan base** desde USD 14.
- **Microsoft cobra USD 10 (Premium) o USD 18–30 (Copilot).**

El upgrade Premium→Max de USD 8 del overview queda por debajo de todas estas anclas. No se encontró públicamente ningún plan "Max" para contrastarlo; es dato interno. El riesgo en cuentas de 100+ es que el comprador espere tener los action items "en la base", como pasa con Google.

## Lane 4: herramientas externas y churn (Q4)

- **Sprawl y presión de costos:** en promedio el 36% de las licencias SaaS no se usa, y el 61% de los líderes de IT tuvo que recortar proyectos por aumentos de costo. No hay datos sobre qué apps se recortan y cuáles se mantienen (Zylo 2026 SaaS Management Index, vendor; 40M de licencias + 218 líderes). [verificado: https://zylo.com/news/2026-saas-management-index — 2026-09-27] Esto es coherente con el motivo de baja "pagamos por funciones que no usamos", pero no dice nada sobre el tipo de herramienta.
- **No hay desplazamiento masivo desde Teams tras el unbundling en la UE:** el 84% de los decisores habría comprado Teams igual como producto separado (Cavell, n>400, UK/US). [verificado: https://www.uctoday.com/unified-communications/what-did-the-microsofts-teams-unbundling-really-achieve-for-the-ucaas-market/ — 2026-09-27]
- **La consolidación visible va hacia Teams:** Cornell migró de Slack a Teams en enero de 2026 por costo. Es un solo caso. [verificado: https://it.cornell.edu/news/cit-slack-transitions-microsoft-teams-january-23-2026 — 2026-09-27]
- **La señal de recorte por bajo uso aparece en los add-ons, no en la licencia base:**
  - Solo el 3,3% de los usuarios de Copilot Chat paga (Q2 FY26). [verificado: https://www.theregister.com/2026/02/02/microsoft_ai_spend_copilot/ — 2026-09-27]
  - El uso semanal sostenido de Copilot es de 30–55% de los asientos comprados (Redress, 25–35 despliegues). [verificado: https://redresscompliance.com/microsoft-copilot-adoption-2026 — 2026-09-27]
  - Según Gartner 2025, la mayoría de las organizaciones pausó la expansión de Copilot para evaluar el ROI. [verificado: https://www.techpartner.news/news/gartner-microsoft-copilot-hype-offset-by-roi-and-readiness-realities-618118 — 2026-09-27]
- **Notion, Miro y Jira frente a Loop y Whiteboard:** no hay datos de adopción ni de desplazamiento; solo comparativas de blogs. Desconocido.

## Impacto en creencias

| Creencia (de overview.md) | Veredicto | Evidencia |
|---|---|---|
| **#5** [opportunity] [value]: los Team Leads con reuniones de 8+ dedican ≥2 h/semana a reconstruir lo decidido, y ≥1 tema por semana se vuelve a decidir | **Apoya el síntoma; no dice nada sobre la magnitud** | 55% sin próximos pasos claros (Microsoft 2023) y 54% sin responsable (Atlassian 2024) [verificado]. No hay datos de horas, de temas re-decididos ni de reuniones 8+. |
| **#6** [opportunity] [viability]: en las cuentas que bajaron citando "otras herramientas", pesan más las de registro (Notion, Miro, Jira) | **No dice nada** | No hay datos por app sobre qué se recorta (Zylo, Okta) [verificado]. Es causalidad a nivel cuenta: solo los datos internos la resuelven. |
| **#2** [product] [value]: el link externo aparece porque lo nativo no cubre la necesidad; con una alternativa nativa buena, se dejaría de usar | **Contradice la formulación actual (parcialmente)** | La alternativa nativa ya existe en GA (recap, Copilot, Facilitator) [verificado]. Si el link persiste, las causas probables son el acceso (Copilot ~6,5% de los asientos; recap solo con Premium o Copilot) o que el trabajo vive en Jira o Notion, no una función faltante. |
| **#1** [product] [viability]: la coexistencia con Slack/Google Chat es un riesgo real de reducción de licencias | **Contradice débilmente / no concluye** | No hay desplazamiento masivo tras el unbundling (Cavell 84%), y la consolidación visible favorece a Teams (Cornell) [verificado]. La señal de recorte aparece en los add-ons (Copilot), no en la licencia base. |
| #3, #4 | No tocadas | Fuera del alcance de esta corrida. |

Ninguna de estas creencias se anota en `overview.md` a partir de esta corrida. Si alguna contradicción amerita `weakened`, lo decide `/review-evidence`.

## Qué sigue necesitando research primario

**Datos internos** (ya en la agenda del brief, antes del 11 oct):

- Cruzar la adopción de recap, Copilot y Facilitator en reuniones de 8+ con la tasa de links externos: ¿el link cae cuando la cuenta tiene Premium o Copilot? Esto resuelve la nueva forma de #2.
- Herramientas nombradas en las cancelaciones y dominios de los links externos, en cuentas que bajaron frente a cuentas que renovaron (#6).
- El plan "Max": qué incluye hoy en relación con el recap y los action items.

**Encuesta** (`/design-survey`, cuántos y cuánto; creencia #5):

- Horas por semana reconstruyendo lo decidido.
- Temas re-decididos por semana.
- % de reuniones de 8+ con recap activo.
- Acceso a Premium o Copilot.
- Qué herramienta usan hoy para registrar.

**Entrevistas** (`/design-interview`, por qué y qué hacen hoy):

- Por qué, teniendo recap, se sigue recurriendo a Notion, Jira o Miro.
- Si el problema es capturar o **cerrar el ciclo** (seguimiento y asignación).
- Si el recap acierta en reuniones de 8+.
- Cómo vive el participante-ejecutor (Julián) que la IA le asigne tareas que no aceptó.
