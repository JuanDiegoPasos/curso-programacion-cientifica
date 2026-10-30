# Retroalimentación — Taller evaluativo 02: Funciones y POO

**Estudiante:** Juan Diego Pasos Gómez · **Taller:** Taller evaluativo 02 — Funciones y POO
**Fecha límite:** 2026-10-30 23:59 · **Versión revisada:** commit `b62026e`

Muy buen trabajo en el código: todo funciona y los resultados son los esperados.

## Nota

| Criterio | Puntos |
|---|---|
| Funciones: parámetros, valores por defecto y retorno (Ej. 1 a 3) | 20 / 20 |
| `map`, `filter` y `lambda` (Ej. 4) | 10 / 10 |
| Clases, atributos y métodos (Ej. 5 y 7) | 15 / 15 |
| Encapsulamiento y validación (Ej. 6) | 15 / 15 |
| `__repr__` y `__str__` (Ej. 6 a 8) | 10 / 10 |
| Integración de funciones y clases (Ej. 8) | 10 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 1 / 5 |
| Entrega correcta | 1 / 5 |
| **Total** | **92 / 100** |
| **Nota (0–5)** | **4.60** |

Este taller aporta **13.8 %** de los 15 % del momento evaluativo.

## 1. Funciones: parámetros, valores por defecto y retorno (20 / 20)
**Lo que hizo bien:**
- `calibrar_lectura` tiene los valores por defecto en la firma, usa `return` y da 11.5 y 12.0 como se esperaba.
- `es_lectura_valida` clasifica bien -999.0, 600.0, 25.0 y 0.0.
- `promedio_valido` reutiliza `es_lectura_valida`, da 27.0 y devuelve `None` si no hay lecturas válidas, sin usar variables globales.

## 2. `map`, `filter` y `lambda` (10 / 10)
**Lo que hizo bien:**
- Obtuvo 5 lecturas calibradas (de 11.5 a 61.9) y 2 excedencias, sin bucles ni comprensiones.

## 3. Clases, atributos y métodos (15 / 15)
**Lo que hizo bien:**
- `Lectura` guarda sus tres datos con valores por defecto y convierte 0.0252 mg/m3 a 25.2 ug/m3.
- `Estacion` guarda objetos `Lectura` y `valores()` usa `a_microgramos()` sin tocar los atributos de cada lectura.

## 4. Encapsulamiento y validación (15 / 15)
**Lo que hizo bien:**
- `Sensor` lanza `ValueError` para código vacío y para pendiente menor o igual a cero, antes de guardar nada.
- La pendiente y el intercepto quedan como `_pendiente` y `_intercepto`, y `calibrar` reutiliza `calibrar_lectura`.
- No dejó celdas de prueba que fallen.

## 5. `__repr__` y `__str__` (10 / 10)
**Lo que hizo bien:**
- Los textos de `repr(sensor_a)`, `repr(estacion_oriente)` y `str(informe)` coinciden exactamente con lo pedido.
- `print(sensor_a)` muestra código, pendiente e intercepto en una línea clara.

## 6. Integración de funciones y clases (10 / 10)
**Lo que hizo bien:**
- `InformeEstacion` da promedio 31.9 y categoría "Moderada" reutilizando las funciones anteriores y el método `calibrar` del sensor.
- `categoria_pm25` usa una sola cadena `if` / `elif` / `else` y cubre las cuatro categorías.
- También resolvió el reto opcional de `excedencias` (da 2).

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo desde cero sin errores y la celda de verificación imprime el mensaje final.

## 8. Documentación (1 / 5)
**Lo que hizo bien:**
- Los nombres siguen `snake_case` y `PascalCase`, sin tildes.
- `es_lectura_valida` tiene su docstring.

**Lo que puede mejorar:**
- Antes de cada ejercicio solo hay un título ("Ejercicio 1", etc.); falta una explicación de lo que hace.
- Solo una función tiene docstring. Faltan en `calibrar_lectura`, `promedio_valido`, `categoria_pm25`, las clases `Lectura`, `Sensor`, `Estacion` e `InformeEstacion` y todos sus métodos.
- La celda inicial no trae la fecha.

**Cómo corregirlo:**
- Debajo de cada título de ejercicio, escriba una o dos frases sobre qué resuelve y qué resultado se espera.
- Agregue a cada función, clase y método una frase corta entre triples comillas, justo debajo de su primera línea, que diga qué hace.
- Agregue la fecha de entrega en la celda del título.

## 9. Entrega correcta (1 / 5)
**Lo lograron:** el notebook se subió a GitHub a tiempo.

**Lo que puede mejorar:**
- No siguió la estructura acordada: el notebook está en la raíz del repositorio y no en la carpeta `ejercicios/`.
- El nombre del archivo no es el exacto: usted usó `taller_evaluativo_02_funciones_y_poo.ipynb` (con guiones bajos).

**Cómo corregirlo:**
- Mueva el archivo a la carpeta `ejercicios/` y cámbiele el nombre a `taller-evaluativo-02-funciones-y-poo.ipynb` (con guiones medios). Haga lo mismo con los otros talleres.

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación imprime "Verificación completada sin errores." y todos los resultados coinciden con los esperados.

## Para el próximo taller
- Guarde el notebook en `ejercicios/` con el nombre exacto que pide la guía.
- Escriba una explicación breve antes de cada ejercicio.
- Ponga un docstring de una línea en cada función, clase y método.
- Incluya nombre completo y fecha en la primera celda.
