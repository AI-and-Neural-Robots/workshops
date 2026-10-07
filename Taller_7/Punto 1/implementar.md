---
name: implementar
description: Implementa un ticket generando código y pruebas con TDD y ciclos de feedback. Úsala cuando se pida implementar, codificar o resolver un ticket.
---

# Implementar

Inspirada en `/implement` y `/tdd`: rojo → verde → refactor, en pasos pequeños.

## Proceso
1. **Leer**: ticket, criterios de aceptación y código vecino. Respeta convenciones existentes.
2. **Plan breve**: lista los comportamientos a probar, en orden. Si algo es ambiguo, pregunta antes de codificar.
3. **Ciclo TDD**, un comportamiento a la vez:
   - Rojo: escribe una prueba que falle por la razón correcta.
   - Verde: el código mínimo para pasar.
   - Refactor: limpia con las pruebas en verde.
4. **Feedback loops**: tras cada ciclo ejecuta tests, tipos y linter. No avances con errores.
5. **Verificar**: recorre cada criterio de aceptación y confirma que está cubierto.
6. **Cerrar**: resume qué cambió, qué pruebas se añadieron y qué quedó fuera.

## Reglas
- Prueba comportamiento por la interfaz pública, no detalles internos; evita mocks innecesarios.
- Cambios mínimos y enfocados: nada fuera del alcance del ticket.
- Módulos profundos: interfaz simple, lógica oculta.
- Sin código muerto, sin comentarios que repitan el código.
- Commits pequeños con mensajes descriptivos.
- Si encuentras un bug o deuda ajena al ticket, anótalo; no lo mezcles.
