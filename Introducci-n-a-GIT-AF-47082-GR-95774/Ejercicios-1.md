# Ejercicios - Tema 1: Introducción

A continuación, encontrarás 10 ejercicios prácticos sobre la introducción a Git y GitHub. Intenta resolverlos antes de consultar la teoría.

---

## Ejercicio 1. Conceptos básicos

Explica con tus palabras qué es Git y para qué sirve. Después, responde también qué diferencia existe entre Git y GitHub.

---
Git es la aplicación que permite registrar en local los cambios que se hacen en un proyecto (archivos en una carpeta de diferentes tipos).
GitHub es el repositorio online del proyecto, con los cambios registrados en un histórico.


## Ejercicio 2. Instalación de Git

Instala Git en tu equipo según tu sistema operativo. Cuando termines, abre la terminal y ejecuta el comando necesario para comprobar que Git se ha instalado correctamente. Escribe el comando utilizado y anota la versión que te aparece.

---
git -v
git version 2.54.0.windows.1


## Ejercicio 3. Configuración inicial

Configura Git con tu nombre y tu correo electrónico en modo global. Después, ejecuta el comando necesario para comprobar que la configuración se ha guardado correctamente.

---
git config --global user.name "Antonio Mena"
git config --global user.email "antonio.mena.contractor@bbva.com"
git log -n 5


## Ejercicio 4. Crear tu primer repositorio

Crea una carpeta llamada `first_repository`. Entra en ella desde la terminal e inicializa un repositorio Git. Después, explica qué carpeta interna crea Git al ejecutar este proceso y cuál es su función.

---
crea una carpeta llamada .git, es un directorio oculto que se crea automáticamente en la raíz de tu proyecto cuando inicializas un repositorio de Git
El historial de commits, las ramas, la configuración local...

## Ejercicio 5. Primer archivo y estado del repositorio

Dentro del repositorio anterior, crea un archivo llamado `README.md` con una breve descripción del proyecto. Después, comprueba el estado del repositorio con el comando correspondiente y describe qué información te muestra Git.

---
git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

## Ejercicio 6. Añadir y guardar cambios

Añade el archivo `README.md` al área de preparación y realiza un primer commit con un mensaje descriptivo. Después, consulta el historial de commits del repositorio.

---
git add README.md 
git commit -m"commit README.md"
[master (root-commit) 2b9ca29] commit README.md
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

git log
commit 7f49ab40e4c9fac0830299eda2edf50486ad09ef (HEAD -> main, origin/main, origin/HEAD)
Author: buzzfear-creator <buzzfear@gmail.com>
Date:   Tue Jun 2 13:34:39 2026 +0200

    finalizar

commit 2b9ca294af4199b3c937f27df9839bd585b90658
Author: buzzfear-creator <buzzfear@gmail.com>
Date:   Tue Jun 2 13:05:37 2026 +0200

    commit README.md

## Ejercicio 7. Clonar un repositorio

Investiga qué hace el comando `git clone` y explica en qué situaciones se utiliza. Después, escribe un ejemplo realista de uso con una URL de repositorio.

---
trae un repositorio/proyecto desde la web de GitHub
git clone https://github.com/Amaza-ing/my-project.git my-project-2

## Ejercicio 8. GUI de Git

Busca una interfaz gráfica para trabajar con Git, como GitHub Desktop, SourceTree o la integración de Visual Studio Code. Indica cuál has elegido y responde qué ventajas puede tener usar una GUI frente a trabajar solo con comandos en terminal.

---
Mi primera vez, uso la interfaz de Visual Studio Code, no puedo comparar

## Ejercicio 9. GitHub

Crea una cuenta en GitHub, o utiliza una que ya tengas. Después, crea un repositorio remoto llamado `tema1-git`, súbelo a tu perfil y explica qué utilidad tienen plataformas como GitHub en un proyecto de desarrollo.

---
git remote add origin https://github.com/buzzfear-creator/tema1-git.git
git branch -M main
git push -u origin main

Mantiene el control de versiones, ramas y commits de un proyecto para que diferentes personas puedan trabajar a la vez en él

## Ejercicio 10. `git restore file`

Modifica el contenido de un archivo que ya esté siendo controlado por Git, pero sin hacer commit. Después, utiliza `git restore nombre-del-archivo` para deshacer los cambios realizados en ese archivo. Finalmente, comprueba el estado del repositorio y explica qué ha ocurrido.

---
git restore README.md 
Elimina los cambios que he realizado directamente en los archivos

## Ejercicio 11. `git restore --staged file`

Realiza cambios en un archivo y añádelo al área de preparación con `git add`. Después, utiliza `git restore --staged nombre-del-archivo` para sacarlo del área de preparación sin perder los cambios en el directorio de trabajo. Finalmente, ejecuta `git status` y explica la diferencia entre restaurar un archivo normal y restaurarlo desde el área de preparación.

---
git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

## Reto final opcional

Si ya has realizado los ejercicios anteriores, intenta conectar tu repositorio local con un repositorio remoto y subir tu primer commit.

git add .
git commit -m"finalizar"
git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 302 bytes | 302.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/buzzfear-creator/tema1-git.git
   2b9ca29..7f49ab4  main -> main