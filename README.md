Analisis Financiero Empresa: "PATITO AZUL"


Resumen:

El objetivo de este proyecto es aprovechar el poder del análisis de datos para mejorar la eficiencia operativa y respaldar la toma de decisiones estratégicas en la empresa el pato azul. Mediante el análisis de conjuntos de datos internos financieros relevantes, se busca identificar patrones, tendencias y relaciones ocultas que puedan proporcionar información valiosa para mejorar la eficiencia, optimizar los procesos y brindar una ventaja competitiva.

Objetivos del Proyecto:

1.	Recopilar, limpiar y estructurar los datos relevantes disponibles en la empresa, incluyendo fuentes internas y externas pertinentes.
2.	Realizar un análisis exploratorio de los datos para identificar patrones, correlaciones y tendencias significativas.
3.	Diseñar paneles interactivos y visualizaciones claras para presentar los resultados del análisis de manera comprensible y accesible para los diferentes equipos y niveles de la organización.
4.	Realizar el estado de resultados financieros del 01 de enero al 31 de diciembre del 2020
5.	Proponer recomendaciones concretas basadas en los resultados del análisis para mejorar la eficiencia operativa, reducir costos, optimizar los recursos y respaldar la toma de decisiones estratégicas.

Entregables Esperados:

1.	Un conjunto de datos limpios, estructurados y preparados para el análisis en excel.
2.	Informes y visualizaciones que presenten los hallazgos y recomendaciones de manera clara y concisa que respondan las siguientes preguntas:
    - El top 5 de costos de venta más elevados
    - Top 10 de gastos Operativos 
    - Que 5 meses son en los que más se vendieron. 
    - Que 2 meses son en los que menos se vendieron.

3.	Estado de resultados.
4.	Recomendaciones concretas y accionables para mejorar la eficiencia operativa y respaldar la toma de decisiones.

Recursos Utilizados:
  1)	Excel
  2)	Driver Snowflake

Recursos de datos:
  1)	JSON ( GASTOS DE VENTA )
  2)	SQL ( VENTAS )
  3)	SNOSFLAKE ( GASTOS OPERATIVOS )

Para elaborar el estado de resultado necesitamos poder llegar a obtener la utilidad neta sin llegar a algo mas detallado guiarse por el siguiente cuadro

        VENTAS:	SUM(VENTAS)
        COSTO VENTAS:	SUM(COSTO VENTAS)
        UTILIDAD BRUTA:	VENTAS-COSTO DE VENTAS
        GASTOS OPERATIVOS:	SUM(GASTOS OPERATIVOS)
        UTILIDAD OPERACIONAL:	UTILIDAD BRUTA - GASTOS OPERATIVOS
        ISR 1 TRIMESTRE:	SUM(ENE,FEB,MAR) *0.28
        ISR 2 TRIMESTRE:	SUM(ABR,MAY,JUN) *0.28
        ISR 3 TRIMESTRE:	SUM(JUL,AGO,SEP) *0.28
        ISR 4 TRIMESTRE:	SUM(OCT,NOV,DIC) *0.28
        UTILIDAD NETA:	UTILIDAD OPERACIONAL - SUM(ISR TRIMESTRE 1,2,3,4)
