---
name: capturar-requerimientos
description: Lee documentos provistos (PDF, Word, texto, etc.) y extrae requerimientos estructurados, ambigüedades y preguntas abiertas. Úsala cuando el usuario entregue documentos de los que haya que sacar requisitos.
---

# Capturar requerimientos

Inspirada en `/to-spec` y `/grill-with-docs`: convertir material crudo en una especificación clara y cuestionar los vacíos.

## Proceso
1. **Leer** todos los documentos completos (usa la herramienta adecuada al formato). Anota la fuente de cada dato.
2. **Extraer** requerimientos explícitos; marca los implícitos como "inferidos".
3. **Clasificar** y numerar (RF-01, RNF-01...).
4. **Detectar** contradicciones, ambigüedades, términos sin definir y huecos.
5. **Cuestionar**: formula preguntas concretas, una por vez, con tu propuesta de respuesta.
6. **Entregar** la especificación en `.md`.

## Formato de salida
```md
# Requerimientos: [proyecto]

## Resumen y objetivo
## Actores / usuarios
## Glosario (términos del dominio)

## Requerimientos funcionales
| ID | Requerimiento | Prioridad | Fuente | Tipo (explícito/inferido) |

## Requerimientos no funcionales
(rendimiento, seguridad, accesibilidad, compatibilidad...)

## Restricciones y supuestos
## Fuera de alcance

## Contradicciones y ambigüedades
## Preguntas abiertas
```

## Reglas
- Cada requerimiento: atómico, verificable y trazable a su fuente (documento y sección/página).
- No inventes: lo no dicho va en "Preguntas abiertas".
- Prioriza con MoSCoW (Must/Should/Could/Won't) cuando haya señales.
- Resultado listo para alimentar la skill `documentar-ticket`.
