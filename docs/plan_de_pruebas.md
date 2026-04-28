# Plan de pruebas

## Estrategia
- Pruebas funcionales de caja negra desde terminal.
- Verificación de fórmulas con valores conocidos.
- Prueba de robustez básica para opción inválida.
- Confirmar que el programa puede iterar y salir sin errores.

## Casos de prueba
| entrada | esperado | éxito |
|---|---|---|
| Opción `1`, valor `0` | Resultado `32 F` | Sí, coincide exactamente |
| Opción `1`, valor `100` | Resultado `212 F` | Sí, coincide exactamente |
| Opción `2`, valor `32` | Resultado `0 C` | Sí, coincide exactamente |
| Opción `2`, valor `212` | Resultado `100 C` | Sí, coincide exactamente |
| Opción `9` | Mensaje de opción inválida y retorno al menú | Sí, no se cierra abruptamente |
| Opción `3` | Mensaje de salida y fin del programa | Sí, termina con código de éxito |
