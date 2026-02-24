# 📊 Diseño Causal de Series Temporales

**Autor:** Mateo Quimbiulco | Ing. Matemático  
**Tecnologías:** Python, Modelado Estadístico, Causal Inference.

## 🎯 Resumen General
Este proyecto aplica técnicas de **Inferencia Causal** y análisis de **Series Temporales Interrumpidas (ITS)** para evaluar el impacto estadísticamente significativo de una intervención en un proceso industrial continuo. El objetivo principal es aislar el efecto real de la intervención con respecto a la estacionalidad previa, demostrando relaciones causales y no simples correlaciones.

## 🧠 Metodología Analítica
En entornos de negocio y procesos estocásticos, los test A/B tradicionales a menudo son imposibles de implementar. Para este caso, se utilizó un diseño cuasi-experimental (ITS) que permite:
1. **Modelar la tendencia pre-intervención** utilizando modelos autorregresivos (ARIMA / SARIMA) para capturar la inercia del sistema.
2. **Evaluar el "Efecto de la Intervención"** modelando el cambio en el nivel y la pendiente de la serie temporal. 
3. **Validación Estadística:** Análisis de la significancia estadística de los resultados para descartar relaciones espurias y atribuir el efecto a la intervención realizada. 

## 💼 Aplicación Transversal 
Aunque este caso de estudio está aplicado a la termodinámica de un secadero continuo para optimización de manufactura, la arquitectura matemática del modelo es directamente aplicable a la toma de decisiones financieras y comerciales:
* **Banca y Riesgos:** Medir el impacto real de un cambio en la tasa de interés sobre la captación de clientes, o evaluar si una nueva política de cobranzas redujo efectivamente la cartera vencida a lo largo del tiempo.
* **Marketing:** Calcular el Retorno de Inversión (ROI) causal de una campaña publicitaria sobre las ventas diarias.
* **Medicina:** Examinar el efecto de cierto medicamento en la salud de las personas que lo usaron.
## 🚀 Resultados Clave
* *[NOTA PARA MATEO: Aquí debes escribir 2 o 3 viñetas con los resultados reales de tu tesis/proyecto. Ejemplo: "Se demostró que la intervención X redujo la variabilidad de la temperatura en un Y%, con un p-value < 0.05, lo que se traduce en una estabilización del proceso."]*
* *[Resultado 2]*

## 📂 Estructura del Repositorio
- `/notebooks`: Cuadernos de jupyter con el Análisis Exploratorio de Datos y el desarrollo paso a paso del modelo ITS, así como el sustento matemático que justifica su aplicación y valida los resultados.
- `/data`: Datasets utilizados (anonimizados por confidencialidad)
---
*Para ver el código y el desarrollo matemático detallado, por favor navega a la carpeta `/notebooks`.*













