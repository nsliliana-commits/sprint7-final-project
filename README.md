# 📊 Análisis ConnectaTel - Sprint 7

Este proyecto corresponde al **Sprint 7 del programa de análisis de datos**, donde se realiza la **limpieza, diagnóstico y segmentación** del dataset de clientes de ConnectaTel.  
El objetivo principal es **identificar problemas de calidad de datos**, analizar **patrones de uso** y proponer **recomendaciones de negocio** basadas en los segmentos detectados.

# Proyecto de Limpieza y Segmentación de Datos - ConnectaTel

## 📌 Descripción
Este proyecto tiene como objetivo **diagnosticar, limpiar y analizar** un dataset de clientes de ConnectaTel, identificando problemas de calidad de datos y generando segmentaciones útiles para el negocio.

## ⚠️ Problemas detectados en los datos
- **Sentinels en `age` (-999 y edades fuera de rango):** detectados y reemplazados por valores nulos.
- **Fechas imposibles en `reg_date` (año 2026):** representaban 1.00% de las filas.
- **Nulos en `date` de `usage`:** representaban 0.125% de las filas.

## 🔍 Segmentos por Edad
- **Jóvenes (<30 años):** 19.00% → intensivos en mensajes.
- **Adultos (30–59 años):** 50.45% → uso balanceado.
- **Adultos mayores (≥60 años):** 30.55% → llamadas largas.

## 📊 Segmentos por Nivel de Uso
- **Bajo uso:** 19% (778 clientes).
- **Uso medio:** 72% (2943 clientes).
- **Alto uso:** 7% (279 clientes).

## 📈 Outliers
- **Mensajes y minutos de llamada:** winsorizados para evitar distorsión.
- **Número de llamadas:** mantenido, ya que refleja heavy users reales.

## ⭐ Segmentos más valiosos
- **Adultos (50.45%)**: núcleo estable y mayoritario.
- **Jóvenes (19%)**: menor tamaño pero alta intensidad digital.

## 💡 Recomendaciones
- Optimizar planes básicos para clientes de bajo uso.
- Reforzar planes Premium para heavy users.
- Crear planes segmentados por edad:
  - Jóvenes → paquetes de datos y mensajes.
  - Adultos → planes balanceados.
  - Adultos mayores → minutos preferenciales.
- Monitorear outliers para diferenciar entre errores y clientes especiales.

## 🛠️ Tecnologías utilizadas
- Python 3
- Pandas
- Jupyter Notebook

## 🚀 Cómo ejecutar
1. Clonar este repositorio.
2. Instalar dependencias: `pip install -r requirements.txt`.
3. Abrir el notebook `connectatel_analysis.ipynb`.
4. Ejecutar las celdas en orden para reproducir el análisis.

## 📂 Estructura del repositorio
- `data/` → dataset original y limpio.
- `notebooks/` → notebook principal con el análisis.
- `README.md` → documentación del proyecto.
## 👩‍💻 Autoría
Proyecto realizado por **Liliana**  
Sprint 7 - Data Analysis

