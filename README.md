# RappiPlus | Análisis de negocio y visualización de datos

Proyecto final del bootcamp de Análisis de Datos de TripleTen. Se evalúa el desempeño comercial de RappiPlus mediante limpieza de datos, análisis de rentabilidad, embudo de conversión, retención por cohortes, experimentación estadística y un dashboard en Power BI.

## Herramientas
Python, pandas, SQL (PostgreSQL), pruebas estadísticas y Power BI.

## Preguntas de negocio
- ¿Cómo se comportan los ingresos, costos y la ganancia estimada?
- ¿Qué productos y categorías requieren atención por su rentabilidad?
- ¿En qué etapa del proceso de compra se pierden usuarios?
- ¿Cómo evolucionan las cohortes de usuarios?
- ¿La modificación de la interfaz de checkout mejora la conversión?

## Hallazgos destacados
- **Ganancia estimada:** aproximadamente **2.92 millones**, después de costos de productos identificados e inversión en marketing. **No equivale a utilidad neta**, porque no incluye todos los gastos operativos.
- **Pedidos con pérdida:** 4,528 de 24,906 pedidos con costos identificados (**18.18 %**).
- **Embudo:** la mayor pérdida identificada fue entre `begin_checkout` y `add_payment_info`: **958 usuarios** (**13.29 %** respecto a la etapa anterior).
- **Prueba A/B:** conversión de **15.69 %** (control) frente a **16.29 %** (tratamiento), con **p = 0.4161**. No se encontró evidencia estadística suficiente para afirmar una mejora al nivel de significancia de 5 %.

## Archivos
- [`RappiPlus_analisis.ipynb`](RappiPlus_analisis.ipynb): análisis en Python y SQL, metodología y conclusiones.
- [`RappiPlus_dashboard.pbix`](RappiPlus_dashboard.pbix): dashboard interactivo en Power BI Desktop.

## Notas de reproducibilidad
El notebook utiliza datasets educativos de TripleTen. Algunas consultas requieren acceso a una base de datos del entorno de formación; por seguridad, la contraseña **no está incluida** en este repositorio. Para ejecutar esa sección, configure la variable de entorno `RAPPIPLUS_DB_PASSWORD` con credenciales autorizadas. El dashboard puede requerir ajustar rutas o conexiones de origen de datos en Power BI Desktop.

## Alcance
Proyecto académico con fines de portafolio. Los indicadores y conclusiones corresponden al conjunto de datos del ejercicio y no representan resultados financieros auditados de una empresa real.
