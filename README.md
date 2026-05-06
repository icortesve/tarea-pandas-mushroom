## Contenido
- `Analisis con Panda y Kaggle.ipynb`: Notebook con el flujo de datos.
- `mushrooms.csv`: Dataset original.

## Pasos realizados
1. Limpieza de datos
- Buscar duplicados
- Contar faltantes
- Verificar si hay "Falsos Nulos" ("NaN", "null" o "None")
- Contar valores '?' (Falsos nulos del dataset original)
- Encontrar valores '?' (Falsos nulos del dataset original)
- Eliminar columna ['stalk-root'] (Es la columna donde están los falsos nulos)
- Se vuelve  revisar si es que se encuentran duplicados
2. Se crea proyecto:" GUÍA DE SEGURIDAD PARA LA RECOLECCIÓN DE HONGOS (MUSHROOM DATASET)"
- El objetivo es: Identificar patrones físicos y firmas biológicas consistentes que permitan diferenciar con certeza un hongo comestible de uno venenoso, reduciendo el riesgo de intoxicación.
- Para ello, se trabaja con la clase (venenoso o comestible), el olor, y el color de la esporada de cada observación fúngica (fila del dataset)
3. Se crean diccionarios para traducir los 'códigos' del dataset al español, para las columnas objetivos
- Se traduce y reemplazan los valores en español en las columnas objetivo
4. Se realiza un análisis base del DF
- Se cuantifica cuántos y qué porcentaje de los hongos son comestibles, y cuántos son venenosos.

Desarrollo:

Hipótesis 1 (H1): "El olor es el mecanismo biológico de advertencia más fuerte"
1.1: Contar hongos comestibles y venenosos por cada olor
- Encontrar tipos diferentes de olor
- Contar hongos por cada tipo de olor
1.2: Ver si existen aromas exclusivos de hongos venenosos o comestibles
- Agrupar hongos por olor y clase (comestible / venenoso)
- Agrupar hongos en 'Grupos Sensoriales'
- Obtener % de hongos que pertenecen a cada 'Grupo Sensorial'
1.3: Obtener métrica matemática de riesgo
- Se  obtiene el % de riesgo para cada tipo de olor
* Se obtiene síntesis parcial para a H1