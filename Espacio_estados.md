# Espacio de Estados: Selección de Asteroides según su Potencial de Recursos

## 1. Descripción del problema
El problema consiste en seleccionar asteroides candidatos para una posible misión de minería espacial, considerando su potencial estimado de recursos y las restricciones de la misión.
Para representar el problema, se utilizará un espacio de estados que permita describir las diferentes alternativas de selección. Cada estado representará una situación dentro del proceso de evaluación y selección de candidatos.
El objetivo será encontrar una selección de asteroides que cumpla las restricciones definidas y obtenga el mejor resultado de acuerdo con un criterio de evaluación establecido.

## 2. Estado inicial
El estado inicial representa el comienzo del proceso, cuando todavía no se ha seleccionado ningún asteroide.
**Estado inicial:** conjunto de candidatos disponibles, con una selección vacía.
Representación:
S₀ = (C, ∅)
Donde:
- C: conjunto de asteroides candidatos disponibles.
- ∅: conjunto vacío de asteroides seleccionados.

## 3. Estados
Cada estado representa una selección parcial o completa de asteroides candidatos.
Un estado se puede representar como:
S = (C, A)
Donde:
- C: conjunto de candidatos disponibles.
- A: conjunto de asteroides seleccionados hasta ese momento.
Durante la exploración, el estado cambia cuando se incorpora un candidato a la selección o se decide continuar sin incorporarlo.

Por ejemplo:
- **Estado inicial:** no se ha seleccionado ningún asteroide.
- **Estado intermedio:** se ha seleccionado uno o más candidatos.
- **Estado final:** se ha obtenido una selección que cumple las restricciones establecidas.

## 4. Operadores
Los operadores son las acciones que permiten pasar de un estado a otro.
Se consideran los siguientes operadores:
- **Seleccionar candidato:** incorporar un asteroide disponible a la selección actual.
- **Descartar candidato:** excluir un asteroide de la selección.
- **Evaluar selección:** calcular el valor de la selección utilizando los criterios definidos, como el potencial estimado de recursos.
- **Verificar restricciones:** comprobar si la selección cumple las condiciones establecidas para la misión.
La aplicación de estos operadores permite explorar distintas alternativas de selección.

## 5. Restricciones
Para limitar las alternativas y evitar selecciones que no cumplan las condiciones del problema, se establecerán las siguientes restricciones:
- **Presupuesto:** el costo estimado de la misión no debe superar el presupuesto disponible.
- **Capacidad de la misión:** la cantidad de asteroides seleccionados debe respetar el límite establecido.
- **Distancia:** los candidatos deben encontrarse dentro de un rango de distancia considerado aceptable para el escenario simulado.
- **Disponibilidad de datos:** cada candidato debe contar con los datos necesarios para su evaluación.
- **Potencial de recursos:** se utilizará la estimación del modelo de regresión como criterio para comparar candidatos, no como garantía de que los recursos existan o puedan extraerse realmente.
Los valores específicos de estas restricciones se definirán durante la implementación del pipeline.

## 6. Estado objetivo
El estado objetivo representa una selección de asteroides que cumple las restricciones y alcanza el mejor valor posible según el criterio de evaluación definido.
Para este proyecto, se priorizará el potencial estimado de recursos sin exceder las restricciones de la misión.
Como se trata de un escenario simulado, el resultado será una selección computacional de candidatos y no una recomendación para una misión espacial real.

## 7. Representación del espacio de estados
El proceso puede representarse mediante el siguiente esquema:

**Estado inicial**  
No hay asteroides seleccionados.

↓  

**Evaluación de candidatos**  
Se analizan las características disponibles y el potencial estimado de recursos.

↓  

**Aplicación de operadores**  
Se seleccionan o descartan candidatos y se generan nuevas alternativas.

↓  

**Verificación de restricciones**  
Se comprueba el cumplimiento de los límites establecidos para la misión.

↓  

**Evaluación de la selección**  
Se compara el potencial estimado de recursos de las alternativas válidas.

↓  

**Estado objetivo**  
Se obtiene una selección que cumple las restricciones y presenta el mejor resultado encontrado según el criterio definido.

## 8. Relación con los pipelines de Machine Learning
El espacio de estados proporciona la representación conceptual del problema para el pipeline de búsqueda. Este pipeline explorará alternativas de selección y evaluará los resultados de acuerdo con las restricciones definidas.
Por otro lado, el pipeline de regresión permitirá estimar una variable cuantitativa relacionada con los recursos potencialmente aprovechables. Esa estimación podrá utilizarse como uno de los criterios para evaluar y comparar candidatos.
Ambos pipelines estarán relacionados dentro del mismo proyecto, pero cumplirán funciones diferentes: el primero explorará alternativas y el segundo realizará predicciones numéricas.
