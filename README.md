# 📡 Telecom X Latam - Análisis de Deserción de Clientes

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Numpy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

Análisis exploratorio de datos (EDA) sobre **deserción de clientes en Telecom X Latam**. Este proyecto busca comprender los factores que impulsan la deserción y generar insights accionables para:

- 📉 Reducir la tasa de abandono
- 🎯 Priorizar segmentos de alto riesgo
- 🤖 Sentar las bases para modelos predictivos de deserción

---

## 📑 Índice
1. [📖 Descripción](#-descripción)
2. [🎯 Objetivo](#-objetivo)
3. [📊 Principales hallazgos](#-principales-hallazgos)
4. [📁 Estructura del proyecto](#-estructura-del-proyecto)
5. [📊 Ejemplos de visualizaciones](#-ejemplos-de-visualizaciones)
6. [🚀 Cómo ejecutar el proyecto](#-cómo-ejecutar-el-proyecto)
7. [🚀 Tecnologías utilizadas](#-tecnologías-utilizadas)
8. [💡 Recomendaciones estratégicas](#-recomendaciones-estratégicas)
9. [📜 Licencia](#-licencia)
10. [✨ Autor](#-autor)

---

## 📖 Descripción

**Telecom X Latam** enfrenta una tasa de deserción del **26.6%**, lo que representa un impacto significativo en los ingresos de la compañía. Este proyecto aborda el desafío mediante un análisis exploratorio exhaustivo de **7,032 clientes** y **23 variables**, utilizando Python y sus principales bibliotecas de ciencia de datos.

El análisis identifica patrones claros de deserción relacionados con:
- ⏱️ Experiencia temprana del cliente (primeros 6 meses críticos)
- 📝 Tipo de contrato y método de pago
- 🌐 Servicios contratados (especialmente fibra óptica)
- 👥 Perfil demográfico y comportamiento de uso

A partir de estos hallazgos, el equipo de Data Science puede desarrollar **modelos predictivos** y **estrategias de retención** basadas en evidencia.

---

## 🎯 Objetivo

✔️ **Identificar los factores clave** que impulsan la deserción de clientes  
✔️ **Cuantificar el impacto** de cada variable en la tasa de deserción  
✔️ **Segmentar clientes** de alto riesgo para acciones preventivas  
✔️ **Proponer recomendaciones estratégicas** fundamentadas en datos  
✔️ **Establecer bases sólidas** para modelos predictivos de machine learning

---

## 📊 Principales hallazgos

### 🔴 Tasa de deserción global: **26.6%**

### ⏰ Momento crítico
- **53% de la deserción** ocurre en los primeros **6 meses**
- La antigüedad muestra correlación negativa moderada con el abandono
- Superar los 6 meses aumenta drásticamente la probabilidad de permanencia

### 👤 Perfil de alto riesgo
| Factor | Tasa de Deserción |
|--------|-------------------|
| Contrato mensual | 42.7% |
| Fibra óptica | 41.9% |
| Adultos mayores | 41.7% |
| Cheque electrónico | 45.3% |
| Sin soporte técnico | 2.7x mayor |

### 💰 Impacto financiero
- La deserción afecta **desproporcionadamente** a clientes de alto cargo mensual
- Mediana de cargo: **$80** (desertores) vs **$63** (no desertores)
- El abandono temprano de clientes premium representa el **mayor riesgo** para ingresos

### 📌 Insight clave
> La deserción **no es aleatoria**: responde a patrones claros de experiencia temprana, tipo de contrato y composición del servicio.

---

## 📁 Estructura del proyecto

```
challenge-telecom-x/
│
├── TelecomX_LATAM.ipynb       # Notebook principal con el análisis completo
├── data/
│   └── TelecomX_Data.json     # Dataset original (7,267 registros → 7,032 después de ETL)
├── Gráficos/                  # Visualizaciones generadas durante el análisis
│   ├── Distribución_desercion.png
│   ├── Antiguedad_Deserción.png
│   ├── TipoContrato_Deserción.png
│   ├── ServicioInternet_Deserción.png
│   └── MétodoPago_Deserción.png
├── README.md                  # Documentación del proyecto
└── requirements.txt           # Dependencias de Python
```

### 📋 Descripción de archivos principales

- **TelecomX_LATAM.ipynb**: Contiene todo el análisis exploratorio, desde la carga de datos hasta las conclusiones finales
- **data/**: Carpeta con el dataset original en formato JSON (7,267 registros antes de ETL, 7,032 registros limpios)
- **Gráficos/**: Visualizaciones clave generadas durante el análisis
- **requirements.txt**: Lista de librerías necesarias con sus versiones específicas

---

## 📊 Ejemplos de visualizaciones

### 1. Distribución de Deserción
![Churn Distribution](https://github.com/EddersonPR/challenge-telecom-x/blob/main/Gr%C3%A1ficos/Distribuci%C3%B3n_desercion.png)
*Tasa general de deserción: 26.6% de los clientes abandonan el servicio*

### 2. Análisis de Antigüedad vs Deserción
![Tenure Analysis](https://github.com/EddersonPR/challenge-telecom-x/blob/main/Gr%C3%A1ficos/Antiguedad_Deserci%C3%B3n.png)
*El 53% de la deserción ocurre en los primeros 6 meses de servicio*

### 3. Impacto del Tipo de Contrato
![Contract Type](https://github.com/EddersonPR/challenge-telecom-x/blob/main/Gr%C3%A1ficos/TipoContrato_Deserci%C3%B3n.png)
*Contratos mensuales presentan 42.7% de deserción vs 11% en contratos anuales*

### 4. Servicio de Internet y Deserción
![Internet Service](https://github.com/EddersonPR/challenge-telecom-x/blob/main/Gr%C3%A1ficos/ServicioInternet_Deserci%C3%B3n.png)
*Clientes con fibra óptica tienen 41.9% de deserción*

### 5. Método de Pago
![Payment Method](https://github.com/EddersonPR/challenge-telecom-x/blob/main/Gr%C3%A1ficos/M%C3%A9todoPago_Deserci%C3%B3n.png)
*El cheque electrónico es el método con mayor tasa de abandono (45.3%)*

---

## 🚀 Cómo ejecutar el proyecto

### 📍 Opción 1: Google Colab (Recomendado - No requiere instalación)

1. Haz clic en el siguiente enlace:  
   🔗 [📊 Abrir Notebook en Google Colab](https://colab.research.google.com/github/EddersonPR/challenge-telecom-x/blob/main/TelecomX_LATAM.ipynb)

2. El notebook se abrirá directamente en tu navegador

3. Haz clic en **"Ejecutar todo"** en el menú `Runtime > Run all`

4. Todos los gráficos y análisis se generarán automáticamente

**Ventajas:**
- ✅ No necesitas instalar nada en tu computadora
- ✅ Funciona desde cualquier dispositivo con navegador
- ✅ Incluye GPU gratuita si necesitas procesamiento adicional

---

### 💻 Opción 2: Ejecución Local

#### Requisitos previos
- Python 3.8 o superior
- pip (gestor de paquetes de Python)
- Git (opcional, para clonar el repositorio)

#### Pasos de instalación

**1. Clona el repositorio**
```bash
git clone https://github.com/EddersonPR/challenge-telecom-x.git
cd challenge-telecom-x
```

**2. Crea un entorno virtual (recomendado)**
```bash
# En Windows
python -m venv venv
venv\Scripts\activate

# En Mac/Linux
python3 -m venv venv
source venv/bin/activate
```

**3. Instala las dependencias**
```bash
pip install -r requirements.txt
```

**4. Inicia Jupyter Notebook**
```bash
jupyter notebook TelecomX_LATAM.ipynb
```

**5. Ejecuta el análisis**
- El notebook se abrirá en tu navegador predeterminado
- Ejecuta las celdas secuencialmente con `Shift + Enter`
- O ejecuta todo el notebook con `Cell > Run All`

---

### 📦 Dependencias principales

```txt
pandas==2.0.3
numpy==1.24.3
matplotlib==3.7.2
seaborn==0.12.2
jupyter==1.0.0
requests==2.31.0
chardet==5.2.0
scipy==1.11.0
```

**Instalación manual de dependencias:**
```bash
pip install pandas numpy matplotlib seaborn jupyter requests chardet scipy
```

**Nota:** Los módulos `json` y `datetime` vienen incluidos con Python y no requieren instalación adicional.

---

### 🔧 Solución de problemas comunes

**Problema:** `ModuleNotFoundError: No module named 'pandas'`  
**Solución:** Ejecuta `pip install pandas numpy matplotlib seaborn`

**Problema:** Jupyter no se inicia  
**Solución:** Verifica que el entorno virtual esté activado y ejecuta `pip install jupyter`

**Problema:** Error al cargar el dataset  
**Solución:** Verifica que el archivo `data/TelecomX_Data.json` exista en la ruta correcta

**Problema:** Error con `scipy.stats`  
**Solución:** Instala scipy con `pip install scipy==1.11.0`

---

## 🚀 Tecnologías utilizadas

- 🐍 **Python 3.8+** – Lenguaje principal de análisis
- 📊 **Pandas** – Manipulación y análisis de datos estructurados
- 📈 **Matplotlib / Seaborn** – Visualización de datos y gráficos estadísticos
- 🔢 **NumPy** – Operaciones numéricas y estadísticas
- 📓 **Jupyter Notebook** – Desarrollo interactivo del análisis
- ☁️ **Google Colab** – Ejecución en la nube sin instalación local
- 💻 **Visual Studio Code** – Desarrollo y edición de código
- 🌐 **Git / GitHub** – Control de versiones y colaboración
- 📡 **Requests** – Obtención de datos desde APIs
- 🔍 **Chardet** – Detección de codificación de archivos
- 📊 **Scipy** – Análisis estadístico avanzado (correlación point-biserial)

---

## 💡 Recomendaciones estratégicas

### 🚀 Acciones de corto plazo (operativas)

1. **Programa de onboarding intensivo** en los primeros 90 días
   - Llamadas proactivas de bienvenida
   - Tutoriales personalizados de servicios contratados
   - Verificación de satisfacción en días 7, 30 y 90

2. **Seguimiento proactivo** a clientes de fibra óptica
   - Monitoreo de calidad de servicio
   - Soporte técnico prioritario
   - Encuestas de satisfacción trimestrales

3. **Incentivos para migrar** de contrato mensual a anual
   - Descuentos del 15-20% en contratos anuales
   - Meses gratis por adelantado
   - Servicios premium sin costo adicional

4. **Promover métodos de pago automáticos**
   - Descuentos por pago con tarjeta o transferencia
   - Facilitar el cambio desde cheque electrónico
   - Recordatorios automáticos de vencimiento

---

### 🎯 Acciones de retención (mediano plazo)

**Sistema de alertas tempranas para clientes con:**
- ⏱️ Antigüedad < 6 meses
- 💰 Cargo mensual > $70
- 🚫 Sin soporte técnico contratado
- 📝 Contrato próximo a vencer
- 📞 Historial de quejas o reclamos

**Programa de retención personalizado:**
- Ofertas exclusivas 30 días antes del vencimiento contractual
- Upgrades gratuitos de servicios
- Atención por ejecutivo dedicado para clientes de alto valor

---

### 🤖 Data Science - Variables clave para modelo predictivo

**Variables de mayor peso para el modelo de ML:**

1. **Antigüedad del cliente** (tenure) - Correlación: -0.35
2. **Tipo de contrato** (Contract) - Deserción: 42.7% mensual vs 11% anual
3. **Servicio de internet** (InternetService) - Deserción fibra: 41.9%
4. **Cargo mensual** (MonthlyCharges) - Mayor en desertores
5. **Soporte técnico** (TechSupport) - Sin soporte: 2.7x más deserción
6. **Adulto mayor** (SeniorCitizen) - Deserción: 41.7%
7. **Método de pago** (PaymentMethod) - Cheque: 45.3% deserción

**Próximos pasos sugeridos:**
- Implementar modelos de clasificación (Random Forest, XGBoost, Regresión Logística)
- Validar con métricas: Accuracy, Precision, Recall, F1-Score, AUC-ROC
- Desarrollar sistema de scoring de riesgo de deserción (0-100)
- Integrar predicciones con CRM para acciones automatizadas

---

## 🔮 Próximos pasos

- [ ] Desarrollar modelo predictivo de Machine Learning
- [ ] Implementar dashboard interactivo con Power BI
- [ ] Análisis de cohortes por mes de ingreso
- [ ] Estudio de CLV (Customer Lifetime Value)
- [ ] A/B Testing de estrategias de retención

---

## 📜 Licencia

Este proyecto se comparte bajo la licencia **MIT**.  
Puedes usarlo, modificarlo y distribuirlo libremente citando la fuente.

```
MIT License

Copyright (c) 2025 Edderson Pomacanchari Ramos

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## ✨ Autor

**Edderson Pomacanchari Ramos**  
Data Analyst | Python Developer | Business Intelligence

📧 **Contacto:**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/eddersonpr/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EddersonPR)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:edderson.pr@gmail.com)

---

## 🙏 Agradecimientos

Este proyecto fue desarrollado como parte del **Challenge de Análisis de Datos - Telecom X Latam**, con el objetivo de aplicar técnicas de:
- 👨‍💻 **ETL** (Extracción, Transformación y Carga de datos)
- 📊 **Análisis Exploratorio de Datos (EDA)**
- 📈 **Storytelling con datos**
- 💡 **Generación de insights de negocio**
- 🎯 **Resolución de problemas reales empresariales**

Agradecimientos especiales a:
- La comunidad de Data Science por sus recursos y herramientas open source
- Telecom X Latam (caso de estudio) por proporcionar el contexto del desafío
- Alura Latam y Oracle Next Education por la formación en análisis de datos

---

## 📞 ¿Dudas o sugerencias?

Si tienes preguntas sobre el análisis o deseas colaborar:
- 🐛 Reporta issues en [GitHub Issues](https://github.com/EddersonPR/challenge-telecom-x/issues)
- 💬 Abre una discusión en [GitHub Discussions](https://github.com/EddersonPR/challenge-telecom-x/discussions)
- 📧 Contáctame directamente por [LinkedIn](https://www.linkedin.com/in/eddersonpr/) o [Email](mailto:edderson.pr@gmail.com)

---

⭐ **Si este proyecto te resulta útil, considera darle una estrella en GitHub**

[![Star on GitHub](https://img.shields.io/github/stars/EddersonPR/challenge-telecom-x?style=social)](https://github.com/EddersonPR/challenge-telecom-x)
