📬 Autor:
Michael Paul Collado Morales  
📍 Arequipa, Perú  
📧 michael.collado@outlook.com  
🔗 LinkedIn: https://www.linkedin.com/in/michaelpaulcm  

🎯 Propósito del proyecto
Portafolio de **Business Intelligence con Power BI**: modelado dimensional, **DAX avanzado**, dashboards ejecutivos y análisis accionables sobre ventas, productos, canales, geografía y calendario.  
Dirigido a roles como:
- Data Analyst
- Business Intelligence Analyst
- Process Analyst
- Business Analytics / Reporting
- Data-Driven Operations

▶️ Power BI portfolio – Dashboards, DAX y modelo estrella
Este portafolio demuestra:
- Diseño de **modelo estrella** (dimensiones de producto, tienda, canal, geografía y calendario; hecho de ventas).
- Uso avanzado de **DAX** para KPIs, comparativas interanuales, ranking, parámetros y storytelling.
- **Visualizaciones interactivas** con tooltips, bookmarks y segmentación por filtros.

🗂 Contenido del repositorio
01-PowerBI-Portafolio/
- 01-Proyecto_DAX_v1.pdf  ← Documentación y capturas de dashboards
- Enlace de descarga del PBIX y Bse de datos: https://drive.google.com/drive/folders/1Pf_XlWlxIIfev5NUEz1iPMUhpJU86ZO1?usp=sharing

🧱 Modelo de datos (esquema estrella)
- DimProductCategory(ProductCategoryKey, ProductCategoryName)  
- DimProductSubcategory(ProductSubcategoryKey, ProductSubcategoryName)  
- DimProduct(ProductKey, ProductName, BrandName, ClassName, ColorName, Manufacturer, ProductDescription)  
- DimGeography(GeographyKey, City, StateProvinceName, CountryRegionName)  
- DimStore(StoreKey, StoreName, StoreType, Manager, Address, GeographyKey, EmployeeCount, SellingAreaSize)  
- DimChannel(ChannelKey, ChannelName)  
- DimPromotion(PromotionKey, PromotionName, PromotionCategory, DiscountPercent, EndDate)  
- DimCalendar(DateKey, Date, DayNumberOfWeek, DayName, WeekNumberOfYear, Month, MonthName, Quarter, Semester, Year)  
- FactSales(DateKey, ProductKey, StoreKey, PromotionKey, ChannelKey, SalesQuantity, SalesAmount, ReturnQuantity, ReturnAmount)  
- Tablas auxiliares y medidas DAX (SUMMARIZECOLUMNS, CALCULATE, SUMX, DIVIDE, FILTER, RANKX, SWITCH, FORMAT, CONCATENATEX, VAR/RETURN, ALL, ALLSELECTED, VALUES, RELATED, USERELATIONSHIP, CROSSFILTER, REMOVEFILTERS, ISFILTERED, HASONEVALUE, ISBLANK, operadores lógicos)

🛠 Funciones y técnicas aplicadas (DAX y visualizaciones)
- F. Fecha: extracción y uso de campos temporales (año, trimestre, mes).
- F. IF, OR/||, AND/&&: lógica condicional y combinaciones de filtros.
- F. CONCAT, UPPER, LOWER: rotulación y títulos dinámicos.
- F. RELATED: navegación entre dimensiones para cálculos por relación.
- F. DIVIDE, AVERAGE: ratios y promedios robustos (DIVIDE contra división por cero).
- F. COUNT, COUNTA, COUNTROWS, COUNTBLANK: conteos y control de vacíos.
- F. CALCULATE: cambio de contexto, métricas acumuladas y comparativas.
- F. FILTER: filtrado controlado para KPIs y condiciones de negocio.
- F. SUM, SUMX: agregación directa y fila a fila.
- F. DATEYTD, TOTALYTD: acumulado anual (YTD) por contexto de tiempo.
- F. SAMEPERIODLASTYEAR, DATEADD: comparativas YoY y desplazamientos de fecha.
- F. RANKX (ALL, ALLSELECTED), ISBLANK: ranking global y por selección, supresión de vacíos.
- F. SWITCH, HASONEVALUE, UNICHAR: categorización, control de unicidad y estrellas/íconos.
- F. Crear tabla, ISFILTERED: tablas auxiliares y medidas dependientes de filtros (ej. cambio de moneda).
- F. Parámetro de ajuste: intervalos numéricos para simular escenarios (ej. +10% ingresos).
- Tooltips personalizados: páginas dedicadas como información contextual.
- Bookmarks y botones: navegación de páginas y vistas guardadas.
- Gráficas de barras y comparativas: ingresos, utilidades, variaciones y distribución por región/producto.

📊 Principales KPIs y vistas
- Ingresos ajustados vs año anterior por año/mes/trimestre.
- Utilidad ajustada, margen y variaciones interanuales (YoY).
- Ranking de tiendas y categorías (ALL vs ALLSELECTED) con control de blancos.
- Distribución geográfica y por subcategorías (Top-N, estrellas via UNICHAR).
- YTD/MTD y series temporales con métricas acumuladas.
