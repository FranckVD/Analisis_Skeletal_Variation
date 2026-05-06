# 🦴 Variación Esquelética: Análisis Comparativo de Huesos en Vertebrados

## Descripción

Este proyecto explora los huesos del cuerpo humano y los compara con los de una amplia variedad de mamíferos y aves, usando Python y pandas. A través del análisis de datos reales, se verifican afirmaciones populares sobre la anatomía humana y se descubren patrones evolutivos fascinantes en el esqueleto de los vertebrados.

## Objetivos

- Analizar la distribución de huesos en el cuerpo humano adulto
- Verificar la afirmación de que más de la mitad de los huesos están en manos y pies
- Explorar el proceso de fusión ósea de bebé a adulto
- Comparar el número de vértebras cervicales entre humanos, mamíferos y aves

## Hallazgos principales

| Pregunta | Hallazgo |
|---|---|
| ¿Más del 50% de huesos en manos y pies? | ✅ Verdadero: 106 de 206 huesos (51.5%) |
| ¿Cuántos huesos tienen los bebés? | 305 huesos (se fusionan hasta llegar a 206) |
| ¿Vértebras cervicales en mamíferos? | 7 en casi todos (excepto manatíes y perezosos) |
| Ave con más vértebras cervicales | Cisne mudo: 23 vértebras |
| Ave con menos vértebras cervicales | Guacamayo azul y amarillo: 10 vértebras |
| ¿Brazos o piernas con más huesos? | Piernas (8) > Brazos (6) |
| ¿Cuántas costillas tienen los humanos? | 24 costillas |

## Tecnologías utilizadas

- **Python 3**
- **pandas** — carga, filtrado y análisis de datos
- **Matplotlib** — visualización con gráfico de barras

## Archivos del proyecto

```
📁 skeletal-variation/
├── skeletal-variation.ipynb       # Notebook principal con el análisis
├── adult-human-skeleton.csv       # Datos de los 206 huesos del cuerpo humano
├── mammal-neck-bones.csv          # Vértebras cervicales de 302 mamíferos
├── bird-neck-bones.csv            # Vértebras cervicales de diversas aves
└── README.md
```

## Cómo ejecutar

### Opción 1 — Google Colab (recomendado)
1. Abre `skeletal-variation.ipynb` en [Google Colab](https://colab.research.google.com/)
2. Descomenta la celda de carga de archivos al inicio del notebook
3. Sube los tres archivos CSV cuando se lo solicite
4. Ejecuta las celdas en orden

### Opción 2 — Local
```bash
# Clona el repositorio
git clone https://github.com/tu-usuario/skeletal-variation.git
cd skeletal-variation

# Instala dependencias
pip install pandas matplotlib jupyter

# Abre el notebook
jupyter notebook skeletal-variation.ipynb
```

## Estructura del análisis

1. **Carga de datos** — Importación del CSV del esqueleto humano con pandas
2. **Afirmación: manos y pies** — Verificación con `value_counts()`
3. **Huesos de bebé** — Fusiones óseas con `sort_values()` y `sum()`
4. **Cuello humano** — Filtrado con `query()` para identificar las 7 vértebras cervicales
5. **Mamíferos** — Comparación de 302 especies; se identifican excepciones (manatíes y perezosos)
6. **Aves** — Análisis de distribución con gráfico de barras; mayor diversidad cervical

## Extensiones realizadas

Además del análisis principal, se resolvieron las siguientes preguntas extra:

- 🦜 **Ave con menos vértebras:** Guacamayo azul y amarillo (10 vértebras)
- 💪 **Brazos vs. piernas:** Las piernas tienen más huesos (8 vs. 6)
- 🫀 **Costillas humanas:** 24 costillas en total

## Autor

> Agrega aquí tu nombre, perfil de LinkedIn o correo de contacto.

## Licencia

Este proyecto es de uso educativo y está disponible bajo la licencia [MIT](LICENSE).
