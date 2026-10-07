---
name: explicar-trabajo
description: Genera un HTML autocontenido que explica en detalle el trabajo realizado (qué, por qué, cómo, pruebas). Úsala al terminar una implementación o cuando se pida explicar cambios.
---

# Explicar trabajo

Inspirada en `/teach` y `/wait-what`: explicar para que el lector **entienda**, no solo vea el diff.

## Proceso
1. Reúne la evidencia real: ticket, diff/commits, archivos tocados y resultados de pruebas. No inventes.
2. Ordena de lo general a lo particular.
3. Genera **un solo archivo `.html`** (CSS inline, sin dependencias externas, legible en claro/oscuro).
4. Entrégalo y resume en una línea qué contiene.

## Estructura del HTML
1. **Resumen**: qué se hizo y por qué, en 3-5 líneas.
2. **Contexto**: problema y requerimiento original.
3. **Enfoque y decisiones**: alternativas consideradas y por qué se eligió esta.
4. **Recorrido de cambios**: por archivo/módulo, con fragmentos de código comentados.
5. **Diagrama o flujo** (SVG inline) si ayuda a ver la arquitectura o el flujo de datos.
6. **Pruebas**: qué se cubre, cómo ejecutarlas, resultados.
7. **Riesgos, límites y pendientes**.
8. **Cómo verificar**: pasos para que el lector lo compruebe.

## Reglas
- Lenguaje claro, términos del dominio definidos la primera vez.
- Muestra el *porqué*, no solo el *qué*.
- Código en bloques `<pre><code>`, breve y solo lo relevante.
- Diseño sobrio: tipografía legible, secciones con índice, responsive.
