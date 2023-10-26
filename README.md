# quilmesRecommendations
Descripción
Este proyecto tiene como objetivo ajustar las recomendaciones de productos de Quilmes para cumplir con ciertas restricciones y objetivos de negocio. Utiliza datos de clientes, productos y recomendaciones previas para redistribuir las recomendaciones de manera que se adhieran a los criterios especificados.

Instrucciones de Uso
Carga de Datos: El script comienza cargando los datos necesarios de tres archivos Excel: clientes del último mes (customers_last_month.xlsx), recomendaciones actuales (recommendations.xlsx) y detalles de productos (products.xlsx).

Preparación de Datos:

Se calcula el total de recomendaciones por producto (product_desc).
Se combina esta información con el número de clientes del último mes y se calcula el ratio de recomendaciones por cliente.
Se agrega la información del segmento de marca (Premium o no) de cada producto.
Algoritmo de Ajuste de Recomendaciones:

Se asegura que "Brahma Dorada-1 Lts-Bottle-RET" tenga al menos 200 recomendaciones.
Se ajusta para que al menos el 20% del total de las recomendaciones sean de productos Premium.
Se ajustan las recomendaciones para que estén entre el 75% y el 200% del número de clientes del último mes.
Análisis de los Resultados:

Se ordenan los productos según la variación en el número de recomendaciones comparado con el número original.
Se exporta este análisis a un archivo CSV para su revisión y uso futuro.
Cálculo de Recomendaciones por Marca:

Se calcula el número total de recomendaciones por marca y se presenta en orden descendente.
Estructura del Código
El código se organiza en bloques funcionales que realizan tareas específicas, desde la carga de datos hasta la generación de análisis y reportes.

Personalización
Para adaptar el script a otros conjuntos de datos o criterios de ajuste, modifique los parámetros y rutas de archivo en la sección de carga de datos y los criterios específicos en la función ajuste_recomendaciones.

Contribuciones
Las contribuciones a este proyecto son bienvenidas. Por favor, siga las mejores prácticas de codificación y documentación al hacer modificaciones o adiciones.
