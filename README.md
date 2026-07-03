# SP1668-Proyecto-4

El presente repositorio contiene el código ejecutado del Proyecto 4, que se basa en la siguiente arquitectura de redes neuronales:

<img width="798" height="429" alt="imagen" src="https://github.com/user-attachments/assets/050566f9-73ef-4447-bd1e-64284e3cde17" />

Asimismo, se detalla a continuación cada uno de los escenarios generados a partir de los bloques:

<img width="1101" height="389" alt="imagen" src="https://github.com/user-attachments/assets/43474e71-2cd3-4a9c-b5bd-5db8faaa56cb" />

Los resultados de las métricas de rendimiento arrojaron 3 mejores modelos por bloque:

<img width="1055" height="453" alt="imagen" src="https://github.com/user-attachments/assets/bb1b88e6-3c5a-4bff-81a0-d9f2b64719d7" />

Siendo el Modelo 14 con tres capas ocultas, SGD y lr 0.001 el que posee el mejor recall. A la hora de comparar con el resto de modelos de machine learning, se tiene que:

<img width="1071" height="319" alt="imagen" src="https://github.com/user-attachments/assets/2629909d-7617-4d5e-8f89-83b49686e1ed" />

Como puede notarse, ciertos modelos como el XGBoost y Random Forest poseen sobreajuste, por lo que se descartan. Del resto de modelos, con base en su Recall, se elige como mejor modelo la *Red Neuronal Profunda Optimizada* (recall = 0.8786), seguido de la *Regresión Logística con Regularización* (recall = 0.8536).

Figura A. Gráfico SHAP para la Regresión Logística.

<img width="770" height="956" alt="imagen" src="https://github.com/user-attachments/assets/1a30d0d6-8e5c-433b-b16e-d86602ac769c" />

Figura B. Gráfico SHAP para la Red Neuronal

<img width="769" height="940" alt="imagen" src="https://github.com/user-attachments/assets/2e1bd436-31de-413e-9dfc-87f2e410a696" />

De los gráficos anteriores es posible identificar que para ambos modelos, las primeras cinco variables que más influyen en la predicción de la probabilidad de enfermedad coinciden, con lo que, tanto desde un punto de vista de interpretabilidad, como de rendimiento del modelo, lo más relevante para el negocio es elegir el modelo seleccionado de redes neuronales. 

De este modo, el tener historial familiar de diabétes es la variable que más influye en la probabilidad de tener diagnóstico positivo de diabetes, seguido de un aumento de la edad, pocos minutos de actividad física semanal, alto nivel de ritmo cardíaco y ser hombre.
