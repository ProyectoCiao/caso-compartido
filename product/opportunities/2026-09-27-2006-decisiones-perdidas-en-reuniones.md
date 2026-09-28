---
status: framed
segment: Team Leads y mandos medios que convocan y conducen reuniones de 8+ participantes en cuentas Microsoft 365 medianas y grandes (100+ licencias)
personas: carolina-ferreyra, julian-correa
---

# Opportunity: Lo decidido en reuniones grandes se pierde

Quienes conducen reuniones de 8 o más personas en Teams terminan sin un registro compartido de qué se decidió y quién se comprometió a qué: los temas se re-deciden en la reunión siguiente y los pendientes se caen. Por qué ahora: Reuniones es el módulo más usado (82% semanal, 11,4 h/semana por usuario corporativo), las funciones nativas de registro casi no se usan (notas 8%, Whiteboard 5%), y "el equipo ya usa otras herramientas" aparece entre los motivos de baja.

## Segment and personas

- **Sufre:** Carolina Ferreyra (primaria) — Team Lead que conduce reuniones de 8+ y toma notas a mano mientras modera.
- **Le importa, no lo sufre:** Martín Ibarra (secundaria) — comprador; le importa porque el uso real justifica (o no) el plan en la renovación.
- **Fuera:** Rosa Giménez (terciaria) — su dolor es encontrar archivos, no lo decidido; Tomás Aldao (negativa) — invitado externo sin M365.
- **Sufre (lado receptor):** Julián Correa (secundaria) — analista que recibe los compromisos de reuniones de 8+ de dos líderes; escéptico de que un registro se vuelva control o le asigne tareas que no aceptó. Ver `product/personas/julian-correa.md`.
- **Persona faltante (cubierta):** el integrante del equipo que *recibe* los compromisos de la reunión (participante-ejecutor en cuentas medianas/grandes). Generada con `/generate-personas` el 27 sep 2026 → **Julián Correa** (`product/personas/julian-correa.md`).

## Signals

| Signal | Provenance | Source |
|---|---|---|
| Notas de reunión se usan en el 8% de las reuniones; Whiteboard en el 5% | unverified | overview.md — "datos de uso del producto", sin reporte adjunto |
| 41% de las reuniones tiene más de 8 participantes; 23% supera la hora | unverified | overview.md — datos de uso, sin reporte adjunto |
| En el 29% de las reuniones de 5+ se comparte un link externo (Notion, Miro, Jira…) | unverified | overview.md — datos de uso, sin reporte adjunto |
| 19% de los comentarios negativos post-reunión son sobre "colaboración durante la reunión" | unverified | overview.md — encuestas post-reunión, sin n ni archivo |
| "El equipo ya usa otras herramientas" es el 3er motivo de baja/downgrade (sin especificar cuáles) | unverified | overview.md — encuestas de cancelación, sin n ni archivo |
| Team Lead repite decisiones en la reunión siguiente, pierde quién se comprometió a qué, los pendientes se caen; links a Miro/Jira se pierden en el chat | synthetic | carolina-ferreyra.md |
| Participante-ejecutor se entera de lo asignado cuando se lo reclaman; compromisos dispersos entre reunión, chat, Jira y mail; ~1,5 h/semana reconstruyéndolos | synthetic | julian-correa.md |

## Business outcome

**Retención / renovación neta** (modo existing · commercial). Reducir el 3,6% de cuentas que bajan de plan o no renuevan, atacando "el equipo ya usa otras herramientas" y dándole a IT evidencia de uso real en la renovación ("pagamos por funciones que no usamos").

## Constraints

- Cualquier solución debe vivir dentro de la gobernanza de Microsoft 365: retención de datos y auditoría (fuente: Martín Ibarra, synthetic — a confirmar con cuentas reguladas).
- No se diseña para invitados externos sin Microsoft 365 (límite de la persona negativa).
- Presupuesto y fechas de entrega: no declarados.
- Decisión de perseguir o descartar esta oportunidad: en 3 semanas (18 oct 2026).

## Beliefs

Referencias a `product/overview.md` (registro único):

- [product] [value] #2 — el link externo en reuniones de 5+ aparece porque las herramientas nativas no cubren la necesidad *(existente; esta oportunidad la toca directo)*
- [product] [viability] #1 — la coexistencia con Slack/Google Chat es un riesgo real de reducción de licencias *(existente; relacionada)*
- #5 — [opportunity: decisiones-perdidas-en-reuniones] [value] Los Team Leads que conducen reuniones de 8+ participantes dedican ≥2 h/semana a reconstruir y perseguir lo decidido (notas a mano, re-preguntar, re-decidir), y al menos 1 tema por semana se vuelve a decidir porque no quedó registrado.
- #6 — [opportunity: decisiones-perdidas-en-reuniones] [viability] En las cuentas que bajaron de plan o no renovaron citando "el equipo ya usa otras herramientas", esas herramientas incluyen las usadas para registrar lo decidido en reuniones (Notion, Miro, Jira) en mayor proporción que en las cuentas que renovaron.

## Research agenda

| Belief | Instrument | Decision it unlocks | By when |
|---|---|---|---|
| Todas (señales) | **Datos internos:** pedir los reportes detrás de las cifras del overview (uso de notas/Whiteboard por tamaño de reunión, n de la encuesta post-reunión) | Si las señales pasan de `unverified` a `real`, o se cae el "por qué ahora" | 4 oct 2026 |
| [viability] opportunity | **Datos internos:** cruzar respuestas abiertas de las encuestas de cancelación con las herramientas nombradas; comparar dominios de links externos en reuniones de cuentas que bajaron vs. renovaron | Si registrar decisiones está ligado a la baja → perseguir; si no → descartar o re-enmarcar como oportunidad de productividad sin impacto en retención | 11 oct 2026 |
| [value] opportunity + #2 | **`/research-market`:** evidencia secundaria sobre costo de decisiones perdidas en reuniones y adopción de herramientas de registro (Notion, Miro, Jira en reuniones) | Si el problema es real y pagado en el mercado → justifica encuesta; si no → baja la prioridad | 11 oct 2026 |
| — | **Decisión go / no-go** | Pasar a `/clarify-idea` o guardar como `discarded` | **18 oct 2026** |
| [value] opportunity (horas, frecuencia) | **`/design-survey`** a Team Leads de cuentas 100+ con opt-in para entrevista | Tamaño del problema: cuántos, cuántas horas | Después del 18 oct, solo si pasa el go |
| [value] opportunity (por qué, workaround actual) | **`/design-interview`** entre opt-ins, priorizando a quienes contradicen la creencia; incluir al participante-ejecutor | Qué hacen hoy y dónde duele — insumo para `/clarify-idea` | Después de la encuesta |

## Candidate ideas (not evaluated)

- Herramientas colaborativas integradas en la reunión (el pedido original)
