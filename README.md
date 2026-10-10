# Pipeline de Machine Learning para la Selección de Asteroides según su Potencial de Recursos

# 1. Contexto del problema
La minería de asteroides es una propuesta tecnológica orientada a la exploración y posible extracción de recursos presentes en cuerpos menores del sistema solar. Entre los materiales de interés se encuentran metales del grupo del platino, níquel, cobalto y otros elementos que podrían tener aplicaciones en la industria tecnológica y espacial.
Sin embargo, la selección de asteroides para futuras misiones de exploración y extracción presenta dificultades relacionadas con la incertidumbre sobre su composición, la cantidad de recursos aprovechables, la distancia, los costos de las misiones y las limitaciones tecnológicas.
En este contexto, la Inteligencia Artificial y los métodos de búsqueda computacional pueden servir como herramientas de apoyo para analizar alternativas y priorizar candidatos bajo criterios definitivos.

# 2. Descripción del problema
El problema consiste en seleccionar y priorizar candidatos para la minería espacial a partir de sus características y de una estimación de sus recursos portencialmente aprovechables.
Se busca desarrollar un sistema que utilice un modelo de regresión para estimar una variable cuantitativa relacionada con los recursos y un algoritmo de búsqueda para explorar alternativas, aplicar restricciones y obtener una selección de candidatos según un criterio de optimización.
La pregunta principal del proyecto es: ¿Cómo seleccionar y priorizar asteroides candidatos para la minería espacial mediante un modelo predictivo y un algoritmo de búsqueda, considerando el potencial estimado de recursos y las restricciones de una misión?

# 3. Objetivos
## 3.1 Objetivo General
Desarrollar un sistema inteligente que permita seleccionar y priorizar asteroides candidatos para la minería espacial mediante técnicas de búsqueda y un modelo de regresión aplicado a datos sintéticos o de referencia.
## 3.2 Objetivos Específicos
- Representar el problema mediante un espacio de estados que incluya estados, operadores y restricciones.
- Implementar un algoritmo de búsqueda que explore alternativas de selección de asteroides.
- Entrenar un modelo de regresión para estimar la cantidad de recursos potencialmente aprovechables a partir de características de los candidatos.
- Evaluar las predicciones mediante métricas apropiadas y representarlas gráficamente.
- Integrar las estimaciones del modelo predictivo en el proceso de selección y priorización de candidatos.

# 4. Justificación del uso de Inteligencia Artificial y Machine Learning
La selección de asteroides involucra múltiples variables y restricciones que pueden dificultar la comparación manual de candidatos. Un sistema computacional permite organizar la información, evaluar diferentes alternativas y aplicar criterios de selección de forma sistemática.
El aprendizaje automático se utilizará para construir un modelo de regresión capaz de estimar una variable numérica de interés a partir de los datos disponibles. Por su parte, un algoritmo de búsqueda permitirá explorar alternativas y seleccionar candidatos que cumplan las restricciones establecidas.
La combinación de ambos componentes permitirá desarrollar un prototipo que integre predicción y búsqueda para apoyar la toma de decisiones en un escenario simulado de minería de asteroides.

# 5. Alcance del proyecto
El proyecto se desarrollará mediante Python y Google Colab, con integración del código y la documentación en Github.
Se utilizarán datos sintéticos o datos de referencia adecuados para representar las características de asteroides candidatos. El sistema incluirá un pipeline de búsqueda y un pipeline de regresión, junto con resultados y visualizaciones que permitan analizar su funcionamiento.
El prototipo estará orientado a la comparación y priorización de candidatos bajo criterios definidos. No realizará operaciones espaciales reales ni garantizará la viabilidad económica o técnica de una misión de minería.

# 6. Limitaciones
Los resultados dependerán de las variables, los supuestos y la calidad de los datos utilizados. Si se emplean datos sintéticos, las estimaciones representarán el comportamiento del escenario simulado y no constituirán evidencia de la composición mineral real de un asteroide.
Asimismo, la selección obtenida estará condicionada por las restricciones y los criterios definidos para el problema. Por ello, los resultados deberán interpretarse como apoyo experimental a la toma de decisiones y no como recomendaciones operativas para misiones reales.
