# ⚡ Módulo 01: Real-Time Analytics con Eventstreams

Este módulo demuestra la capacidad de **Microsoft Fabric** para gestionar la ingesta y el procesamiento de datos en streaming con latencia mínima. Se simula un entorno de sensores IoT que envían telemetría en tiempo real.

## 🎯 Escenario de Negocio
Monitoreo de una flota de sensores de temperatura industriales. El objetivo es detectar picos de calor críticos (>80°C) y persistir los datos para análisis histórico sin pasar por procesos Batch tradicionales.

---

## 🛠️ Arquitectura Técnica
1.  **Ingesta (Source):** Script de Python que actúa como "Custom App" enviando eventos JSON.
2.  **Orquestación:** **Fabric Eventstream** que actúa como el "hub" central de los datos.
3.  **Transformación:** Uso del motor de procesamiento en tiempo real de Fabric para filtrar y dar formato a los eventos.
4.  **Destino (Sink):**
    * **KQL Database:** Para consultas ultrarrápidas y dashboards de tiempo real.
    * **Lakehouse (OneLake):** Almacenamiento en formato Delta para integración con el resto del ecosistema.

---

## 📂 Contenido del Módulo
* `/data-generator/main.py`: Script en Python para simular el envío de datos.
* `/notebooks/`: Ejemplos de KQL queries y procesamiento Spark sobre los datos recibidos.
* `architecture-flow.png`: Diagrama visual del flujo de datos en Fabric.

---

## 🚀 Cómo reproducir este ejemplo
1.  **En Microsoft Fabric:** Crea un nuevo *Eventstream* en tu Workspace.
2.  **Configurar Source:** Añade un "Custom App" y copia la cadena de conexión (Connection String).
3.  **Ejecutar Generador:** ```bash
    python data-generator/main.py
    ```
4.  **Verificar:** Abre el "Real-Time Hub" en Fabric para ver los eventos entrando en vivo.

---

## 💡 Conceptos Clave Demostrados
* **Low Latency:** Procesamiento de eventos en milisegundos.
* **No-Code Transformation:** Uso de la interfaz visual de Eventstream para transformar datos.
* **OneLake Integration:** Escritura directa en tablas Delta sin necesidad de pipelines adicionales.
