# Práctica 6 · AHPSort II: nivel de seguridad por provincias

**Sistemas de Ayuda a la Decisión · Universidad de Jaén**
**Autor:** Samuel Muñoz Millán

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/smmdev/SAD-P6-AHPSort/blob/main/AHPSort_P6.ipynb)

Clasificación de las provincias españolas en tres niveles de seguridad (Alto, Medio y Bajo) según sus datos de criminalidad, con el método AHPSort II, y representación de los resultados en mapas.

## Cómo ejecutarlo

### En Google Colab
1. Pulsar el botón **Abrir en Colab** de arriba.
2. Menú **Entorno de ejecución → Ejecutar todas**.

La primera celda descarga este repositorio (datos y mapas) e instala lo que falte.

El cuaderno ya está ejecutado y guardado con todas sus salidas, así que los resultados se pueden consultar en GitHub sin ejecutarlo.

### En local
```bash
git clone https://github.com/smmdev/SAD-P6-AHPSort
cd SAD-P6-AHPSort
pip install -r requirements.txt
jupyter notebook AHPSort_P6.ipynb
```

## Contenido
| Carpeta / fichero | Descripción |
|---|---|
| `AHPSort_P6.ipynb` | Cuaderno con los cuatro ejercicios |
| `datos/` | Datos de criminalidad (Andalucía 2017, España 2017 y 2023) y población de las provincias |
| `mapas/andalucia/` | Provincias de Andalucía (shapefile) |
| `mapas/espana/` | Provincias de la Península, Baleares, Ceuta y Melilla (shapefile del IGN) |
| `mapas/canarias/` | Provincias de Canarias (GeoJSON) |
| `resultados/` | Tablas (CSV) y mapas (PNG) generados al ejecutar el cuaderno |

## Ejercicios
1. Andalucía con datos absolutos.
2. Andalucía con datos por cada 10.000 habitantes.
3. España (50 provincias), 2017.
4. España, 2023, con la calibración de 2017: mapas comparados, tabla de transición y matriz de cambios.

## Fuentes de los mapas
- Andalucía y España (sin Canarias): ficheros proporcionados con el enunciado de la práctica.
- Canarias: `spain-provinces.geojson` del proyecto [click_that_hood](https://github.com/codeforgermany/click_that_hood).
