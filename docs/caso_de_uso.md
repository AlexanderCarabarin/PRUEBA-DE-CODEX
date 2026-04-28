# Caso de uso: Conversión térmica en consola

## Actor
Estudiante de sistemas embebidos que ejecuta una utilidad ARM64 desde terminal.

## Flujo principal
1. El actor ejecuta el binario.
2. El sistema muestra menú con opciones: 1) C→F, 2) F→C, 3) Salir.
3. El actor selecciona opción válida (1 o 2).
4. El sistema solicita valor numérico.
5. El actor captura el valor.
6. El sistema calcula conversión y muestra resultado.
7. El sistema regresa al menú.

## Flujos alternos
### Alterno A: opción inválida
1. El actor ingresa opción distinta de 1, 2 o 3.
2. El sistema muestra mensaje de error.
3. El sistema regresa al menú sin terminar ejecución.

### Alterno B: salida voluntaria
1. El actor selecciona opción 3.
2. El sistema muestra mensaje de cierre.
3. El proceso termina limpiamente.

## Criterios de aceptación
- El menú se muestra en cada iteración hasta seleccionar salida.
- Opción inválida no truena programa y muestra error claro.
- Fórmula C→F implementada correctamente: `(C * 9 / 5) + 32`.
- Fórmula F→C implementada correctamente: `(F - 32) * 5 / 9`.
- Existe al menos una macro ARM64 usada en el flujo normal.
