# **Proyecto: ETL – Enfermedades del Corazón (UCI)**

Este proyecto fue desarrollado como práctica para aplicar los conceptos básicos de ETL (Extract, Transform, Load) trabajados en clase. El objetivo fue tomar el dataset de Heart Disease del repositorio UCI, limpiarlo, transformarlo y hacer un análisis rápido para entender mejor la información. Todo se realizó en Python, manteniendo el código claro y manejable.

---

## **Descripción**

Este notebook permite:

- Cargar el dataset de enfermedades del corazón usando la librería oficial `ucimlrepo`.
- Realizar una limpieza básica para dejar los datos en un formato entendible.
- Crear nuevas columnas que ayudan a interpretar la información.
- Generar tablas y gráficos para identificar patrones o diferencias entre grupos de pacientes.
- Incluir un ejercicio adicional (bonificación) con lógica condicional escrita de forma natural.

---

## **Principales pasos del proyecto**

### **1. Extracción de datos**
Se usó la librería `ucimlrepo` para traer el dataset directamente desde UCI, asegurando que los metadatos y columnas llegaran completos y sin errores.

---

### **2. Limpieza**
- Revisión de valores nulos e inconsistentes.  
- Los datos extraños se marcaron como **"desconocido"** para hacer la lectura más natural.  
- Ajuste de tipos de datos para evitar problemas en pasos posteriores.

---

### **3. Transformación**
Se agregaron dos columnas útiles para el análisis:

- **`edad_grupo`**: rangos de edad (30–39, 40–49, 50–59, etc.).  
- **`hipertension_proxy`**: indicador simple basado en presión en reposo mayor a 140.

Estas transformaciones facilitan la lectura y permiten análisis más claros.

---

### **4. Análisis**
Se generaron varias visualizaciones para entender mejor los datos:

- Histograma de edades.  
- Dispersión colesterol vs enfermedad.  
- Porcentaje de enfermedad según el sexo.  
- Gráfico circular con la distribución real del target.

---

### **5. Ejercicio de bonificación**
Incluye un pequeño sistema con condicionales (vidas, energía, arma, nivel), revisado para corregir casos ilógicos y escrito con un tono natural.

---

## **Tecnologías usadas**

- Python 3  
- Pandas  
- Matplotlib  
- NumPy  
- ucimlrepo  
- Google Colab

---

## **Cómo ejecutar el proyecto**

1. Abrir el notebook en Google Colab o un entorno compatible con `.ipynb`.  
2. Ejecutar las celdas en orden.  
3. Instalar dependencias si es necesario:

```bash
pip install ucimlrepo pandas matplotlib numpy
```

## **Autor**

**Alejandro García**  
Proyecto realizado con fines académicos para practicar un proceso ETL completo en Python.  
README redactado con apoyo de IA para organizarlo mejor.
