[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=OscarGR25210050/Practica1GD)

# Práctica 3: Liberación controlada de fármacos por hidrogeles

## Información del estudiante
Oscar González Ramírez \[M25210050]; m25210050@tectijuana.edu.mx

Gemelos Digitales

Maestría en Ciencias de la Ingenería

## Docente
Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura
La asignatura de Gemelos Digitales forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Formula el gemelo digital a través de datos experimentales para el desarrollo estrategias de control mediante teorías de sistemas dinámicos no lineales y la experimentación in silico. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional.

En el contexto de sistemas dinámicos que describen sistemas biológicos o fisiológicos, el modelizado in silico es una extensión lógica de la experimentación in vitro controlada, es el resultado natural del gran aumento de la potencia computacional disponible a un costo que disminuye continuamente, combinando las ventajas de la experimentación in vivo e in vitro, sin someterse a las consideraciones éticas y la falta de control asociadas con los experimentos in vivo. A diferencia de los experimentos in vitro, que existen de forma aislada, los modelos in silico permiten incluir un conjunto prácticamente ilimitado de variables y parámetros, lo que hace que los resultados sean más aplicables en problemas del mundo real. La experimentación in silico ha dado lugar al paradigma denominado como "gemelos digitales" (en inglés digital twins); en esencia, los gemelos digitales son una réplica o representación digital de un proceso o sistema del mundo real, donde por replica se refiere a un modelo computacional desarrollado con base en datos experimentales y características especiales que le permiten conectar lo físico con lo virtual con el propósito de mejorar el rendimiento de un sistema, detectar y prevenir fallas, y realizar predicciones sobre su respuesta ante diferentes estímulos o escenarios de operación; una definición más formal establece que: un gemelo digital es un conjunto de modelos adaptativos que emulan el comportamiento de un sistema físico en un sistema virtual obteniendo datos en tiempo real para actualizarse a lo largo de su ciclo de vida; replica al sistema físico para predecir fallas y oportunidades de cambio, prescribir acciones en tiempo real para optimizar y/o mitigar eventos inesperados observando y evaluando el perfil operativo del sistema. En el campo particular de la Biología de Sistemas, un gemelo digital se presenta como un algoritmo o conjunto de algoritmos computacionales desarrollados con base en modelos mecanicistas de un organismo vivo, esto con el objetivo de emular su fisiología para ilustrar su dinámica en el corto y en el largo plazo, así como predecir su respuesta a diferentes estímulos endógenos y exógenos.

## Objetivo y descripción del sistema
Determinar la tasa de liberación del hidrogel N36-2MBA3 con base en los datos experimentales de figura, denominada "datos_sistema.png".

Palabras clave: Bioestadísticos; Regresión no lineal; Experimentación in silico; Función de Peppas; Función farmacocinética.

## Actividades a realizar  
1. Utilizar Graph Grabber para encontrar los datos correspondientes a cada uno de los fármacos graficados en la figura 9 del artículo "PNVCL‐PEGMA nanohydrogels with tailored transition temperature for controlled delivery of 5‐fluorouracil" de M. A. González‐Ayón, J.A. Sañudo‐Barajas, L.A. Picos‐Corrales y A. Licea‐Claverie; donde el eje X es el tiempo medido en minutos y el eje y es la liberación cumulativa del fármaco como un porcentaje (%).
2. Desarrollar un algoritmo en MATLAB que permita realizar el procesamiento y graficado de los datos obtenidos.
3. Aplicar la función fitnlm de MATLAB para ajustar los datos mediante regresión no lineal utilizando las siguientes modelos:

a. Función de Peppas: x(t) = kt^n
  
b. Función farmacocinética de primer orden: x(t) = beta(1 - e^(-kt))
  
c. Una función obtenida con Eureqa, utilizando los datos obtenidos del gráfico para buscar soluciones para la ecuación f(x_1) = f(t)
  
d. Una ecuación diferencial ordinaria obtenida con Eureqa, utilizando los datos obtenidos del gráfico para buscar soluciones para la ecuación D(x_1,t,1) = f(x_1)

5. Desarrollar un algoritmo que, con ayuda de la función del punto pasado, refleje los bioestadísticos siguientes correspondientes para cada función: Error estándar, margen de error, intervalos de confianza del 95% y valor P; además de pruebas de bondad de ajuste como el coeficiente de determinación (R²), la suma residual de cuadrados (RSS) y el criterio de información de Akaike ajustado (AICc).
6. Gráficar el comportamiento de los modelos ajustados con respecto a los datos obtenidos para cada uno de los fármacos y guardar las figuras obtenidas como archivos .pdf.
## Lista de archivos incluidos en el repositorio
1. Cuaderno computacional de MATLAB [.mlx].
2. Imagénes de las simulaciones [.pdf].
3. Diagrama biológico del sistema [.png].
4. Archivo de datos utilizado en Eureqa para determinar las funciones [.fxp].

## Referencias
\[1] P. A. Valle, Syllabus para Gemelos Digitales, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

\[2] M. A. González‐Ayón, J.A. Sañudo‐Barajas, L.A. Picos‐Corrales, & A. Licea‐Claverie, "PNVCL‐PEGMA nanohydrogels with tailored transition temperature for controlled delivery of 5‐fluorouracil", Journal of Polymer Science Part A: Polymer Chemistry, vol. 53, issue 22, pp. 2662-2672, Aug 2015. DOI: https://doi.org/10.1002/pola.27766
