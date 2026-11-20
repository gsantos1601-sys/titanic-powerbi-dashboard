# 🚢 Titanic: Análisis de Supervivencia (Power BI)

Dashboard interactivo en Power BI que analiza la supervivencia de los **891 pasajeros** del Titanic según clase del boleto, género, edad y puerto de embarque.

![Dashboard completo](Dash%20imagenes%20PB/dashboard.png)

## 🔎 Hallazgos principales

- **38.38%** de los pasajeros sobrevivió (342 de 891).
- **Género:** sobrevivió el **74.20%** de las mujeres frente al **18.89%** de los hombres.
- **Clase:** la tasa de supervivencia fue de **62.96%** en Primera clase, **47.28%** en Segunda y **24.24%** en Tercera.
- **Efecto combinado:** en Tercera clase sobrevivió el 50% de las mujeres, mientras que en Primera clase solo el 36.89% de los hombres.

## 🎛️ Interactividad

Los segmentadores (slicers) de **género**, **puerto de embarque** y **clase del boleto** filtran todo el dashboard: tarjetas, gráficos y dispersión.

| Hombres | Mujeres |
|---|---|
| ![Filtro femenino](Dash%20imagenes%20PB/dashboard-filtrado-femenino.png) | ![Filtro masculino](Dash%20imagenes%20PB/dashboard-filtrado-masculino.png) |

## 📊 Visualizaciones

- Tarjetas KPI: pasajeros, sobrevivientes, fallecidos y sus tasas.
- Columnas agrupadas: tasa de supervivencia y de fallecidos por clase.
- Dona: estado de supervivencia.
- Circular: sobrevivientes por género.
- Dispersión: edad vs. tarifa por clase.

## 🛠️ Herramientas

- Power BI Desktop
- DAX (medidas y columnas calculadas)
- Segmentadores, formato condicional y diseño con tema oscuro

## 🧮 Ejemplo de medidas DAX

```dax
Tasa de supervivencia = [Sobrevivientes] / [Pasajeros]

Tasa por grupo = AVERAGE('Titanic-Dataset'[Survived])

Tasa de fallecidos por grupo = 1 - AVERAGE('Titanic-Dataset'[Survived])
```

## 📁 Contenido del repositorio

- `Dash imagenes PB/`: capturas del dashboard (completo y filtrado).
- `titanic_dashboard.pbix`: archivo de Power BI (ábrelo con Power BI Desktop, es gratuito).
- `data/`: dataset utilizado.

## 📚 Dataset

Titanic

## 👤 Autor

**Gerardo Narvaez De Los Santos** · [LinkedIn]([https://www.linkedin.com/in/tu-perfil](https://www.linkedin.com/in/gerardo-narvaez-abb24a371/))
