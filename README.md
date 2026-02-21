# Análisis de Rentabilidad: Tarifas de Prepago Megaline

Este proyecto analiza el comportamiento de consumo de usuarios de telecomunicaciones para optimizar el presupuesto publicitario basado en datos de ingresos.

## Herramientas Utilizadas
* **Python** (Pandas, NumPy)
* **Visualización**: Matplotlib, Seaborn
* **Estadística**: SciPy (Pruebas t de Student)

## Metodología
1. **Limpieza**: Ajuste de tipos de datos y redondeo según política de la empresa.
2. **Cálculo**: Agregación de consumo mensual e ingresos por usuario.
3. **Análisis**: Estudio de distribución, media y varianza por plan.
4. **Hipótesis**: Validación estadística de la diferencia de ingresos entre planes y regiones.

## Conclusiones del Análisis
* **Validación Estadística**: Se confirmó mediante pruebas t de Student que el tipo de plan es un factor determinante en el ingreso promedio, a diferencia de la ubicación geográfica.
* **Comportamiento del Consumidor**: Los usuarios del plan económico (Surf) exceden sus límites con mayor frecuencia, pero el plan Ultimate sigue siendo el más rentable por usuario debido a su tarifa base.
* **Impacto**: Este análisis permite a Megaline optimizar su inversión publicitaria, priorizando la captación de clientes en el segmento de alto valor (Ultimate).
