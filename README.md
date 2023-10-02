# Revisar procesos con Prefect
Materia: Computación Tolerante a Fallas<br>
Maestro: MICHEL EMANUEL LOPEZ FRANCO<br>
Nombre: Diego Alonso Mercado Brizuela<br>
Carrera: Ingeniería en Computación<br>
Código: 215425636<br>
Fecha: 02/10/2023<br>
Sección: D06<br>
## Introducción
Una aplicación consta de uno o varios procesos. Un proceso, en los términos más sencillos, es un programa en ejecución. Uno o varios subprocesos se ejecutan en el contexto del proceso. Un subproceso es la unidad básica a la que el sistema operativo asigna tiempo de procesador. Un subproceso puede ejecutar cualquier parte del código de proceso, incluidos los elementos que está ejecutando actualmente otro subproceso.
## Pruebas
Esta práctica consta de utilizar la librería "prefect" con la que lograremos ver el flujo de procesos en nuestro programa, lo que permitirá ver a detalle lo que estamos ejecutando.
<br>
Como ejemplo se usó la api de coingecko, lo que nos dará información de criptomonedas.
<br>
La primer task es traer el precio de la moneda dogecoin.
<br>
<img
src="https://github.com/Diego3207/Workflow-managers/blob/main/C%C3%B3digo%201.png">
<br>
La segunda tarea es tratar los datos, extráyendo los datos del objeto json.
<br>
<img
src="https://github.com/Diego3207/Workflow-managers/blob/main/C%C3%B3digo%202.png">
<br>
Por último intenté usar un bot para enviarnos un mensaje por telegram, que nos indicara cuando el precio de la moneda bajase y otro para cuando subiese la moneda.
<br>
Sin embargo no fué posible por temas de configuraciones.
<br>
<img
src="https://github.com/Diego3207/Workflow-managers/blob/main/C%C3%B3digo%203.png">
<br>
Se agregó un temporizador para que repita el flujo de trabajo cada 10 segundos
<br>
<img
src="https://github.com/Diego3207/Workflow-managers/blob/main/C%C3%B3digo%204.png">
<br>
Resultados.
<br>
<img
src="https://github.com/Diego3207/Workflow-managers/blob/main/Evidencia%201.png">
# Conclusiones
Verificar cómo funciona nuestro código ya en funcionamiento es una tarea que todo programador debería conocer para poder evaluar temas de rendimiento, de fallas, para evitar retrasos a la hora de evaluar en el mismo código cómo solventar los errores, sino en la ejecución.
