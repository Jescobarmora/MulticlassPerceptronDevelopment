# Multiclass Perceptron Development - Ejercicios 1 a 6

Este repositorio contiene la implementación progresiva de un **Perceptrón Multiclase** para resolver problemas de clasificación, siguiendo los enunciados de los ejercicios 1 a 6. Cada ejercicio añade una capa de complejidad y refinamiento al modelo, comenzando con la generación de datos y culminando con la visualización de la frontera de decisión.

## Estructura del Proyecto

El proyecto está organizado en varios scripts que abarcan los puntos del 1 al 6 de la progresión del perceptrón multiclase:

### Ejercicios:

### **1. Generación de Datos**
- **Descripción**: Uso de la función `make_blobs` para generar datos de prueba con tres clases y dos características (variables).
- **Funcionalidad**: Permite la visualización de los datos generados para observar la distribución de las clases.
  
### **2. Implementación del Perceptrón Multiclase**
- **Descripción**: Implementación de la clase `PerceptronMulticlass` que inicializa los pesos y sesgos a ceros. Incluye la definición de las variables de aprendizaje (`learning_rate` y `n_iters`).
- **Funcionalidad**: Inicializa la matriz de pesos y el vector de sesgos y establece las bases del modelo perceptrón.

### **3. Función de Activación (Escalón)**
- **Descripción**: Se añade la función de activación (`step_function`), que clasifica los datos en función de si el valor de salida es mayor o igual a 0.
- **Funcionalidad**: Esta función transforma las salidas lineales en 1 o 0 y se utiliza para hacer predicciones en el perceptrón.

### **4. Entrenamiento del Perceptrón**
- **Descripción**: El perceptrón multiclase se entrena utilizando el enfoque "One vs Rest", comparando una clase con todas las demás. El modelo se actualiza cuando la predicción no coincide con la clase verdadera.
- **Funcionalidad**: Implementación de la función `fit` para entrenar el modelo iterando sobre los datos de entrada y ajustando los pesos y sesgos cuando la predicción no es correcta.

### **5. Predicción con el Perceptrón**
- **Descripción**: Implementación de la función `predict` que, dado un nuevo conjunto de datos, predice la clase más probable para cada ejemplo. La clase con el valor máximo de salida lineal es seleccionada.
- **Funcionalidad**: Calcula las predicciones sobre un conjunto de datos de entrada y selecciona la clase con la mayor salida lineal.

### **6. Visualización de la Frontera de Decisión**
- **Descripción**: Visualización gráfica de las regiones de decisión del perceptrón entrenado. Se crea una cuadrícula de puntos y se predice la clase para cada punto de la cuadrícula, generando un contorno que separa las regiones clasificadas por cada clase.
- **Funcionalidad**: Permite visualizar la frontera de decisión generada por el perceptrón para ver cómo divide el espacio de características entre las clases.
