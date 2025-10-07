# Universidad [Universidad Tecnica de Ambato]  
## Facultad de [FISEI]  
### Carrera de Ingeniería en Software  

**Asignatura:** Manejo y Configuración de Software  
**Nombre del Estudiante:** Henry Lagua  
**Fecha:** 7/10/25  

---

# Evaluación Práctica de Git y GitHub

## Instrucciones Generales

- Cada pregunta debe ser respondida directamente en este archivo **(README.md)** debajo del enunciado correspondiente.
- Cada respuesta debe ir acompañada de uno o más **commits**, según se indique en cada pregunta.
- Cuando se indique, deberán realizarse acciones prácticas dentro del repositorio (como creación de archivos, ramas, resolución de conflictos, etc.).
- Cada pregunta debe estar **etiquetada con un tag**, únicamente en el commit final correspondiente, con el formato: `"Pregunta 1"`, `"Pregunta 2"`, etc.

---


## Pregunta 1 (1 punto)

**Explicar la diferencia entre los siguientes conceptos/comandos en Git y GitHub:**

- `git clone`  
- `fork`  
- `git pull`

### Parte práctica:

- Realizar un **fork** de este repositorio en la cuenta personal de GitHub del estudiante.
- Luego, realizar un **clone** del fork en el equipo local.
- En este README, describir el proceso seguido:
  - ¿Cómo se realizó el fork?
  - ¿Cómo se realizó el clone del fork?
  - ¿Cómo se verificó que se estaba trabajando sobre el fork y no sobre el repositorio original?

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta a la Pregunta 1 -->

Explicar la diferencia entre los siguientes conceptos/comandos en Git y GitHub:

El git clone, copia un repositorio remoto a nuestra computadora, 
el fork es una copia independiente de otro repositorio en mi cuenta  para podermodificarlo sin afectar al original, y el git pull es traer todos los cambios que estan en el repositorio remoto a nuestra computadora.


Parte práctica:
- ¿Cómo se realizó el fork?
Ingres al repositorio con el link de la prueba, y atraves el aintervas genere el fork
![alt text](img/image.png)

  - ¿Cómo se realizó el clone del fork?

de ahi me fui al fork que genere y le di en code y me copie el https para clonarlo
![alt text]img/(image.png)
y utilise el comando 
git clone https://github.com/Hlagua/EVALUACION_1P.git
pa copiar el repositorio
![alt text](image-1.png)



  - ¿Cómo se verificó que se estaba trabajando sobre el fork y no sobre el repositorio original?
primero ingrese al repositorio y de ahi utilize le comando git remote -v

![alt text](image-2.png)


---

## Pregunta 2 (1 punto)

**Configurar un archivo `.gitignore` para que ignore:**

- Todos los archivos con extensión `.log`.
- Una carpeta llamada `temp/`.
- Todos los archivos `.md` y `.txt`de la carpeta `doc/`. (Probar agregando un archivo `prueba.md` y un archivo `prueba.txt` dentro de la carpeta y fuera de la carpeta.)

### Requisitos:

1. Realizar un **primer commit** que incluya únicamente el archivo `.gitignore` con las reglas de exclusión definidas.
2. Realizar un **segundo commit** donde se explique en este README la función del archivo `.gitignore` y se muestre evidencia de que los archivos y carpetas indicadas no están siendo rastreadas por Git.

**Importante:**  
- Solo el **segundo commit** debe llevar el **tag `"Pregunta 2"`**.

**📝 Respuesta:**

<!-- Escribe aquí tu explicación y evidencia para la Pregunta 2 -->

1. Realizar un **primer commit** que incluya únicamente el archivo `.gitignore` con las reglas de exclusión definidas.
![alt text](image-3.png)

2. Realizar un **segundo commit** donde se explique en este README la función del archivo `.gitignore` y se muestre evidencia de que los archivos y carpetas indicadas no están siendo rastreadas por Git.

El archivo .gitignore le indica a Git qué archivos o carpetas no deben ir al repositorio remoto.

Verificacion
![alt text](image-4.png)

![alt text](image-5.png)

---

## Pregunta 3 (2 puntos)

**Utilizar Git Flow para desarrollar una nueva funcionalidad llamada `ingresar-encabezado`.**

### Requisitos:

- Inicializar el repositorio con Git Flow, utilizando las ramas por defecto: `main` y `develop`.
- Crear una rama de tipo `hotfix` con el nombre `ingresar-encabezado`.
- En dicha rama, **completar con los datos personales del estudiante** el encabezado que ya se encuentra al inicio de este archivo `README.md`.
- Realizar al menos un commit durante el desarrollo.
- Finalizar el hotfix siguiendo el flujo de trabajo establecido por Git Flow.

### En este README, se debe incluir:

- Los **comandos exactos** utilizados desde la inicialización de Git Flow hasta el cierre del hotfix.
- Una descripción del **proceso seguido**, indicando el propósito de cada paso.
- Una reflexión sobre las **ventajas de aplicar Git Flow**, especialmente en contextos colaborativos o proyectos de larga duración.

**Importante:**

- Deben realizarse varios commits durante esta pregunta.
- **Solo el commit final** debe llevar el **tag `"Pregunta 3"`**.
- El flujo debe respetar la estructura de Git Flow con las ramas `develop` y `main`.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 3 -->

---
- Los **comandos exactos** utilizados desde la inicialización de Git Flow hasta el cierre del hotfix.
git flow init
git flow hotfix start ingresar-encabezado
git add .
git commit -m "Agregar encabezado con datos personales"
git flow hotfix finish ingresar-encabezado


- Una descripción del **proceso seguido**, indicando el propósito de cada paso.
se inicio el git flow el cual configura la estructura de ramas (main, develop, feature, release, hotfix).
de ahi se genero la rama hotfix con el nombre ingresa encabezado,la cual es una rama temporal para corregir errores pequenos ,y se agrego el emcabesado, y se realizo el comit, y se finalizo la rama hotfix con git flow hotfix fisich lo cual fusiona los cambios en main y develop y elimina la rama del hotfix.




- Una reflexión sobre las **ventajas de aplicar Git Flow**, especialmente en contextos colaborativos o proyectos de larga duración.

Permite mantener un flujo de trabajo ordenado, separando el desarrollo principal, las pruebas y los lanzamientos.
En equipos grandes, evita conflictos y facilita el control de versiones en proyectos de larga duración.


## Pregunta 4 (2 puntos)

**Trabajo con Issues y Pull Requests**

### Parte teórica:

- Explicar qué es un **issue** en GitHub.
- Explicar qué es un **pull request** y cuál es su finalidad.
- Indicar la diferencia entre ambos y cómo se relacionan en un entorno de trabajo colaborativo.

### Parte práctica:

- Trabajar en la rama `develop`, ya existente desde la configuración de Git Flow.
- Crear un **issue** titulado `"Respuesta a la Pregunta 4"`, en el que se indique que su objetivo es documentar esta pregunta.
- Realizar los cambios necesarios en este archivo `README.md` para responder esta pregunta.
- Realizar un **commit** con los cambios y subirlo a la rama `develop` del repositorio remoto.
- Crear un **pull request** desde `develop` hacia `main` en GitHub.
- **Vincular el pull request con el issue creado**, de manera que al ser aprobado y fusionado, el issue se cierre automáticamente.
- **Aprobar** el pull request para que se haga el merge respectivo hacia `main`.

### En este README, se debe incluir:

- Un resumen del procedimiento realizado.
- El número y enlace del issue creado.
- El número y enlace al pull request.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 4 -->

---
Parte teórica:

un Issue es un reporte o tarea que describe un problema o mejora del proyecto.

un pull Request es una solicitud para fusionar cambios de una rama a otra.

Un issue indica qué hay que hacer, y un pull request implementa la solución. Cuando el pull request se aprueba, el issue puede cerrarse automáticamente.

Parte práctica:
- Un resumen del procedimiento realizado.
primero se habilito issue en git hub ya que no estaba habilitado, de ahi se genero el isus respuesta preunta 4 con #1, y dea hi se relizo el pull request verificando que sea  al fork de una mismo, y para terminar el issu se puso resolve #1, y no hubi problemas de merge




![alt text](image-7.png)

pull reuqest
![alt text](image-8.png)


resolvio 
![alt text](image-9.png)


- El número y enlace del issue creado.
1
https://github.com/Hlagua/EVALUACION_1P/issues/1

- El número y enlace al pull request.
#2
https://github.com/Hlagua/EVALUACION_1P/pull/2



## Pregunta 5 (2 puntos)

**Resolver conflictos entre ramas y realizar un Pull Request**

### Requisitos:

- Crear dos ramas llamadas `ramaA` y `ramaB`, ambas a partir de la rama `develop`.
- En `ramaA`, crear un archivo llamado `archivoA.txt` con el contenido:  
  `Contenido A`
- En `ramaB`, crear un archivo con el mismo nombre (`archivoA.txt`), pero con el contenido:  
  `Contenido B`
- Intentar fusionar `ramaB` sobre `ramaA`, lo cual debe generar un conflicto.
- Resolver el conflicto combinando ambos contenidos.
- Realizar el merge de `ramaA` hacia `develop`.
- Crear un **pull request** desde `develop` hacia `main`.
- Una vez completado lo anterior, eliminar las ramas `ramaA` y `ramaB` tanto local como remotamente.

### En este README, se debe incluir:

- El procedimiento completo:
  - Cómo se crearon las ramas.
  - Cómo se generó y resolvió el conflicto.
  - Cómo se realizó el merge hacia `develop`.
  - Cómo se eliminaron las ramas al finalizar.
- El enlace al pull request.
- Una breve explicación de qué es un conflicto en Git y por qué ocurrió en este caso.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 5 -->


---
- El procedimiento completo:
  - Cómo se crearon las ramas.

![alt text](image-10.png)



  - Cómo se generó y resolvió el conflicto.

  ![alt text](image-11.png)

se realizo el merge en vscode

  - Cómo se realizó el merge hacia `develop`.

![alt text](image-12.png)

  - Cómo se eliminaron las ramas al finalizar.
![alt text](image-13.png)


- El enlace al pull request.
https://github.com/Hlagua/EVALUACION_1P/pull/3


- Una breve explicación de qué es un conflicto en Git y por qué ocurrió en este caso.
Un conflicto en Git ocurre cuando dos ramas modifican la misma parte de un archivo y Git no puede decidir cuál conservar.
En este caso, ambas ramas editaron archivoA.txt, lo que generó un conflicto que resolví manualmente combinando ambos contenidos.





## Pregunta 6 (2 puntos)

**Realizar limpieza, explicar versionamiento semántico y enviar cambios al repositorio original**

### Requisitos:

- Trabajar en la rama `develop` del fork del repositorio.
- Eliminar los archivos `archivoA.txt` y `archivoB.txt` creados en preguntas anteriores.
- Realizar un merge desde `develop` hacia `main` en el repositorio local.
- Enviar los cambios de la rama `main` local a la rama `develop` del repositorio remoto (fork). Recuerde incluir todos los tags creados (6 tags).
- Finalmente, crear un **pull request** desde la rama `develop` del fork hacia la rama `main` del repositorio original (del cual se realizó el fork en la Pregunta 1). El titulo del pull request debe ser "NOMBRE APELLIDOS", en la descripción colocar el link de su repositorio de GitHub.

### En este README, se debe incluir:

- Una explicación del proceso realizado paso a paso.
- Una explicación del **versionamiento semántico**, indicando:
  - En qué consiste.
  - Sus tres componentes (MAJOR, MINOR, PATCH).
- El enlace al pull request creado hacia el repositorio original.
- Si hace falta agregar alguna evidencia adicional, agregue un tag adicional que sea `Version Final`.

**📝 Respuesta:**

<!-- Escribe aquí tu respuesta completa a la Pregunta 6 -->
