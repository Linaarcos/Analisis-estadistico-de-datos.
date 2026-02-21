# Análisis de Rentabilidad: Tarifas de Prepago Megaline

📝 Contexto del Problema
Megaline ofrece dos planes a sus usuarios, cada uno con diferentes límites de minutos, SMS y volumen de datos. La empresa necesita entender no solo quién gasta más, sino cómo consumen los servicios sus clientes. El reto consistió en procesar datos de 500 usuarios, corregir discrepancias técnicas (redondeos de llamadas y datos) y aplicar pruebas de hipótesis para tomar una decisión basada en datos y no en suposiciones.

🛠️ Tecnologías Utilizadas
Lenguaje: Python 3.x

Análisis de Datos: Pandas, NumPy

Estadística: SciPy (stats)

Visualización: Matplotlib, Seaborn

📊 Metodología
ETL & Limpieza: Carga de 5 datasets, corrección de tipos de datos y manejo de valores ausentes.

Ingeniería de Características: Creación de una tabla agregada por usuario y mes que calcula el consumo de llamadas, mensajes e internet.

Lógica de Negocio: Aplicación de las reglas de facturación de Megaline (redondeos específicos y cargos por excedentes).

Análisis Estadístico: Comparación de distribuciones de consumo mediante histogramas y diagramas de caja.

Pruebas de Hipótesis: Uso de pruebas t de Student (Welch’s t-test) para comparar ingresos entre planes y regiones geográficas.

## Conclusiones del Análisis
* **Validación Estadística**: Se confirmó mediante pruebas t de Student que el tipo de plan es un factor determinante en el ingreso promedio, a diferencia de la ubicación geográfica.
* **Comportamiento del Consumidor**: Los usuarios del plan económico (Surf) exceden sus límites con mayor frecuencia, pero el plan Ultimate sigue siendo el más rentable por usuario debido a su tarifa base.
* **Impacto**: Este análisis permite a Megaline optimizar su inversión publicitaria, priorizando la captación de clientes en el segmento de alto valor (Ultimate).

🚀 Resultados Clave
Rentabilidad por Plan: Se determinó que el plan Ultimate genera ingresos promedio significativamente mayores y más estables que el plan Surf.

Comportamiento de Excesos: Los usuarios del plan Surf tienden a exceder sus límites con mucha frecuencia, lo que genera cargos adicionales, pero estos no alcanzan a equiparar la rentabilidad del cargo fijo más alto del plan Ultimate.

Consistencia Regional: La prueba de hipótesis confirmó que no existe una diferencia significativa entre el ingreso promedio de los usuarios del área NY-NJ y el resto de las regiones, sugiriendo que el comportamiento de consumo es uniforme.

Conclusión de Negocio: Se recomendó a la empresa priorizar la publicidad del plan Ultimate, ya que ofrece una fuente de ingresos más alta y predecible por cada cliente captado.
