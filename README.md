# Tarea-2-Paradigmas
Sistema de Evaluacion - Taxonomia de BLoom

Por: Sebastian Alejandro Abarca Acevedo

-------------------------------------
Descripcion General Del Proyecto
-------------------------------------

Este sistema permite aplicar pruebas copmuestas por items (preguntas) que son clasificados segun los niveles de la Taxonomia de Bloom.
El programa es desarrollado en Java utilizando el framework Swing, y tiene como objetivo aplicar, registrar y evaluar examenes. Con resultados desglosados por tipo de item y nivel Taxonomico.

Este sistema cumple con los siguientes requisitos:
1.- Carga de Items/Preguntas desde un archivo de texto.
2.- Aplicacion de una prueba visualmente, mostrando un item por vez.
3.- Registro de respuestas del usuario.
4.- Calculo y visualizacion de resultados segun:
	- Nivel de Taxonomia de Bloom.
	- Tipo de item (Seleccion multiuple o verdadero/falso)

---------------------------------------
Alcances y supuestos
---------------------------------------

- El sistema solo admite items de tipo [Multiple] (Seleccion Multiple) y [vf] (verdadero o falso)
- Cada item tiene una unica respuesta correcta.
- El archivo con los items debe estar correctamente formateado, segun de describira mas adelante.
- Las respuestas se mantienen al navegar entre items, pero no se almacenan en un archivo.

---------------------------------------
Requisito del sistema
---------------------------------------
- Java JDK 17 o superior
- Cualquier entorno de desarrollo que soporte Java
- Sistema operativo Windows, Linux o macOS
- Archivo `items.txt` con las preguntas a cargar

---------------------------------------
Instrucciones de Ejecucion
---------------------------------------
1. Abrir el proyecto en un entorno de desarrollo Java
2. Ejecutar la clase `Main.java`.
3. En la ventana que se abre:
   - Haz clic en “Cargar archivo de ítems”.
   - Se simula la carga de preguntas desde un archivo.
   - Luego haz clic en “Iniciar prueba”.
   - Navega entre las preguntas y responde.
   - Al finalizar, se muestra un resumen (en desarrollo).

---------------------------------------
Formato de achivo con Items
---------------------------------------
-El archivo debe tener extensión .txt y estar codificado en UTF-8.
-Cada línea representa una pregunta y debe contener exactamente 9 campos, separados por punto y coma (;).
-No usar punto y coma (;) dentro del texto de la pregunta ni de las opciones, ya que es el separador de campos.
-Las preguntas de tipo vf (Verdadero/Falso) también deben tener 4 campos de opciones, aunque 2 estén vacíos (;;).

[0] Pregunta (sin punto y coma interno)
[1] Opción A
[2] Opción B
[3] Opción C (puede estar vacía: dejar como ;)
[4] Opción D (puede estar vacía: dejar como ;)
[5] Respuesta correcta (debe coincidir exactamente con una de las opciones)
[6] Tipo de ítem: `multiple` o `vf`
[7] Nivel de la taxonomía: `Recordar`, `Entender`, `Aplicar`, `Analizar`, `Evaluar`, `Crear`
[8] Tiempo estimado para responder (solo números enteros en segundos)


Ejemplo de item valido:
¿Qué es Java?;Un lenguaje;Un compilador;Una base de datos;Un hardware;Un lenguaje;multiple;Recordar;60 (Multiple)
La JVM interpreta el código Java.;Verdadero;Falso;;; ;Verdadero;vf;Entender;30 (Verdadero o Falso)

---------------------------------------
Contacto
---------------------------------------
Cualquier duda sobre la ejecución o estructura puede escribirse a [s.abarcaacevedo@uandresbello.edu]
