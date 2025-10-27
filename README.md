Este proyecto realiza un análisis exploratorio y de componentes principales (PCA) utilizando los datos del Varieties of Democracy (V-Dem Project), un conjunto de indicadores globales sobre democracia y gobernanza. Coppedge, Michael et al. (2023). Varieties of Democracy (V-Dem) Project Dataset v13. University of Gothenburg.

Objetivo general

El objetivo principal es examinar la distribución del índice de poliarquía (v2x_polyarchy), que mide el grado de democracia electoral en los países, y explorar su relación con otros indicadores institucionales y de derechos humanos a través de un Análisis de Componentes Principales (PCA).

Objetivos específicos

1.Explorar la distribución del índice de poliarquía a nivel global.
2.Evaluar la normalidad y variabilidad de los datos.
3.Calcular medidas descriptivas básicas (media, mediana, desviación estándar, cuartiles y percentiles).
4.Aplicar un PCA para identificar dimensiones latentes comunes entre indicadores institucionales y de derechos humanos.
5.Visualizar la varianza explicada y las cargas factoriales de los componentes principales.

Variables utilizadas

Variable dependiente:

1.v2x_polyarchy: Índice de poliarquía (nivel de democracia electoral).

Variables independientes:

1.v2x_rule: Estado de derecho
2.v2x_jucon: Independencia judicial
3.v2xcl_rol: Cumplimiento de la ley por parte del ejecutivo
4.v2jupurge: Purga de jueces
5.v2pepwrsoc: Distribución equitativa del poder social
6.v2xeg_eqdr: Igualdad de recursos
7.v2xeg_eqaccess: Igualdad de acceso a la educación
8.v2clkill: Asesinatos políticos
9.v2cltort: Tortura
10.v2csreprss: Represión civil


Flujo del análisis

1.Carga de datos:
Los datos se obtienen directamente desde el paquete vdemdata.

2.Análisis descriptivo:

-Histograma y densidad del índice de poliarquía.
-Boxplot para visualizar concentración de valores.
-Test de normalidad (Anderson-Darling).
-Cálculo de media, mediana, desviación estándar, coeficiente de variación, cuartiles y percentiles.

3.Análisis de Componentes Principales (PCA):

-Selección de variables institucionales.
-Normalización y reducción de dimensionalidad mediante prcomp().
-Visualización de varianza explicada (fviz_eig) y cargas factoriales.
-Interpretación de las dimensiones latentes.
