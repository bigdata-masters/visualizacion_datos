<p align="right">
  <a href="./README.md">
    <img alt="Español" src="https://img.shields.io/badge/ES-Español-blue">
  </a>
  <a href="./README.en.md">
    <img alt="English" src="https://img.shields.io/badge/EN-English-lightgrey">
  </a>
</p>

# Visualización de datos - Análisis de Principales Causas de Muerte en el Mundo
## Descripción

Este dashboard fue diseñado con el objetivo de visualizar las principales causas de muerte en el mundo, considerando únicamente aquellas que representan el 0.5 % o más del total de muertes globales.

Las causas con menor incidencia se agruparon en una categoría llamada “Others”, permitiendo una representación más limpia y comparativa.
El enfoque principal fue lograr una visualización clara, legible y minimalista que facilitara la interpretación rápida de los datos.

## 🧰 Herramientas utilizadas
<code><img title="Power BI" alt="power bi" width="40px" src="https://raw.githubusercontent.com/microsoft/PowerBI-Icons/f1d4dd6cd52338a186f58bc29c437f64cf6b327b/SVG/Power-BI.svg" /></code>

## Dataset
Variables principales:
- Cause of death or injury → Causa de muerte o lesión.
- Percent of total deaths → Porcentaje del total de muertes (rango 0–1).
- Deaths annual % change → Variación porcentual anual de las muertes (rango -1 a 1).

## Proceso de análisis y diseño
1. Filtrado de causas relevantes
    - Se incluyeron solo las causas de muerte con una contribución ≥ 0.5 % del total global.
    - Las demás se agruparon en una categoría “Others” mediante medida condicional (IF + GROUP BY).

2. Visualización principal, gráfico de dispersión (scatter plot) que representa:
    - Eje X: Variación anual de muertes (Deaths annual % change).
    - Eje Y: Porcentaje del total de muertes (Percent of total deaths).
    - Etiquetas: Causa de muerte.

3. Comparación visual
    - Permite identificar de forma inmediata qué causas tienen mayor proporción y si presentan una tendencia al alza o a la baja.
    - Se utilizaron colores neutros para mantener limpieza visual y destacar valores positivos o negativos.

4. Interactividad y precisión
    - Se añadieron tooltips para mostrar los valores exactos de porcentaje y variación anual.
    - La escala de ejes se ajustó al rango de datos reales para evitar distorsión.

## Resultados e insights
Las principales causas de muerte global fueron:
- Ischemic heart disease
- Stroke
- Chronic obstructive pulmonary disease

Se identificaron patrones negativos y positivos de variación anual:
- Causas como infecciones respiratorias y diarreas mostraron reducción.
- Algunas enfermedades no transmisibles (como cáncer o Alzheimer) mantuvieron crecimiento leve.
- La categoría “Others” agrupa causas con muy baja incidencia (< 0.5 %).

<p align="center">
  <img src="/assets/causes_of_death.png" alt="causas_de_muerte" />
</p>
<p align=center><em>Figura 1. Causas de muerte</em></p>

## ⚙️ Autores:
- [Alonso Ismael Camarena](https://www.linkedin.com/in/camarenaai/)
- [Erick Martinez Blas](https://www.linkedin.com/in/erick-martinez-blas/)