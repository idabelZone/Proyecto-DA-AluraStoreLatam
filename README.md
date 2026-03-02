# 🛍️ Análisis de Ventas - Alura Store LATAM

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lSghUdvuN09wlgbAberNI6BlQEJhnsYx)

## 📘 Propósito y Descripción del Proyecto

Este proyecto forma parte del reto de **Oracle Next Education (ONE) - Alura LATAM**, donde el **propósito principal** es aplicar la **narración de historias con datos (Data Storytelling)** para analizar el rendimiento de las sucursales de la empresa *Alura Store* y determinar estratégicamente cuál genera menos ingresos y por qué.

El análisis integral se desarrolló en **Google Colab**, implementando técnicas fundamentales de Análisis Exploratorio de Datos (EDA) y visualización en Python para respaldar y guiar la toma de decisiones del cliente principal, el **Sr. Juan**.

---

## 📂 Estructura del Proyecto y Organización de Archivos

El repositorio está organizado de la siguiente manera para facilitar su lectura y reproducción:

* `/` (Raíz del repositorio)
  * `README.md`: Documentación principal del proyecto (este archivo).
  * `Proyecto_DA_AluraStoreLatam.ipynb`: Archivo principal (Notebook de Jupyter/Colab) que contiene todo el código Python, limpieza de datos, análisis matemático y generación de gráficos.
* `/assets/`: Carpeta que contiene las imágenes de los gráficos generados para este reporte.

---

## 🎯 Objetivo del Análisis

El Sr. Juan necesita identificar qué tienda debe ser vendida o liquidada para financiar nuevos proyectos. Para ello, se evaluaron los siguientes factores clave:
1. **Facturación total:** Ingresos generados por cada tienda.
2. **Categorías más populares:** Distribución del éxito de ventas por tipo de producto.
3. **Satisfacción del cliente:** Promedio de calificación (estrellas) otorgado por los usuarios.
4. **Rotación de inventario:** Identificación de los productos más y menos vendidos.
5. **Eficiencia logística:** Costo promedio de envío asociado a cada sucursal.

---

## 📊 Ejemplos de Gráficos e Insights Obtenidos

Durante el análisis exploratorio, se generaron diversas visualizaciones para sustentar los hallazgos. A continuación, se presentan los resultados clave que fundamentan la recomendación final:

### 1. Comparativa de Facturación Total
![Gráfico de Facturación] <img width="1190" height="690" alt="image" src="https://github.com/user-attachments/assets/96e425f0-621a-4253-a2f6-971732fee1b6" />
> **Insight Financiero:** Se evidencia claramente que la **Tienda 4**
** presenta el menor ingreso total ($1,038,375,700.00), quedando significativamente rezagada frente a la sucursal líder (Tienda 1, con $1,150,880,400.00). Esta diferencia de más de 112 millones es el factor crítico para la toma de decisión.

### 2. Correlación de Precio vs. Satisfacción
<img width="1487" height="955" alt="Gráfico de Correlación" src="https://github.com/user-attachments/assets/e3333da4-f367-40af-8c89-951117748688" />

> **Insight Estratégico:** Al analizar si el costo de los productos afecta las reseñas de los clientes, se descubrió que este factor solo influye en la mitad de las sucursales. Específicamente, en las **Tiendas 3 y 4** existe una correlación muy negativa. Esto significa que en estas tiendas, a mayor precio del producto, la satisfacción del cliente tiende a disminuir, lo cual representa un foco de riesgo comercial que justifica aún más la decisión de vender la Tienda 4.

### 3. Satisfacción Promedio del Cliente
![Gráfico de Satisfacción]<img width="989" height="590" alt="image" src="https://github.com/user-attachments/assets/3b08d8b4-e979-4971-87d0-38d186a0a937" />

> **Insight de Calidad:** A pesar de sus bajos ingresos, la **Tienda 4** mantiene una satisfacción de cliente muy sólida (4.00/5.00), muy cercana a la líder (Tienda 3 con 4.05). Esto indica que el problema de la tienda no es el mal servicio, sino probablemente factores logísticos o de ubicación.

### 4. Costos Operativos y Alcance Geográfico
<img width="868" height="549" alt="Gráfico de Costos de Envío" src="https://github.com/user-attachments/assets/a3556f96-13db-4152-91a2-b9e9aee73b97" />

> **Insight Logístico:** El análisis de distribución confirmó que la mayor concentración de ventas ocurre en el eje central del país (Bogotá, Medellín y Cali). Al evaluar los gastos operativos, observamos que la **Tienda 1** asume los costos de envío más altos ($26,018.61 en promedio). Por otro lado, aunque la **Tienda 4** parece ser la más "eficiente" por tener el costo de envío más bajo ($23,459.46), este aparente ahorro realmente refleja su menor penetración en el mercado masivo, y no logra compensar su déficit en la facturación total.

---

## 💡 Conclusión y Recomendación

> **"Sugerimos proceder con la venta y liquidación de la Tienda 4."**

Basado en la evidencia de los datos analizados, la **Tienda 4** es la candidata definitiva para financiar los nuevos proyectos del Sr. Juan. A pesar de tener gastos de envío eficientes y clientes satisfechos, es el eslabón más débil financieramente. 

Como estrategia paralela para el resto del negocio, se recomienda:
1. Ajustar los modelos de cobro de envío en la Tienda 1 (la más costosa operativamente).
2. Potenciar el inventario de los productos individuales más exitosos (como el libro *"Iniciando en programación"*) mediante marketing cruzado.
3. Reducir el stock de productos de baja rotación (ej. *Juegos de mesa*) en las tiendas 1, 2 y 3 para maximizar la liquidez general.

---

## 🚀 Instrucciones para Ejecutar el Notebook

Para reproducir este análisis en tu propio entorno, sigue estos pasos:

1. Da clic en el botón **"Open in Colab"** al inicio de este documento, o descarga el archivo `.ipynb` de este repositorio.
2. Abre [Google Colab](https://colab.research.google.com/) y sube el archivo `.ipynb` si lo descargaste manualmente.
3. El código está configurado para leer los datos directamente desde los enlaces RAW proporcionados por Alura LATAM.
4. Ve a la pestaña **Entorno de ejecución** en el menú superior y selecciona **"Ejecutar todo"** (o presiona `Ctrl + F9`).
5. Observa cómo se procesan los datos y se generan los gráficos paso a paso en tiempo real.

---

## 🧠 Tecnologías Utilizadas

| Herramienta | Uso Principal |
| :--- | :--- |
| 🐍 **Python** | Lenguaje de programación base |
| 📊 **Pandas** | Limpieza, estructuración y análisis de datos |
| 🎨 **Matplotlib / Seaborn** | Creación de gráficos y visualización de datos |
| ☁️ **Google Colab** | Entorno de ejecución de Notebooks |
| 💾 **GitHub** | Control de versiones y publicación del portafolio |

---

## 👩‍💻 Autora

**Idabel Coparropa**

Proyecto realizado con éxito para el programa **Oracle Next Education (ONE) - Alura LATAM**.

### Autorización
Se permite el uso, estudio y reproducción de este proyecto para fines académicos y de aprendizaje, siempre y cuando se otorguen los créditos correspondientes a la autora.

* 📧 **Contacto:** idabelcoparropa382@gmail.com
* 🌐 **Repositorio:** [Perfil de GitHub](https://github.com/repos)
