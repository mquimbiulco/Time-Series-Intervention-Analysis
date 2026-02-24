# 📊 Diseño Causal de Series Temporales

**Autor:** Mateo Quimbiulco | Ing. Matemático  
**Tecnologías:** Python, Modelado Estadístico, Causal Inference.

## 🎯 Resumen General
El objetivo del proyecto es cuantificar el efecto de cierta intervención realizada en los procesos previos al secado de piezas cerámicas sobre la temperatura de un secadero continuo mediante el diseño de Series Temporales Interrumpidas (ITS) para explicar la magnitud del efecto inmediato y la evolución de la intervención de manera sostenida.

## 🧠 Metodología Analítica
En entornos de negocio y procesos estocásticos, los test A/B tradicionales a menudo son imposibles de implementar. Para este caso, se utilizó un diseño cuasi-experimental (ITS) que permite:
1. **Modelar la tendencia pre-intervención** utilizando modelos autorregresivos para capturar la inercia del sistema.
2. **Evaluar el Efecto de la Intervención** modelando el cambio en el nivel y la pendiente de la serie temporal. 
3. **Validación Estadística:** Análisis de la significancia estadística de los resultados para descartar relaciones espurias y atribuir el efecto a la intervención realizada. 

## 💼 Aplicación Transversal 
Aunque este caso de estudio está aplicado a la termodinámica de un secadero continuo para optimización de manufactura, la arquitectura matemática del modelo es directamente aplicable a la toma de decisiones financieras y comerciales:
* **Banca y Riesgos:** Medir el impacto real de un cambio en la tasa de interés sobre la captación de clientes, o evaluar si una nueva política de cobranzas redujo efectivamente la cartera vencida a lo largo del tiempo.
* **Marketing:** Calcular el Retorno de Inversión (ROI) causal de una campaña publicitaria sobre las ventas diarias.
* **Medicina:** Examinar el efecto de cierto medicamento en la salud de las personas que lo usaron.
## 🚀 Resultados Clave
* 
* 

## 📂 Estructura del Repositorio
- `/notebooks`: Cuadernos de jupyter con el Análisis Exploratorio de Datos y el desarrollo paso a paso del modelo ITS, así como el sustento matemático que justifica su aplicación y valida los resultados.
- `/data`: Datasets utilizados (anonimizados por confidencialidad)
---












