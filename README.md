# 🚀 Microsoft Fabric: End-to-End Data Solutions

Este repositorio es un ecosistema de proyectos prácticos diseñados para demostrar el potencial de **Microsoft Fabric** como plataforma unificada de datos (SaaS). Aquí encontrarás desde ingesta en tiempo real hasta orquestación avanzada y analítica distribuida.

---

## 🏗️ Arquitectura del Workspace
El repositorio está organizado siguiendo el flujo lógico del dato dentro de un entorno de producción en Fabric:

| Módulo | Componentes de Fabric | Descripción |
| :--- | :--- | :--- |
| **[01-Real-Time Analytics](./01-realtime-analytics-eventstream)** | Eventstreams, KQL, Data Activator | Ingesta de telemetría IoT con baja latencia y alertas automáticas. |
| **[02-Data Engineering](./02-data-engineering-lakehouse)** | Lakehouse, Spark Notebooks, V-Order | Procesamiento ETL a escala utilizando PySpark y optimización Delta. |
| **[03-Data Integration](./03-data-factory-pipelines)** | Data Factory, Copy Activity | Orquestación de pipelines híbridos (On-premise & Cloud). |
| **[04-Data Warehousing](./04-synapse-dw)** | Synapse DW, T-SQL, Schemas | Modelado de datos relacional y análisis mediante SQL Endpoint. |

---

## ⚡ Proyecto Destacado: Eventstream & Real-Time Intelligence
En el módulo `01-Real-Time Analytics`, implemento una solución de monitoreo de eventos en vivo:
* **Ingesta:** Captura de JSONs mediante un Custom App.
* **Procesamiento:** Transformación "en vuelo" (streaming) para filtrar anomalías.
* **Persistencia:** Integración nativa con **OneLake** y visualización inmediata en **KQL Database**.

---

## 🛠️ Tecnologías Clave
* **Lenguajes:** Python (PySpark), SQL (T-SQL/KQL).
* **Almacenamiento:** Delta Lake, OneLake, Parquet.
* **Visualización:** Power BI (Modo Direct Lake).

---

## 📈 ¿Por qué Microsoft Fabric?
El objetivo de este repositorio es explorar la **eliminación de silos de datos**. Al utilizar **OneLake**, todas las herramientas (Spark, SQL, Power BI) acceden a la misma copia de los datos, reduciendo costes de almacenamiento y tiempos de latencia (Copy-less integration).

---

## 👤 Contacto
¿Te interesa saber más sobre alguna implementación específica
