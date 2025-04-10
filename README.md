# 📈 Análisis de Criptomonedas con la API de CoinMarketCap

Este proyecto utiliza un Jupyter Notebook para obtener, procesar y visualizar datos de criptomonedas en tiempo real mediante la API de CoinMarketCap. Se aplican técnicas de automatización, transformación y visualización con `pandas`, `matplotlib` y `seaborn`.

---

## 🚀 Tecnologías Utilizadas

- 🐍 Python 3
- 📦 Bibliotecas: `pandas`, `requests`, `matplotlib`, `seaborn`, `json`, `os`
- 📡 CoinMarketCap API
- 📊 Jupyter Notebook

---

## ⚙️ Requisitos

Antes de ejecutar el notebook, asegúrate de tener instaladas las dependencias:

```bash
pip install pandas matplotlib seaborn requests
```

---

## 🔐 Configurar API Key de CoinMarketCap

Para proteger tu clave de acceso, el proyecto está configurado para leer la API Key desde una **variable de entorno**.

### Pasos para configurar tu clave:

1. Crea una cuenta gratuita en [CoinMarketCap API](https://coinmarketcap.com/api/).
2. Obtén tu clave (API Key).
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

## 🧠 Descripción del Notebook

### 🔁 Automatización del consumo de datos
Cada minuto se realiza una consulta a la API durante 333 ciclos. Los datos se almacenan y normalizan en un `DataFrame`.

![Vista del DataFrame](images/dataframe-preview.png)

### 📊 Visualización Comparativa
Se grafican los cambios porcentuales por criptomoneda en distintos periodos.

![Gráfico de puntos](images/percent-change-graph.png)

### 📈 Evolución del Precio de Bitcoin
Gráfico de línea con el historial del precio de Bitcoin.

![Gráfico de Bitcoin](images/bitcoin-lineplot.png)

---

## 📌 Conclusiones

Este proyecto me permitió:

- Automatizar llamadas a APIs externas.
- Trabajar con datos en formato JSON.
- Aplicar transformaciones avanzadas con `pandas`.
- Visualizar datos financieros con claridad.

---

## 📂 Estructura del Repositorio

```
📁 project-root/
├── 📄 Project-ACAPI.ipynb
├── 📄 README.md
├── ⚙️ .env
└── 📁 images/
    ├── dataframe-preview.png
    ├── percent-change-graph.png
    └── bitcoin-lineplot.png
```

---

## 👤 Autor

**Raul Diaz** — [LinkedIn](https://www.linkedin.com/in/raul-dc/)

---

## 📬 Contacto

¿Tienes dudas o sugerencias? ¡Contáctame por GitHub o LinkedIn!


---
