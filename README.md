# Análisis de Datos de viajes de Uber con Python

## Índice
1. [Descripción](#descripción)
2. [Tecnologías utilizadas](#tecnologías-utilizadas)
3. [Análisis realizados](#análisis-realizados)
4. [Resultados y hallazgos clave](#resultados-y-hallazgos-clave)
5. [Cómo ejecutar el proyecto](#cómo-ejecutar-el-proyecto)
6. [Aprendizajes](#aprendizajes)
7. [Autora](#autora)

---

## Descripción
Este proyecto realiza un análisis exploratorio sobre un conjunto de datos de viajes de Uber. El objetivo principal es comprender el comportamiento de las reservas, identificar los tipos de viaje más comunes, los métodos de pago preferidos, las calificaciones de usuarios y conductores, y la relación entre el valor, la distancia y las características del viaje.

---

## Tecnologías utilizadas
- **Lenguaje:** Python  
- **Entorno de desarrollo:** Visual Studio Code, Jupyter Notebook  
- **Librerías:** Pandas, Matplotlib, Seaborn  

---

## Análisis realizados
El notebook sigue un proceso estructurado para analizar los datos:

- **Limpieza y preprocesamiento de datos:**
    - Conversión de tipos de datos (fechas y horas).
    - Eliminación de caracteres innecesarios en IDs.
    - Detección y eliminación de registros duplicados.
    - Selección de columnas relevantes para el análisis y manejo de valores nulos.

- **Análisis de la distribución de variables numéricas:**
    - Estudio de `Booking Value`, `Ride Distance`, `Driver Ratings` y `Customer Rating` mediante histogramas y boxplots para identificar la distribución y la presencia de outliers.

- **Análisis de variables categóricas:**
    - Frecuencia de los diferentes `Booking Status` para entender la tasa de viajes completados vs. cancelados.
    - Distribución de los `Payment Method` más utilizados.

- **Análisis de relaciones:**
    - Relación entre el `Vehicle Type` y el `Booking Value` para segmentar los precios.
    - Identificación de las **10 principales zonas de origen y destino** para detectar focos de alta demanda.

---

## Resultados y hallazgos clave

- **El viaje típico:** La mayoría de los viajes son de **corta distancia** (menos de 20 km) y **bajo costo** (la mayoría por debajo de 500), lo que sugiere un uso predominante para trayectos urbanos y rutinarios.

- **Calificaciones altas:** Tanto conductores como clientes reciben mayormente **calificaciones altas** (entre 4.0 y 5.0), indicando un nivel general de satisfacción alto en el servicio.

- **Estado de las reservas:** Aunque la mayoría de los viajes se completan, existe un número significativo de reservas que son **canceladas por el conductor** o donde **no se encuentra conductor**.

- **Métodos de pago:** **UPI** y el **efectivo (Cash)** son los métodos de pago dominantes, mostrando una mezcla entre pagos digitales y tradicionales.

- **Segmentación por vehículo:** Los vehículos de gama alta como `Premier Sedan` y `Uber XL` muestran, como es de esperar, un valor de viaje mediano y un rango de precios más elevados que las opciones económicas como `Bike` o `Auto`.

- **Zonas de alta demanda:** Se identificaron focos claros de demanda en ubicaciones como **Khandsa**, **Barakhamba Road** y **Ashram**, que aparecen consistentemente en los top 10 de origen o destino.

---

## Cómo ejecutar el proyecto

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/DamiPinto/analisis-uber.git
   cd analisis-uber
   ```

2. **Crear un entorno virtual (recomendado):**
   ```bash
   python -m venv venv
   source venv/bin/activate   # En Linux/Mac
   venv\Scripts\activate      # En Windows
   ```

3. **Instalar dependencias:**
   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

4. **Ejecutar el notebook:**
   Abre el archivo `analisis_uber.ipynb` en Jupyter Notebook, Jupyter Lab o Visual Studio Code y ejecuta las celdas.

---

## Aprendizajes
Este proyecto me permitió afianzar conocimientos en:
- **Limpieza y preparación de datos:** Aplicación de técnicas para manejar valores nulos, duplicados y outliers, un paso fundamental en cualquier proyecto de datos real.
- **Análisis exploratorio (EDA):** Uso de visualizaciones con Matplotlib y Seaborn para descubrir patrones, distribuciones y relaciones entre variables.
- **Obtención de conclusiones de negocio:** Traducción de los hallazgos técnicos en insights aplicables, como la confiabilidad del servicio, las preferencias de pago y los focos de demanda.
- **Comunicación de resultados:** Estructuración de un notebook de manera clara y documentada para contar una historia coherente a partir de los datos.

---

## Autora
Proyecto desarrollado por **Damiana Sofia Pinto**.  

- **LinkedIn:** [linkedin.com/in/damiana-pinto](https://linkedin.com/in/damiana-pinto)  
