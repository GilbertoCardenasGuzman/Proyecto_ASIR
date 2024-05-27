# Utilizar Git en un Proyecto Web - Tutorial
## INTRODUCCIÓN SOBRE GIT
Git es muy util y cuenta con una amplia cantidad de ventajas y beneficios entre las cuales encontramos:

### 1.Permite controlar las versiones
Imagina que realizar un proyecto hace 2 años y a día de hoy te apetece volver a brindarle tiempo a dicho proyecto, pues git se encarga de revisar los cambios de versión en ese tiempo transcurrido.

### 2.Colaboración entre desarrolladores
Teniendo en cuenta un proyecto que te da tu empresa, te das cuenta que tu solo no puedes llevar a cabo la tarea, por lo que el proyecto se realizará en grupo , pues gracias a git cada miembro del equipo puede trabajar en su propio dispositivo y en su propio branch para luego fucionar los cambios sin comflictos importantes.

### 3.Seguridad
Git usa SHA-1 para asegurar la integridad del código. Cada cambio es identificado de manera única y de manera encriptada, lo que hace que sea prácticamente imposible modificar el historial sin ser detectado.


## INSTALACIÓN DE GIT
Primero abriremos nuestra terminal o CMD para a continuación escribir los siguientes comandos

```bash
sudo apt update #para buscar actualizaciones de git
sudo apt install git #para instalar git
git --version #para verificar la versión de git instalada
```

## CREACIÓN DE UN PROYECTO CON GIT
Para demostrar mas facilmente como usar git, crearemos una carpeta con un documento html dentro de dicha carpeta

```bash
mkdir proyecto #crear un directorio con el nombre proyecto
cd proyecto
touch proyecto.html #crear el documento html
```
Para poder modificar este documento usaremos el editor de texto a preferencia, en mi caso recomendaria usar el nano

```bash
nano proyecto.html 
#Usar este comando cuando estes dentro de la carpeta donde este el documento
```
Dentro del nano escribiremos una estuctura basica de un html

```bash
<!doctype html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>El título de mi página</title>
  </head>

  <body>
    <header>
      <h1>Hola mundo</h1>
    </header>

    <p>Este es un proyecto html</p>
  </body>
</html>
```
Ahora bien para crear un repositorio y subir dicha carpeta con su documento que hemos creado procederemos a usar el comando git init y git add . para que quede tal que asi:

```bash
git init #Iniciar la repo

git status #Verificar que documentos no estan preparados para el backup

git add . #Añadimos a la repo todos los documentos que modificiamos o de la carpeta
```
Si quieres indagar un poco respecto a que otros comandos puedes usar con git estaran en [AQUI](https://www.atlassian.com/es/git/glossary#commands).

Finalmente, para crear un commit en git usaremos el siguiente comando.

```bash
git commit -m "escribir un mensaje"
```
Al commit puedes añadirle un pequeño comentario que te ayuda a recordar dichoso commit