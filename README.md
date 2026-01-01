# Pokemon-Team
Este proyecto analiza datso reales de Pokémon para construir el equipo Pokémon definitivo de un tipo determinado, utilizando técnicas de webs craping, consumo de APIs, visualización de datos y procesamiento del lenguaje natural (NLP) con Python.

El análisis se limita a los 250 primeros Pokémon de la Pokédex (I-II Gen) y permite seleccionar equipos ofensivos, defensivos y balanceados basándose en distintos criterios estadísticos y estratégicos.

## 🎯 Objetivos
* Extraer datos reales de Pokémon mediante APIs y web scraping
* Analizar estadísticas ofensivas y defensivas
* Construir:
  * Un equipo ofensivo
  * Un equipo defensivo
  * Un equipo con sinergias de tipos
  * Un equipo definitivo balanceado
* Visualizar los resultados mediante gráficos
* Aplicar NLP para clasificar movimientos defensivos a partir de sus descripciones
* Seleccionar los mejores ataques para cada Pokémon del equipo final

## 🛠️ Tecnologías y librerías utilizadas
* Python 3
* Google Colab
* ```requests```
* ```beautifulsoup4```
* ```pandas```
* ```numpy```
* ```matplotlib```
* ```seaborn```
* ```scikit-learn``` (para el modelo NLP)
* APIs públicas de Pokémon

## ▶️ Desarrollo del proyecto
1. **Extracción de datos**
   * Obtención de datos de Pokémon y movimientos mediante APIs
   * Complemento de información mediante web scraping
   * Filtrado a los primeros 250 Pokémon (I-II Gen)
3. **Equipo ofensivo**
   * Selección de 6 Pokémon priorizando → ataque especial (SPA), defensa (DEF), ataque (ATK)
   * Cálculo de poker máximo de daño → ```Poder = Ataque especial * Daño base del ataque más potente del tipo```
4. **Equipo defensivo**
   * Selección de 6 Pokémon priorizando → defensa (DEF), vida (HP), Ataque (ATK)
5. **Sinergias de tipos**
   * Identificación de Pokémon con doble tipo
   * Aplicación de un multiplicador (```x1.25```) al ataque especial si existe ventaja estratégica
6. **Equipo definitivo**
   * Selección del equipo más equilibrado combinando los análisis anteriores
   * Justificación razonada de la elección final
7. **Elección de ataques (NLP)**
  * Selección de los 4 mejores ataques por Pokémon
  * Priorización de ataques efectivos frente a debilidades
  * Clasificación automática de movimientos defensivos usando NLP
  * Para cada ataque se muestra → nombre, tipo, poder y descripción

## 📈 Resultados
Este proyecto permite:
* Comparar distintos equipos Pokémon de forma objetiva
* Visualizar métricas ofensivas y defensivas
* Aplicar técnicas de **data science y NLP** en un contexto práctico
* Obtener un equipo Pokémon óptimo basado en datos reales
