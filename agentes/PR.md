## Qué aporto

Una regla para el especificador: en encuestas por muestreo con factor de expansión, toda cifra sobre la población se pondera con ese factor, y el conteo de filas se informa aparte como tamaño de muestra.

**Tipo de aporte:** regla para la ficha de un subagente (`agentes/02-especificador.md`) + lección (`baterias/lecciones.json`).

## Evidencia

Caso real, de un análisis en clase de la GEIH 2025 del DANE (módulo de datos del hogar y la vivienda, noviembre 2025, 24.724 hogares). Comparación entre contar filas y ponderar con `FEX_C18`:

| Indicador | Contando filas | Ponderado |
|---|---|---|
| Hogares de Bogotá D.C. | 3,5 % | 17,1 % |
| Hogares rurales | 12,6 % | 21,4 % |
| Cocinan con leña | 5,5 % | 9,4 % |
| Estrato 1 | 36,2 % | 32,1 % |

Solo hay cifras agregadas: ninguna fila de datos ni datos personales.

**Es un hueco:** ninguna ficha de `agentes/` ni `negocio.md` menciona encuestas, ponderación ni factor de expansión. Hoy el especificador podría pedir porcentajes contando filas, y el resultado describiría la muestra en vez de la población.

## Su prueba

Es una regla de ficha, así que **requiere prueba de efecto** (la hace el dueño). La lección `L-aporte-ponderacion-encuestas` apunta a esta regla; el id es provisional para que el dueño lo renumere.

## Resultado del filtro sin IA

```
✓ pasa el filtro automático. Sigue la revisión del dueño.
RESUMEN {"fallas": [], "avisos": []}
```

## Antes de enviar

- [x] No incluye datos personales, datos de SECOP ni archivos de datos de más de 200 KB.
- [x] No corrí el flujo completo con agentes: no hace falta (la prueba con IA la hace el dueño, con su licencia).
- [x] Si agrego código, solo usa la biblioteca estándar y lo de `herramientas/permitidas.json`. (No agrega código.)
- [ ] Acepto que mi usuario de GitHub aparezca en el registro de cambios si el aporte se acepta.
