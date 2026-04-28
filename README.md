# Actividad GitHub Classroom: Miniutilidad ARM64 con Macro

## Objetivo
Diseñar e implementar una micropráctica de arquitectura de computadoras en ARM64 donde el estudiantado construya una utilidad de línea de comandos con ensamblador ARM64 (obligatorio) y una capa opcional mínima en Bash.

La utilidad propuesta: **convertidor de temperatura** (Celsius/Fahrenheit) con validación básica y despliegue de mensajes.

## Instrucciones
1. Acepta la tarea en GitHub Classroom y clona tu repositorio.
2. Crea una implementación principal en `src/main.s` (ARM64 Assembly) que incluya **al menos 1 macro**.
3. Implementa de 3 a 5 funcionalidades pequeñas:
   - Mostrar menú simple.
   - Convertir Celsius a Fahrenheit.
   - Convertir Fahrenheit a Celsius.
   - Validar opción fuera de rango.
4. (Opcional) Agrega capa mínima en Bash para compilar/ejecutar (`scripts/run.sh`).
5. Documenta y prueba con los formatos solicitados en `docs/`.
6. Entrega por commit y push antes de la fecha límite.

## Criterios
- Uso correcto de registros ARM64 y llamadas al sistema o libc según enfoque.
- Inclusión y uso real de una macro en ensamblador.
- Funcionalidades completas (3 a 5) y sin sobreingeniería.
- Estructura del repositorio clara y reproducible.
- Evidencia de pruebas y reflexión crítica del uso de IA.

## Rúbrica breve
- **40% Implementación ARM64:** compila, ejecuta y usa macro correctamente.
- **25% Funcionalidad:** conversiones y validación cumplen casos esperados.
- **20% Pruebas y documentación:** claridad, cobertura básica y reproducibilidad.
- **15% Integridad técnica/académica:** reflexión de IA, límites y validación manual.
