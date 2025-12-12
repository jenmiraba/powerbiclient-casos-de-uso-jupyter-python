# Power BI + Jupyter Notebooks: Validación, Auditoría Visual y Análisis Avanzado en un Solo Flujo

## 📋 Descripción General

Este repositorio contiene un flujo de trabajo completo para integrar **Power BI** con **Jupyter Notebooks** utilizando la librería `powerbiclient`. La solución permite realizar validación de datos, auditoría visual automática, análisis avanzados y prototipado rápido de reportes, todo sin salir del entorno de Python.

## 🎯 Problema que Resuelve

Como analistas y desarrolladores de Power BI, nos enfrentamos constantemente a estos desafíos:

1. **"Estos números no me cierran"** → Validar datos entre visuales y fuentes originales
2. **"Esta información no la tengo"** → Identificar áreas de atención del usuario y optimizar diseño
3. **"Necesito análisis más avanzados"** → Realizar clustering, forecasting, optimización
4. **"Lo necesito para ayer"** → Crear prototipos rápidos sin modelado complejo

Esta integración permite resolver estos 4 escenarios en un solo flujo de trabajo, sin navegar entre varias páginas.

## 🚀 Casos de Uso Empresariales

### Caso 1: Validación de Datos
**Escenario**: El cliente dice "Las ventas por canal no coinciden con los números que tengo"

**Solución**:
- Extraer datos directamente del visual de Power BI
- Compararlos con la base de datos original (MySQL, SQL Server, etc.)
- Identificar discrepancias en segundos

### Caso 2: Auditoría Visual Automática
**Escenario**: "Los usuarios no encuentran la información más importante en el dashboard"

**Solución**:
- Generar heatmaps de atención visual predicha
- Analizar composición del dashboard (tipos de visuales, uso del espacio)
- Evaluar mejores prácticas de UX/UI con puntuación automática
- Recibir recomendaciones concretas de mejora

### Caso 3: Análisis Avanzado (Forecasting)
**Escenario**: "Necesito un forecast de los próximos 90 días de ventas"

**Solución**:
- Extraer datos limpios directamente del modelo de Power BI
- Aplicar modelos de Machine Learning (Prophet, ARIMA, etc.)
- Generar predicciones con intervalos de confianza
- Crear nuevo reporte con los resultados

### Caso 4: Prototipado Rápido
**Escenario**: "Necesito un reporte de ventas por región y producto para una reunión en 30 minutos"

**Solución**:
- Cargar datos desde un DataFrame de pandas
- Crear reporte interactivo automáticamente
- Editarlo y guardarlo en Power BI Service

## 🛠️ Instalación y Configuración

### Requisitos de powerbiclient
```bash
pip install powerbiclient
```

### Extensiones de Jupyter
```bash
# Para JupyterLab
jupyter labextension install @jupyter-widgets/jupyterlab-manager

# Para Jupyter Notebook 5.2 o anterior
jupyter nbextension enable --py --sys-prefix powerbiclient
```

### Configuración de Credenciales

Para proteger tus credenciales, crea un archivo `.env` en la raíz del proyecto:
```env
user=tu-usuario
password=tu-password
host=localhost
database=tu-database
```

**Importante**: Añade `.env` y `config.txt` a tu archivo `.gitignore` para no subir credenciales a GitHub.

## Recursos Adicionales

- [Documentación oficial powerbiclient](https://github.com/microsoft/powerbi-jupyter)

## 👤 Autor

**@jenmiraba**
