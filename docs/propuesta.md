# Propuesta de micropráctica

## Problema
En cursos introductorios de arquitectura, muchas veces se ve ARM64 de forma teórica, pero falta una práctica corta que conecte registros, operaciones aritméticas y flujo de control con una necesidad concreta.

## Justificación
Una utilidad de conversión de temperatura permite practicar:
- Manejo de entrada/salida básica.
- Aritmética entera o de punto flotante simple.
- Saltos condicionales y validación.
- Reuso de código mediante macro en ARM64.

## Alcance
- Implementación sugerida de máximo ~150 líneas de código ensamblador.
- 4 funcionalidades: menú, C→F, F→C y validación de opción.
- Capa opcional mínima en Bash para automatizar compilación y ejecución.
- Sin Python, sin frameworks pesados, sin contenedores.

## Arquitectura
- `src/main.s`: lógica principal en ARM64.
- Macro obligatoria sugerida: `PRINT msg, len` para despliegue de textos.
- Flujo:
  1. Mostrar menú.
  2. Leer opción.
  3. Ejecutar rutina de conversión.
  4. Mostrar resultado o error.

## Riesgos
- Diferencias de toolchain entre equipos (Linux ARM64 nativo vs cross-compile).
- Errores en manejo de registros volátiles/no volátiles.
- Redondeo inesperado si se usa aritmética entera.
- Validación incompleta de entrada no numérica.
