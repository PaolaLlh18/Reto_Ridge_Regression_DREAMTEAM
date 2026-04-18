# Reto Ridge Regression: Reconocimiento Facial Sintético

**Equipo:** DREAMTEAM  
**Curso:** Machine Learning (TE3002B)  
**Profesor:** Alberto Muñoz  

**Integrantes:**
Héctor Eduardo Tovar Mendoza - A00840308
Jocelyn Anahid Velarde Barron - A01285780
Paola Llamas Hernández - A01178479
José Luis Dominguez Morales - A01285873
Pablo Armando Mac Beath Milián - A01735082

## Descripción del Proyecto
Este repositorio contiene la implementación de un pipeline de reconocimiento facial basado en el artículo de investigación *An, Liu & Venkatesh (2007)*. El proyecto utiliza **Ridge Regression Multivariada** para clasificar identidades generadas sintéticamente mediante una malla paramétrica de 12 dimensiones.

## Componentes del Sistema
1. **Rasterización:** Conversión de parámetros geométricos a imágenes de $32\times32$ px.
2. **Preprocesamiento:** Estandarización de píxeles, manejo de multicolinealidad y aumento de datos (flips, brillo).
3. **Modelo Ridge Manual:** Implementación de la Ecuación Normal $(X^TX + \alpha I)^{-1}X^Ty$ sin el uso de librerías externas como `sklearn.Ridge`.
4. **Análisis de Hiperparámetros:** Búsqueda del $\alpha$ óptimo mediante MSE en escala logarítmica.

## Resultados
- **Exactitud (Accuracy):** ~11.7%
- **Análisis Técnico:** Se identificó que la representación de los targets mediante *One-Hot Encoding* es el limitante principal frente al uso del *Símplex Regular sugerido teóricamente.

## Cómo ejecutar
1. Clona este repositorio:
   ```bash
   git clone [https://github.com/PaolaLlh18/Reto_Ridge_Regression_DREAMTEAM.git](https://github.com/PaolaLlh18/Reto_Ridge_Regression_DREAMTEAM.git)
