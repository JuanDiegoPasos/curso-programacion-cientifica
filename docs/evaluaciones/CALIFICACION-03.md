# Retroalimentación — Taller evaluativo 03 (NumPy)

**Estudiante:** Juan Diego Pasos Gómez · **Taller:** Taller evaluativo 03 — NumPy
**Fecha límite:** 2026-10-30 23:59 · **Versión revisada:** commit `f7d3917`

Excelente trabajo: todos los resultados coinciden con los esperados.

## Nota

| Criterio | Puntos |
|---|---|
| Creación y atributos de arreglos (Ej. 1) | 10 / 10 |
| Indexación y slicing (Ej. 2) | 10 / 10 |
| Máscaras booleanas (Ej. 3) | 15 / 15 |
| Vectorización y broadcasting (Ej. 4) | 15 / 15 |
| Estadística por eje y funciones universales (Ej. 5 y 6) | 20 / 20 |
| Integración (Ej. 7) | 10 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 4 / 5 |
| Entrega correcta | 1 / 5 |
| **Total** | **95 / 100** |
| **Nota (0–5)** | **4.75** |

Este taller aporta **14.3 %** de los 15 % del momento evaluativo.

## 1. Creación y atributos de arreglos (10 / 10)
**Lo que hizo bien:** creó `lecturas_crudas` con `np.array` a partir de una lista de listas, leyó forma, dimensiones, total y tipo de sus atributos, y creó `dias`, `pendientes` e `interceptos` correctamente.

## 2. Indexación y slicing (10 / 10)
**Lo que hizo bien:** cada resultado sale de una sola expresión, usó el índice negativo donde se pedía y el `bloque` tiene forma (3, 4).

## 3. Máscaras booleanas (15 / 15)
**Lo que hizo bien:** `es_util` une las dos comparaciones con `&` y paréntesis; quedaron 5 lecturas útiles, 2 faltantes y promedio 27.0, sin bucles.

## 4. Vectorización y broadcasting (15 / 15)
**Lo que hizo bien:** convirtió pendientes e intercepto en columnas, `calibradas` tiene la fila esperada, el promedio de SBC-A es 31.9 y la explicación del error de formas es clara.

## 5. Estadística por eje y funciones universales (20 / 20)
**Lo que hizo bien:** promedios por sensor y por día, máximos y media sobre el límite son correctos; usó `np.maximum`, `np.abs` y `np.round`, y `en_alerta` es una copia con 8 celdas en alerta sin alterar `calibradas`.

## 6. Integración (10 / 10)
**Lo que hizo bien:** los conteos 9, 18, 7 y 1 suman 35, el día pico es 5 y las dos líneas de salida coinciden con lo pedido. También hizo el reto opcional con `np.digitize`.

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:** el notebook corre completo sin errores y la celda de verificación quedó intacta.

## 8. Documentación (4 / 5)
**Lo que hizo bien:** los siete ejercicios tienen su celda de texto previa y los nombres siguen `snake_case`.
**Lo que puede mejorar:**
- La celda inicial tiene el título y su nombre, pero le falta la fecha.

**Cómo corregirlo:**
- Agregue la fecha de entrega en la celda de texto inicial, junto al título y su nombre.

## 9. Entrega correcta (1 / 5)
**Lo que hizo bien:** el trabajo está subido a GitHub antes del plazo.
**Lo que puede mejorar:**
- No siguió la estructura acordada: el notebook está en la raíz del repositorio y no en la carpeta `ejercicios/`.
- El nombre del archivo es `taller_evaluativo_03_numpy.ipynb` y debía ser `taller-evaluativo-03-numpy.ipynb` (con guiones, no guiones bajos).

**Cómo corregirlo:**
- Cree la carpeta `ejercicios/` en la raíz del repositorio y mueva allí el notebook.
- Cámbiele el nombre a `taller-evaluativo-03-numpy.ipynb`. Haga lo mismo con los talleres anteriores.

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación imprime "Verificación completada sin errores." y todos los resultados coinciden con los esperados.

## Para el próximo taller
- Cree la carpeta `ejercicios/` y use exactamente el nombre de archivo que indica la guía.
- Incluya la fecha en la celda inicial.
- Revise la lista de entrega de la guía antes de subir el archivo.
- Siga ejecutando "Reiniciar y ejecutar todas" antes de entregar, como lo hizo aquí.
