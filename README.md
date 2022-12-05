# ISIS 4822 - Visual Analytics | Proyecto - Cáncer de mama

- Hernán Cuy | 202010199 | [h.cuy@uniandes.edu.co](mailto://h.cuy@uniandes.edu.co)
- Camilo Rozo | 201820147 | [ce.rozob@uniandes.edu.co](mailto://ce.rozob@uniandes.edu.co)

---

- Storytelling | [Cancer, una condición sin distinción en Github pages](https://hernancuy.github.io/ProyectoVisualization/)

- Dashboard | [Dashboard en Tableau Public](https://public.tableau.com/views/ISIS4822_VisualAnalytics_Proyecto-cncerdemama_Dashboard/Cancerunacondicinsindistincin?:language=es-ES&:display_count=n&:origin=viz_share_link)

---

## Contexto del problema y caracterización del usuario final

### Contexto del problema

Una entidad de salud colombiana cuenta con datos de pacientes que se encuentran, o se encontraban en algún momento, en tratamiento de cáncer de mama. Estos datos son recopilados anualmente por la entidad y se planea que en el futuro esto siga ocurriendo. El conjunto de datos consiste de registros de pacientes, incluyendo información demográfica y valores resultado de tratatamientos (por ejemplo, el resultado de un diagnóstico) a los que el paciente ha sido sometido a lo largo del tiempo.

El objetivo es utilizar estos datos de pacientes para analizar la evolución tanto de la enfermedad de los pacientes, como la eficacia del tratamiento brindado por la entidad.

### Perfil de usuarios finales[^1]

- _Personal de salud:_ personal médico con experiencia y conocimientos especializados en las diferentes etapas del tratamiento del cáncer de mama. Los cuales podrán determinar la eficacia del tratamiento brindado por la entidad, así como la evolución de la enfermedad de los pacientes.

- _Personal académico:_ profesores especializados en visualización y análisis de datos. Cuyo objetivo es verificar el cumplimiento de los objetivos de la entidad con la visualización en términos de usabilidad y hallazgo de insights.

[^1]: Debido a que no fue posible firmar los acuerdos de confidencialidad a tiempo, no fue posible interactuar con el personal de salud en lo absoluto, por lo cual, los insights y el desarrollo del proyecto se llevó a cabo únicamente con el personal académico como usuario final.

## Bitácora de validación y prototipado


| Fecha      | Objetivo                                                                                     | Participantes                                                                                    |
|------------|----------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| 24/10/2022 | Revision # 1 : Objetivos y   contextualización de proyecto.                                  | Usuario:       - Maria del Pilar Villamil      Estudiantes:      - Camilo Rozo      - Hernan Cuy |
| 29/10/2022 | Revision # 2 : Definicion de   alcances                                                      | Usuario:       - Jose Tiberio Hernandez      Estudiantes:      - Camilo Rozo      - Hernan Cuy   |
| 3/11/2022  | Revision # 3: Retroalimentación   cliente-estudiante Mockup N°1                              | Usuario:       - Estudiantes ISIS 4822      Estudiantes:      - Camilo Rozo      - Hernan Cuy    |
| 24/11/2022 | Revision # 4: Verificación   Avances por correo electronico con usuario final segundo mockup | Usuario:       - Maria del Pilar Villamil      Estudiantes:      - Camilo Rozo      - Hernan Cuy |
| 24/11/2022 | Revision # 5: Demostración clase   avance mockup n° 2                                        | Usuario:       - Estudiantes ISIS 4822      Estudiantes:      - Camilo Rozo      - Hernan Cuy    |
|  1/12/2022 | Revision # 6: Verificación   prototipo funcional con usuario final                           | Usuario:       - Maria del Pilar Villamil      Estudiantes:      - Camilo Rozo      - Hernan Cuy |
|  1/12/2022 | Revision # 5: Demostración clase   prototipo final.                                          | Usuario:       - Estudiantes ISIS 4822      Estudiantes:      - Camilo Rozo      - Hernan Cuy    |

## Tareas principales del proyecto[^2]

[^2]: _Debido al conflicto con el acuerdo de confidencialidad, se adicionaron tareas acordes a los insights obtenidos por el personal académico junto con las tareas planteadas originalmente_


### Tareas planteadas originalmente

- _Tarea 1 | Principal:_ **Comparar** la **Distribución** de los resultados de los tratamientos de los pacientes a lo largo del tiempo.

- _Tarea 2 | Secundaria:_ **Identificar** **Tendencias** de mejoría en los tratamientos ofrecidos por la entidad de salud.

- _Tarea 3 | Secundaria:_ **Localizar** **Casos atípicos (Outliers)** en tratamientos de pacientes.

### Tareas secundarias adicionadas

- _Tarea 4 | Secundaria:_ **Resumir** las **Características** del tiempo de progresión de los pacientes a lo largo del tratamiento.

- _Tarea 5 | Secundaria:_ **Buscar** la **Distribución** de la ubicación de los pacientes en el territorio nacional.

- _Tarea 6 | Secundaria:_ **Identificar** **Casos atípicos** en los valores de los datos crudos presentes en el dataset.

### Cumplimiento de tareas

|  Tarea  | Cumplimiento | Justificación                                                                                                                                                                                                                                                                                |
| :-----: | :----------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tarea 1 |      🟩      | La distribución de los resultados actuales a lo largo del tiempo es comparable rápidamente con el diagrama de barras de la pestaña #5 del storytelling                                                                                                                                       |
| Tarea 2 |      🟩      | El diagrama de barras de la pestaña #5 del storytelling permite visualizar la tendencia de los pacientes a sobrevivir el tratamiento viendo las proporciones entre sí de los diferentes valores de desenlace en cada año, y filtrar aquellas que se vean sobrerrepresentadas                 |
| Tarea 3 |      🟨      | Es posible identificar _valores atípicos_ en algunas variables presentes en los modismos, sin embargo, no hay manera de localizar exactamente el paciente atípico de forma individual                                                                                                        |
| Tarea 4 |      🟥      | A pesar de que el diagrama de líneas del dashboard muestra la progresión promedio de los pacientes, no hay datos suficientes como para concluir con certeza o tomar alguna decisión sobre los datos mostrados                                                                                |
| Tarea 5 |      🟩      | El mapa del dashboard da un buen indicio de la distribución _geográfica_ de la población, además, el diagrama de burbujas complementa mostrando mejor la distribución _en cantidad_ de la población, así como representando aquellos lugares que no aparecen en el mapa por diversas razones |
| Tarea 6 |      🟩      | En general, todas las visualizaciones exhiben las anomalías de cada atributo usado. Incluyendo datos faltantes, errores de digitación, y etiquetado incorrecto de variables                                                                                                                  |

## Principios de diseño de visualización y codificación

![How](https://user-images.githubusercontent.com/60525731/205521586-cd683f02-5619-405a-88ac-2fa314432009.jpg)

## Mockups iniciales y bocetos

Para este proyecto se realizaron diferentes maquetados y prototipos, inicialmente pensando en la interacción directa que el cliente deseaba tener sobre la herramienta y segundo sobre el tipo de visualización que mejor mostrara los datos a obtener.

### Primera iteración

La idea inicial era con el modismo de barras verticales mostrar los diferentes tipos de desenlaces, este gráfico tendría interactividad seleccionando el tipo de deselance requerido mostraría la información relevante o relacionada en los modismos inferiores.En este, se visualiza al lado izquierdo los filtros que en su momento el usuario requiera realizar, al lado derecho se encuentran los diferentes modismos para graficar la información.

![Wireframe1](https://user-images.githubusercontent.com/60525731/205504943-3f5fa751-4650-433f-b398-e35a0caa3117.JPG)

[Wireframe completo | Figma](https://www.figma.com/proto/UG9fp2ht1vsIaCJOjQRBv7/Wireframe?page-id=0%3A1&node-id=1%3A3&viewport=766%2C257%2C0.23&scaling=scale-down&starting-point-node-id=1%3A3)

### Segunda iteración

Para la segunda iteracion, se decidió mostrar mejoras como los titulos de cada gráfica y los filtros comparativos. Adicionalmente, se definieron los modismos para las gráficas dependientes y como se mostrarían los resultados.

![Mockup1](https://user-images.githubusercontent.com/60525731/205505402-33c0c7aa-c9cb-4c6c-be8c-57177d8cca11.JPG)

[Mockup Completo | Figma](https://www.figma.com/file/xMjwNqJZfp5Nl1xXYZ38GG/Mockup?node-id=0%3A1&t=jpyaiwAopy7wlerm-1)

### Tercera iteración y correcciones finales

Para la tercera iteracion, creamos el modelo funcional con el conjunto de datos real realizado en tableau. Para este prototipo faltaba 
la integracion de los filtros y organizar la disposición de los modismos.

![Mockup3](https://user-images.githubusercontent.com/60525731/205505775-20e59b9c-3b29-47ec-abbc-ec7839a915a9.JPG)

Finalmente, ara la ultima iteracion se genero un dashboard interactivo, en el cual se visualiza totalmente los datos con sus filtros tales como rango de fecha y desenlace clinico.

![Dashboard](https://user-images.githubusercontent.com/60525731/205507628-143cd33f-d257-4f0d-8e44-e912da199107.JPG)

## Insights y feedback obtenidos con la herramienta[^3]

[^3]: _Debido al conflicto con el acuerdo de confidencialidad, los insights fueron obtenidos a partir del personal académico (tanto clientes como encontrados por nosotros) y orientados tanto a hallazgos sobre los pacientes como hacia la aplicabilidad del proyecto del curso en la implementación existente del proyecto de cáncer de mama_

### Storytelling

- La costumbre es usar el eje horizontal como tiempo o número de etapa, por lo que usar las etapas en el eje vertical en simultáneo con el tiempo resulta confuso.
- En los últimos 5 años previos al año actual del dataset, el número de pacientes que están en tratamiento ha aumentado en un 609.77% (de 133 a 944)
- En comparación a lo anterior, la cantidad de pacientes que abandonan el tratamiento tuvo su pico un año antes del año actual del dataset con 40 abandonos, que se redujo a 10 en el año actual del dataset y en ambos casos no supera el 6% del total de pacientes en tratamiento (5.6% y 1.05%). Por lo que sí se percibe mejoría
- El uso de una persona como Andrea Morales como ejemplo de paciente es muy útil para entender la información mostrada en el storytelling
- El uso de la persona da pie a plantear ideas sobre cómo navegar desde el panorama general hacia el detalle de un paciente en particular.

### Dashboard

- El layout del dashboard era confuso [corregido posterior a la validación]
- Habría sido interesante filtrar por el tipo del desenlace del paciente [corregido posterior a la validación]
- 22.25% de los pacientes (178 de 800) no cuenta con información geográfica alguna, lo que hace que el mapa represente de forma incompleta a pacientes ubicados en ciudades no principales.
- Hay muy pocos datos de progresión para ser una variable tan importante, la máxima cantidad de registros se consiguieron un año antes del año actual del dataset, unicamente con 14 registros, lo que hace que el diagrama de líneas actual no sea representativo de la realidad.

### General

El personal académico con el que se validaron las etapas del proyecto usaron esta implemementación en Tableau como punto de partida para un posible replanteamiento de la implementación de la herramienta del cliente. Y en ese sentido se concluyó con lo siguiente:

- El uso de Tableau para el proyecto puede ser inviable debido al costo de las licencias y a la diversidad de alternativas por las que las entidades de salud podrían tener preferencia.

- El uso de Nivo en la herramenta del cliente ha causado limitaciones importantes a lo largo del desarrollo del mismo, por lo que, entre las alternativas de: continuar con nivo, migrar lo existente a D3/Vega/Tableau/PowerBI o mantener Nivo en su estado actual y continuar lo pendiente con D3/Vega/Tableau/PowerBI. La recomandación es mantener lo existente de Nivo, continuar con un intento en Vega/Vega-lite a manera de piloto y por último evaluar migrar lo existente en Nivo a Vega.  

- Hay problemas de rendimiento con los datos en Tableau, este hallazgo es importante porque la implementación del proyecto del cliente, basada en web, tiene el rendimiento como prioridad. Por lo que vale la pena evaluar la composición de los datos para ver si es posible reducirlos de alguna manera.

## Manual de usuario

[Video de manual de usuario | Youtube](https://youtu.be/6RlYBRGwMJw)
