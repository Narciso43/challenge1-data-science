# Challenge 1 Data Science
Durante este desafío, ayudarás al Sr. Juan a decidir qué tienda de su cadena Alura Store debe vender para iniciar un nuevo emprendimiento. Para ello, analizarás datos de ventas, rendimiento y reseñas de las 4 tiendas de Alura Store. El objetivo es identificar la tienda menos eficiente y presentar una recomendación final basada en los datos.
 ## 🎯 **Propósito del Proyecto**

 **Ayudar al Sr. Juan a identificar cuál de sus 4 tiendas retail debería vender**, mediante análisis estratégico que evalúa:

1. 📈 **Rentabilidad** - Ingresos y márgenes de ganancia
2. 📊 **Desempeño Operativo** - Eficiencia logística y costos
3. ⭐ **Satisfacción Cliente** - Calificaciones promedio y reseñas
4. 🌍 **Potencial Geográfico** - Ubicación estratégica y densidad de ventas

---

### 🔍 **Criterios de Evaluación**
| Indicador               | Métrica Clave                          | 
|-------------------------|----------------------------------------|
| 🔴 Baja Rentabilidad    | <15% de contribución a ingresos totales |
| 🚫 Baja Rotación        | >40% de productos poco vendidos        |
| ⚠️ Insatisfacción       | Calificación promedio < 3.5/5          |
| 📍 Logística Costosa    | Costo de envío > promedio del sector    |
| 🌎 Ubicación Débil      | Baja densidad de ventas en mapa de calor|

---

## 📌 **Recomendación Final** 
**Tienda recomendada para venta: Tienda 4**  

✅ **Justificación técnica**:
bash
- 📉 14.9% de ingresos totales (más bajo)
- ⚠️ 3.1/5 en satisfacción cliente 
- 📦 $18.50 costo promedio de envío (+25% vs promedio)
- 🌎 Zona con alta competencia (ver heatmap)



**¿Como se Decidio?**

``` mermaid
graph TD
    A[Análisis Inicial] --> B{Evaluación Cuantitativa}
    A --> C{Evaluación Cualitativa}
    B --> D[Ranking Financiero]
    B --> E[Costos Operativos]
    C --> F[Feedback Clientes]
    C --> G[Análisis Geográfico]
    D & E & F & G --> H[Matriz de Decisión]
    H --> I[Recomendación Final]
```
```mermaid
graph TD
    A[Análisis Inicial]:::orange --> B{Evaluación Cuantitativa}:::purple
    A --> C{Evaluación Cualitativa}:::purple
    classDef orange fill:#FFA500,stroke:#333,stroke-width:2px;
    classDef purple fill:#9370DB,stroke:#333,stroke-width:2px;
```
```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'fontFamily': 'Segoe UI'}}}%%
graph TD
    A[("fa:fa-database Datos Brutos")]:::data --> B[/"fa:fa-filter Limpieza de Datos\n(Outliers, Missing Values)"/]:::process
    B --> C{"fa:fa-balance-scale Evaluación Estratégica"}:::decision
    C -->|Análisis Cuantitativo| D[["fa:fa-calculator Métricas Financieras<br>• ROI<br>• Margen Neto<br>• Costo Logístico"]]:::metrics
    C -->|Análisis Cualitativo| E[["fa:fa-users Feedback Clientes<br>• Calificaciones<br>• Reseñas<br>• Tendencias"]]:::feedback
    D --> F{{"fa:fa-chart-line Ranking Comparativo"}}:::analysis
    E --> F
    F --> G[/"fa:fa-map-marked-alt Geoanálisis<br>Heatmaps y Densidad"/]:::geo
    G --> H[("fa:fa-flag-checkered Recomendación Final")]:::result

    classDef data fill:#2980B9,stroke:#1B4F72,color:white,stroke-width:2px
    classDef process fill:#3498DB,stroke:#21618C,color:white,stroke-dasharray: 5 5
    classDef decision fill:#27AE60,stroke:#196F3D,color:white,shape:rhombus
    classDef metrics fill:#8E44AD,stroke:#6C3483,color:white,stroke-width:3px
    classDef feedback fill:#E74C3C,stroke:#943126,color:white
    classDef analysis fill:#F1C40F,stroke:#B7950B,color:black,shape:rect
    classDef geo fill:#16A085,stroke:#0E6251,color:white
    classDef result fill:#E67E22,stroke:#BA4A00,color:white,shape:cylinder

    click A "https://github.com/tuusuario/repo/blob/main/data/raw" "Ver datos originales"
    click H "#recomendacion-final" "Ir a conclusión"
```
## 2. La estructura del proyecto y organizacion de los archivos.
## 3. Ejemplos de gráficos  e insights obtenidos.
## 4 Intrucciones  para  ejecutar el notebook.
#recomendacion_final
## conclusion

