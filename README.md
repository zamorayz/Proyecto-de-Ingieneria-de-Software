# Evidencia 2 - Instrucciones y rúbrica de evaluación

Instrucciones 

Pare realizar esta evidencia reúnanse con su equipo scrum. 

Recopilen los documentos y archivos de las fases weight tokens, query y web interfaz. 

Incluyan los siguientes elementos scrum: 

Historias de usuario generadas al inicio de cada Sprint. 

 

HU-1.1 (Apertura de Archivos HTML) 

Como Product Owner, 

Quiero que el sistema pueda abrir los archivos HTML originales sin renombrarlos utilizando una función específica (ej. open_file), 

HU-1.2 (Limpieza de Etiquetas HTML) 

Como Desarrollador, 

Quiero crear una función (ej. remove_html_tags) que busque y elimine todas las etiquetas HTML de los archivos de entrada, generando un nuevo archivo de salida limpio, 

HU-1.3 (Extracción, Ordenamiento y Logs de Tiempo) 

Como Scrum Master, 

Quiero que el programa extraiga las palabras separadas por un salto de línea, las ordene alfabéticamente y genere archivos log (a1_matricula.txt, a2_matricula.txt, a3_matricula.txt) con los tiempos de ejecución. 

HU-2.1 (Archivo Consolidado en Minúsculas) 

Como Product Owner, 

Quiero generar un archivo consolidado que contenga todas las palabras de todos los archivos convertidas a minúsculas y ordenadas alfabéticamente, 

HU-2.2 (Frecuencias y Ejecución por Comandos) 

Como Desarrollador, 

Quiero habilitar la ejecución mediante línea de comandos (ej. Tokenize.exe input-dir output-dir), eliminar palabras duplicadas y generar un archivo que muestre los tokens y su frecuencia ordenados por número de repeticiones. 

HU-2.3 (Diccionario de 3 Columnas y Tiempos) 

Como Scrum Master, 

Quiero modificar el programa para crear un diccionario ASCII con tres columnas (Token, Repeticiones, # de archivos con ese token) y exportar los logs de tiempos (a4_matricula.txt, a5_matricula.txt, a6_matricula.txt), Para tener una vista clara de la distribución de los tokens en la colección de documentos y medir la velocidad del equipo. 

HU-3.1 (Estructura Posting y Stop List) 

Como Product Owner, 

Quiero crear un archivo de posting que relacione los documentos con el diccionario e implementar un stop list para eliminar palabras muy cortas (1 letra/dígito) o de baja frecuencia para limpiar el ruido del diccionario y conectar los términos con sus documentos de origen. 

HU-3.2 (Hash Table y Peso TF-IDF) 

Como Desarrollador, 

Quiero implementar una Hash Table para almacenar los tokens registrando el número de colisiones, y reemplazar la columna de frecuencias en el posting por el cálculo del peso tf.idf = (# repeticiones * 100) / # total de tokens en el documento, para normalizar el valor de las palabras y garantizar búsquedas en memoria altamente eficientes. 

HU-3.3 (Optimización de Bytes y Auditoría) 

Como Scrum Master, 

Quiero definir un tamaño fijo en bytes para las columnas del diccionario (ej. 20 bytes) y posting (ej. 10 bytes) para facilitar lecturas de disco, y generar los logs (a7_matricula.txt, a8_matricula.txt, a9_matricula.txt, a10_matricula.txt), para asegurar que la arquitectura de datos sea escalable y registrar la velocidad del sprint. 

HU-E1.1 (Recopilación de Artefactos Ágiles) 

Como Product Owner, 

Quiero recolectar las historias de usuario, el product backlog antes/después, los casos de prueba y los escenarios creados, para respaldar la gestión ágil del proyecto ante las validaciones de calidad. 

HU-E1.2 (Comandos de Sistema Unix/DOS) 

Como Desarrollador, 

Quiero unificar el código para que funcione exclusivamente mediante dos comandos DOS/Unix: tokenize input-dir output-dir e index input-dir output-dir utilizando la Hash Table y el Posting, para entregar un motor de preprocesamiento e indexación funcional e independiente. 

HU-E1.3 (Análisis de Rendimiento y Gráficas) 

Como Scrum Master, 

Quiero realizar pruebas variando la cantidad de documentos (10, 20, 30, 40, 50), generar gráficas de tiempos (Tokenización y Tokenización+Indexación), detallar el hardware de prueba y documentar el diagrama de flujo, para demostrar empíricamente la eficiencia y complejidad temporal del algoritmo. 

HU-4.1 (Índice de Documentos y Motor Retrieve) 

Como Product Owner, 

Quiero crear un catálogo de documentos asignándoles un ID único para usarlo en el posting, y un comando retrieve que devuelva la lista de nombres de archivos HTML que contienen una palabra buscada (ej. retrieve gato), para presentar resultados legibles al usuario y normalizar la base de datos. 

HU-4.2 (Búsqueda Optimizada en Disco y Top 10 

Como Desarrollador, 

Quiero modificar el programa para que lea directamente del disco usando la posición del Hash (sin precargar la tabla en memoria RAM), soportar múltiples tokens de búsqueda y mostrar únicamente un "Top 10" de documentos más relevantes, para maximizar el rendimiento de la búsqueda y ofrecer los resultados matemáticamente más significativos. 

HU-4.3 (Migración Ágil y Logs de Búsqueda) 

Como Scrum Master, 

Quiero migrar el control del proyecto a una herramienta ágil (Jira/IceScrum/Taiga), evaluar el Burn Down Chart e implementar logs de tiempo exactos (a11_matricula.txt, a12_matricula.txt, a13_matricula.txt) por cada consulta ejecutada, para cerrar la fase de Query comprobando tiempos de respuesta a nivel milisegundo y consolidando el uso de herramientas de la industria. 

HU-5.1 (Interfaz web del motor de búsqueda) 

Como Scrum Master, 

Quiero implementar una página web con un cuadro de texto para realizar búsquedas mediante el motor de búsqueda, permitiendo ingresar consultas desde el navegador y generar resultados dinámicos ordenados por relevancia, para facilitar la interacción del usuario con el sistema de búsqueda y comprobar el funcionamiento de la interfaz web CGI. 

HU-5.2 (Pruebas de Carga con JMeter) 

Como Scrum Master, 

Quiero ejecutar pruebas de carga utilizando JMeter con 25 usuarios concurrentes y tiempos de respuesta máximos de 2000 milisegundos para analizar el comportamiento del servidor durante múltiples consultas simultáneas, para evaluar el rendimiento del motor de búsqueda, monitorear el consumo de CPU/I/O y validar la estabilidad del sistema bajo estrés. 

HU-5.3 (Resultados con Ranking y Enlaces) 

Como Scrum Master, 

Quiero que el motor de búsqueda muestre el nombre del documento hallado, tenga un hipervínculo funcional y el ranking TF-IDF correspondiente para cada resultado obtenido, 

Para permitir la navegación entre documentos y visualizar los resultados ordenados según su relevancia. 

HU-E2.1 (Validación de Stopwords y Tokens) 

Como Scrum Master, 

Quiero comprobar que el motor de búsqueda elimine correctamente las stopwords, convierta los tokens a minúsculas y limite el tamaño máximo de los tokens procesados, para garantizar la limpieza y estandarización de los datos utilizados en el índice de búsqueda. 

HU-E2.2 (Resultados Web con Ranking y Top 10) 

Como Scrum Master, 

Quiero que el buscador web muestre el Top 10 de documentos ordenados mediante ranking TF-IDF y enlaces funcionales hacia cada página encontrada, para validar la relevancia de los resultados y facilitar la navegación del usuario dentro del sistema de búsqueda. 

HU-E2.3 (Pruebas de Rendimiento CGI con JMeter) 

Como Scrum Master, 

Quiero ejecutar pruebas de carga mediante JMeter utilizando múltiples usuarios concurrentes y llamadas CGI en Apache, para analizar los tiempos de respuesta, estabilidad del ejecutable buscador_web.exe y el comportamiento del servidor bajo condiciones de estrés. 

 

Lista de historias en el product backlog antes y después de cada sprint. 

 

 

 

Antes: 

 

 

 

Después: 

 

 

Casos de prueba creados a lo largo de cada sprint. 


Sprint 1: 

 

ID 

Caso de prueba 

Resultado esperado 

Resultado obtenido 

CP-1.1 

Abrir archivos HTML 

El sistema abre correctamente archivos HTML 

Correcto 

CP-1.2 

Eliminar etiquetas HTML 

El texto queda limpio sin etiquetas 

Correcto 

CP-1.3 

Generar tokens 

El sistema genera tokens ordenados 

Correcto 

Sprint 2: 

 

Columna1 

Columna2 

Columna3 

Columna4 

ID 

Caso de prueba 

Resultado esperado 

Resultado obtenido 

CP-2.1 

Convertir texto a minúsculas 

Todos los tokens quedan en minúsculas 

Correcto 

CP-2.2 

Calcular frecuencias 

Se generan frecuencias por palabra 

Correcto 

CP-2.3 

Crear diccionario 

El diccionario se almacena correctamente 

Correcto 

 

Sprint 3: 

 

ID 

Caso de prueba 

Resultado esperado 

Resultado obtenido 

CP-3.1 

Aplicar stopwords 

Las stopwords son eliminadas. 

Correcto 

CP-3.2 

Calcular TF-IDF 

Los documentos se ordenan por relevancia. 

Correcto 

CP-3.3 

Optimizar búsquedas 

Disminuyen tiempos de consulta. 

Correcto 

 

Sprint 4: 

 

ID 

Caso de prueba 

Resultado esperado 

Resultado obtenido 

CP-4.1 

Ejecutar comandos DOS/Unix 

Los comandos funcionan correctamente 

Correcto 

CP-4.2 

Generar gráficas 

Se muestran métricas del sistema 

Correcto 

CP-4.3 

Analizar rendimiento 

Se detectan tiempos de respuesta altos 

Correcto 

 

 

Sprint 5: 

 

ID 

Caso de prueba 

Resultado esperado 

Resultado obtenido 

CP-5.1 

Realizar búsqueda web 

El sistema devuelve resultados 

Correcto 

CP-5.2 

Mostrar Top 10 

Solo se muestran 10 resultados 

Correcto 

CP-5.3 

Ejecutar CGI en Apache 

Apache ejecuta correctamente el archivo buscador_web.exe 

Correcto 

 

 

Gráfica con la velocidad del equipo en cada sprint. 

 

 

 

La velocidad del equipo fue calculada mediante los story points que fueron completados en cada sprint dentro de Jira Software. Durante las primeras fases de la 1 a la 4 del proyecto se mantuvo una velocidad constante de 10 puntos, reflejando estabilidad en el desarrollo del motor de búsqueda. En los sprints 5 y evidencia 2 la velocidad disminuyó a 8 ya que las actividades estuvieron enfocadas principalmente en integración CGI, pruebas de carga con JMeter, optimización y documentación de la Evidencia 2. 

 

 

 

 

 

Backlog con todas las fases e historias de usuario en TFS. 

 

 

Agreguen los siguientes elementos funcionales en el programa: 

 

Fecha de inicio fecha de cierre 

 

Comprobar que su programa elimine los stopwords, ponga los tokens en minúsculas y los tokens tengan un tamaño máximo definido. 

El buscador debe enlistar el top 10 de los documentos con un rank y el link funcional para cada documento. 

El programa no debe cargar el índice o diccionario en memoria, debe accederlo directamente en disco. 

Demostrar que la interfaz de la página web realiza llamadas CGI o equivalentes al momento de realizar la búsqueda. 

Resultados: 

Lectura en Disco y TF-IDF Funcionan: Los resultados no están en orden alfabético ni de ID, sino por relevancia (el de 0.542 hasta arriba y el de 0.0021 abajo). 

Límite del Top 10: El algoritmo se detiene exactamente en el resultado número 10, tal como se pedía en la Actividad 13 y se exige en la Evidencia 2. 

 

Interfaz CGI Exitosa: Apache logró invocar el .exe(buscador_web.exe), pasarle la variable uno y devolver el HTML formateado. 

 

  

  

Incluyan la dirección de su buscador web para que sea probado localmente. 

Realicen las impresiones de pantalla y las búsquedas de cada una de las siguientes consultas: 

Exploitation 

 

Higiene 

 

exploitation higiene 

 

Arkansas 

 

gift!! Person? 

 

the 

 

elephants 

 

Gauch 

 

20 

 

Realicen el diagrama de flujo del programa. 

 

Presenten los resultados de pruebas de carga en TFS. 

 

 

 

 

  

La prueba de carga se realizó con los 25 usuarios concurrentes solicitados. El Árbol de Resultados de JMeter arrojó códigos de respuesta HTTP 200 (OK), lo que demuestra que el ejecutable CGI en C++ es estable y no presentó caídas (no hubo errores 500). Sin embargo, se registró un promedio de 99% de error en la métrica debido a la Aserción de Duración. La carga concurrente de lectura directa a los archivos de texto en el disco duro generó un cuello de botella de I/O, provocando que los tiempos de respuesta superaran el límite establecido de 2000 ms (2 segundos). Esto demuestra el punto máximo de estrés de nuestra arquitectura actual bajo el protocolo CGI. 
