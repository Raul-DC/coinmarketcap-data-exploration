# 📈 Análisis Automatizado de Criptomonedas con la API de CoinMarketCap

Este proyecto implementa un sistema automatizado de consulta y análisis de datos financieros en tiempo real utilizando la API de CoinMarketCap. Mediante un Jupyter Notebook, se recolectan datos cada minuto durante más de 5 horas para construir un historial confiable de múltiples criptomonedas. Se procesan, transforman y visualizan con técnicas modernas de análisis y visualización de datos.

---

## 🚀 Tecnologías Utilizadas

- 🐍 Python 3
- 📦 Bibliotecas: `pandas`, `requests`, `matplotlib`, `seaborn`, `json`, `os`, `time`
- 📡 CoinMarketCap API
- 📊 Jupyter Notebook

---

## ⚙️ Requisitos

Antes de ejecutar el notebook, asegúrate de tener las siguientes dependencias instaladas:

```bash
requests==2.31.0
python-dotenv==1.0.0
numpy==1.26.0
pandas==2.1.0
seaborn==0.12.2
matplotlib==3.7.2
jupyter==1.0.0
ipykernel==6.25.0
```

---

## 🔐 Configurar API Key de CoinMarketCap

Para proteger tu clave de acceso, el proyecto está configurado para leer la API Key desde una **variable de entorno**.

### Pasos para configurar tu clave:

1. Crea una cuenta gratuita en [CoinMarketCap API](https://coinmarketcap.com/api/).
2. Obtén tu API Key.
3. Guarda la clave en una variable de entorno llamada `CMC_API_KEY`. Por ejemplo:

**En Linux/macOS:**
```bash
export CMC_API_KEY='tu_clave_aquí'
```

**En Windows (CMD):**
```cmd
set CMC_API_KEY=tu_clave_aquí
```

**En Jupyter (temporalmente):**
```python
import os
os.environ['CMC_API_KEY'] = 'tu_clave_aquí'
```

---

## ⚙️ Características Técnicas Clave

- 🔁 **Automatización completa del consumo de datos**: Se realizan 333 solicitudes a intervalos de 60 segundos, acumulando más de 5 horas de observaciones.
- 📥 **Consumo seguro de API**: Validación del estado de respuesta (`status_code`) antes de procesar cada llamada.
- 🧹 **Transformación avanzada con pandas**: Normalización de datos JSON, selección de campos relevantes, renombrado y pivoteo de columnas.
- 📊 **Visualización multivariable**: Comparación de porcentajes de cambio entre criptomonedas, análisis de tendencia de Bitcoin.
- 💾 **Almacenamiento estructurado** (opcional): Los datos pueden guardarse como CSV o Excel para análisis posterior.
- 🛑 **Control de errores y robustez**: Manejador de excepciones para evitar bloqueos por respuestas inválidas o fallos de red.

---

## 📊 Resultados Visuales

### 📈 Evolución del Precio de Bitcoin
Gráfico de líneas que muestra la evolución temporal del precio de BTC en intervalos de 1 minuto.

![image](https://github.com/user-attachments/assets/97abc027-db81-4fa9-8ea7-79c1bd0e6c5d)

---

### 📊 Comparativa de Porcentajes de Cambio
Visualización comparativa entre criptomonedas (BTC, ETH, ADA, etc.) con sus variaciones porcentuales en distintos periodos.

![image](https://github.com/user-attachments/assets/1fbdb77d-e76b-4009-8227-f985c75fea27)

---

### 🧾 Previsualización del Dataset
Vista previa del DataFrame normalizado tras recolectar los datos desde la API.

![image](https://github.com/user-attachments/assets/83806bea-55f8-4527-b4f4-b44a0d42bf22)

---

## 📂 Estructura del Repositorio

```
📁 project-root/
├── 📄 Project-ACAPI.ipynb
├── 📄 README.md
├── ⚙️ .env
├── 📄 requirements.txt
└── 📁 images/
    ├── dataframe-preview.png
    ├── percent-change-graph.png
    └── bitcoin-lineplot.png
```

---

## 📌 Conclusiones

Este proyecto me permitió:

- Dominar el consumo de APIs externas con autenticación.
- Automatizar procesos de recolección de datos a intervalos de tiempo definidos.
- Trabajar con estructuras complejas como respuestas JSON anidadas.
- Visualizar datos financieros de forma clara y efectiva.
- Fortalecer habilidades en transformación de datos con `pandas`.

---

## 👤 Autor

**Raul Diaz** — [LinkedIn](https://www.linkedin.com/in/raul-dc/)

---

## 📬 Contacto

¿Tienes dudas, sugerencias o ideas para extender el proyecto?  
¡Contáctame por [GitHub](https://github.com/) o [LinkedIn](https://www.linkedin.com/in/raul-dc/)!

---
