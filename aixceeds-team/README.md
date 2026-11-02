# AIXCEEDS Team · 4971 Ventures

Equipo de consultores y desarrolladores IA para el desarrollo de negocios de
**AIXCEEDS** y del venture studio **4971 Ventures**. Funciona en **Claude
Cowork** y en **Claude Code** (es el mismo plugin).

## El equipo (agentes)

| Agente | Rol |
|--------|-----|
| `estratega-bizdev` | Estrategia, modelos de negocio, go-to-market, alianzas, propuestas |
| `analista-mercado` | Mercados, competencia, TAM/SAM/SOM, tendencias de IA, perfiles |
| `analista-inversiones` | Unit economics, stage gates GO/ITERAR/KILL, cap table, valuaciones, memos |
| `arquitecto-desarrollador` | Arquitectura de soluciones IA, MVPs, Command Center, code review |
| `rd-publicaciones` | R&D de publicaciones para posicionamiento: artículos, whitepapers, LinkedIn, calendario |

## Comandos (skills)

| Skill | Para qué |
|-------|----------|
| `/reunion-equipo` | Convoca a los especialistas necesarios sobre una decisión y entrega un acta con la decisión y próximos pasos |
| `/validar-venture` | Evalúa una idea o venture contra los stage gates del studio → GO / ITERAR / KILL |
| `/memo-inversion` | Memo de inversión, spin-out o due diligence |
| `/investigacion-mercado` | Investigación de mercado y competencia con fuentes citadas |
| `/plan-publicaciones` | Estrategia de posicionamiento, calendario editorial de 90 días y redacción de piezas |
| `/brief-tecnico` | Del objetivo de negocio a la arquitectura, el costo y el MVP |
| `contexto-aixceeds` | Se carga sola: perfil de los negocios, plantilla de marca y reglas del equipo |

## Primer paso importante

Completá la ficha `skills/contexto-aixceeds/references/perfil-negocios.md`
(los campos `[POR COMPLETAR]`): tesis del studio, portafolio, prioridades,
credenciales y temas de posicionamiento. Los agentes nunca inventan esos datos.
También podés pedirle al equipo: *"Ayudame a completar el perfil de negocios"*.

## Plantilla de marca

Todos los entregables usan la plantilla AIXCEEDS
(`skills/contexto-aixceeds/references/plantilla-marca.md`):
fondo azul noche `#0B1426` con tipografía Book Antiqua plateada, o fondo plata
`#E9ECF1` con Calibri azul noche; destacados siempre en Blue Martini `#2E74E8`,
raramente Red Martini `#E23B4E` o blanco.

## Instalación

**Cowork**: abrí el archivo `aixceeds-team.plugin` en la conversación y aceptá la instalación.

**Claude Code** (desde una copia local de esta carpeta):

```
/plugin marketplace add ./aixceeds-team
/plugin install aixceeds-team@aixceeds
```

## Conectores que aprovecha

Google Drive, Gmail, Google Calendar, Gamma, DocuSign y búsqueda web, si están
conectados. Las acciones hacia afuera (enviar emails, publicar, firmar, crear
eventos) siempre requieren tu aprobación: el equipo entrega borradores.

## Ejemplos

- *"Convocá al equipo: ¿lanzamos primero el venture de IA para contadores o el de logística?"*
- *"Validá esta idea: agentes de IA que preparan due diligence para fondos chicos."*
- *"Armame el plan editorial de 90 días para posicionarme en venture building con IA, en español e italiano."*
- *"Diseñá el MVP para validar con 5 clientes en 2 semanas y decime cuánto cuesta."*
