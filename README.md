# Análisis de Rentabilidad y Gestión de Inventarios de Xileno en Refinería Venezolana

##Resumen

Este proyecto abordó el problema de un excedente de inventario de Xileno en una refinería venezolana, que inmovilizaba capital y generaba riesgos operativos. Se demostró que un descuento estratégico del 6% permitiría liquidar el 97% del inventario sobrante de 500 galones mensuales. Esta estrategia no solo resolvería el problema de inventario, sino que también aseguraría un margen de ganancia del 14.89%, superando la meta financiera del 12% establecida por la empresa. A pesar de que descuentos mayores pueden reducir el margen de ganancia, una aplicación precisa y un entendimiento de la demanda permiten maximizar la rentabilidad mientras se optimiza la gestión del inventario.

##Problema de negocio

Una de las principales refinerías de Venezuela distribuye combustibles (Gasolina, Gasoil, Querosén), lubricantes (aceite hidráulico y de motor) y petroquímicos (Xileno) a todo el país mediante camiones cisternas y tuberías. Actualmente presenta un excedente de Xileno en sus inventarios, lo cual representa capital inmovilizado y riesgos operativos. La refinería necesita liquidar este stock de manera urgente a través de la distribución por tubería. El desafío principal es hacerlo sin que el margen de ganancia de esta operación caiga por debajo del 12%, una métrica financiera clave para la empresa.

##Metodología

La fase inicial consistió en la preparación y limpieza de los datos. Posteriormente se crearon variables claves para el análisis de la rentabilidad e inventarios de producto, entre ellas precio de venta (sales_price), ganancias (profit) y descuento (discount) a partir de los datos de origen. 

En la segunda fase se llevó a cabo un Análisis Exploratorio de Datos (EDA) para ver el comportamiento de las ventas y la ubicación del producto en estudio (Xileno) con respecto a los demás productos. Además de determinar si existe una relación entre las variables numéricas y identificar patrones de aplicación de descuentos.

La tercera fase se concentró en analizar los galones de Xileno vendidos mediante distribución por tubería y la influencia que tuvo la aplicación de descuentos, con la finalidad de incrementar el volumen de Xileno vendido y desalojar un inventario sobrante de 500 galones mensuales. Se complementó esta etapa con otras segmentaciones de datos para proporcionar una visión del mercado o clientes a los cuales se les pueda ofertar mayor volumen de Xileno. Por último se proporcionó un calculo de elasticidad precio de demanda (PED) para estimar los galones de Xileno vendidos si se aplicara un descuento mayor y el margen de rentabilidad estimado.

![esquema_metodologia](https://github.com/user-attachments/assets/ee89fd40-53dc-4a6c-b2df-1bea1fb71a6e)


##Skills:

- Python (Pandas, Matplolib, Seaborn)
- ERP: SAP para extracción de dataset.

##Resultados y Recomendaciones

- El Xileno ocupa el 3er lugar en volumen de combustibles vendidos (693,5 MGal) y el primer lugar en ventas totales en dólares (29.2 MM$) en la refinería con respecto a los demás productos. Además, es el producto con mayores ventas en los 3 principales consumidores (comercial, domestico e industrial) y en el tipo de entrega (por tubería y camiones cisternas).
- No se encontró un patrón o tendencia definida de aplicación de descuentos, la refinería tiene sus políticas de acuerdo a la oferta y demanda del mercado para establecer porcentajes de descuento en los productos.
- Se encontró una correlación de 0.59 entre la cantidad (en galones) y el descuento aplicado.
- Al segmentar solo el Xileno los resultados fueron los siguiente: mayores descuentos generaron que el numero de ordenes de ventas y el margen de ganancia disminuyera hasta un valor de 15,79% para un 5% de descuento (Tabla 2.2), sin embargo se obtuvo un aumento en el volumen de Xileno vendido (Gráfico 2.3).  
- Las regiones que han comprado mayor volumen de Xileno con respecto porcentaje de descuento aplicado son Oriente (East) y Occidente (West), gráfica 2.4. Y dentro de los clientes que han incrementado la compra de galones de Xileno con mayores porcentajes de descuento, destacan el Comercial y el Doméstico, gráfica 2.5.
- Del año 2022 al año 2023 la cantidad de ordenes, galones de Xileno y el promedio de descuento ponderado por galones, aumentó de 190 a 203, de 66.700 a 70.700 y de 3.55& a 3.65&, respectivamente (Gráfica 2.6).
- Tomando en cuenta la segmentación realizada por año, los cálculos basados en el año 2023 (Tabla 2.4), arrojaron un PED de 26.4% entre los porcentajes de descuento de 4% a 5% y, al incrementar el porcentaje de descuento a 6% se podrían vender 27.808 galones de Xileno anuales, lo que representa un incremento de 5.808 galones con respecto al descuento de 5%, es decir, aumentar a 484 galones mensuales, con lo cual se estarían desalojando 97% del inventario sobrante (500 galones).
- Con un 6% de descuento el margen de ganancia sería de 14.89%, mayor al 12% requerido por la empresa. 
- Se recomienda: comenzar aplicando el descuento de acuerdo a las tendencias obtenidas en la segmentación por regiones y por cliente.

##Próximos pasos: 
- Segmentar otros productos para observar comportamientos con respecto a los descuentos.
- Realizar un modelo de predicción con un equipo de científicos de datos.


