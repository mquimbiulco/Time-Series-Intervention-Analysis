# ⚙️ Extracción, Transformación y Carga (ETL)

Este documento detalla la naturaleza de los conjuntos de datos utilizados y el pipeline de procesamiento implementado para preparar la información antes del modelado.

## 📖 Diccionario y Descripción de Datos

* **🌡️ Sensores:** El secadero continuo está dividido físicamente en 6 zonas de igual longitud. Cada zona está equipada con un sensor que registra la temperatura y la humedad relativa cada que se detecta un cambio significativo.
* **🔍 Control de Calidad:** Al finalizar el proceso de secado, las piezas son inspeccionadas visual y mecánicamente. Se registra la calidad general del lote y se categorizan los defectos específicos encontrados.

---

## 🛠️ Pipeline de Transformación de Datos

### 1. Datos de Temperatura
* **Extracción:** Consulta directa a la base de datos transaccional en **MySQL**. Filtrado exclusivo de las variables de interés (sensores de temperatura).
* **Resampling y Regularización:** Dado que los sensores registran por cambios significativos, se regularizó la serie temporal a una frecuencia **horaria**. Se calculó el promedio de las observaciones por hora y se imputaron los valores faltantes utilizando interpolación hacia adelante (*forward-fill*).
* **Detección y Tratamiento de Anomalías:** * Se entrenó un modelo no supervisado **Isolation Forest** para identificar el 1% de datos anómalos en las lecturas de los sensores.
  * Para no perder la continuidad espacial y temporal de la serie, los valores atípicos detectados fueron sometidos a un proceso de **winsorización**, mitigando su impacto en la varianza sin eliminar las observaciones.

### 2. Datos de Calidad
* **Extracción:** Consulta a la base de datos histórica en **SQL Server**.
* **Agrupación:** Consolidación de las observaciones a nivel diario, agrupadas por fecha, pieza y tipo de defecto.
* **Feature Engineering:** Creación de la métrica objetivo. Se calculó la **Tasa de Defectos**, generando una nueva variable que representa la proporción exacta de piezas defectuosas sobre el total procesado en el día.
