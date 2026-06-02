# Ejercicios - Tema 2: Ramas

A continuación, encontrarás 10 ejercicios prácticos sobre ramas en Git, fusión de ramas, resolución de conflictos y tipos de ramas. Intenta resolverlos antes de consultar la teoría.

---

## Ejercicio 1. Crear y listar ramas

Crea un repositorio nuevo llamado `tema2-ramas` y realiza un primer commit con un archivo `README.md`. Después, crea dos ramas nuevas llamadas `feature/header` y `feature/footer`. Por último, ejecuta el comando necesario para mostrar todas las ramas disponibles e indica cuál es la rama activa.

---
git branch 
* feature/footer
  feature/header
  master

## Ejercicio 2. Cambiar entre ramas

Sitúate en la rama `feature/header` y crea un archivo llamado `header.html` con una estructura básica. Haz un commit con un mensaje descriptivo. Después, cambia a la rama `feature/footer` y comprueba si el archivo `header.html` existe también en esa rama. Explica por qué ocurre ese comportamiento.

---
git checkout feature/header
Switched to branch 'feature/header'
git commit -m"new header.html"
git checkout feature/footer
No existe el archivo, ya que en esta rama no está creado ni salvado en la main

## Ejercicio 3. Fusión de una rama sin conflicto

En la rama `feature/footer`, crea un archivo llamado `footer.html` y guarda los cambios con un commit. Después, vuelve a la rama principal y fusiona `feature/footer`. Comprueba el historial de commits y explica qué ha ocurrido tras hacer el merge.

---
git add footer.html
git commit -m"first footer.html"
[feature/footer 0273fba] first footer.html
 1 file changed, 6 insertions(+)
 create mode 100644 footer.html

git checkout master 



## Ejercicio 4. Provocar un conflicto sencillo

Crea una rama nueva llamada `feature/title`. Modifica en esa rama una misma línea del archivo `README.md`, por ejemplo el título principal, y haz un commit. Después, vuelve a la rama principal, modifica exactamente esa misma línea con un contenido diferente y haz otro commit. Intenta fusionar `feature/title` en la rama principal y observa qué mensaje muestra Git.

---

## Ejercicio 5. Identificar archivos en conflicto

Explica con tus palabras por qué se ha producido el conflicto.

---

## Ejercicio 6. Resolver un conflicto manualmente

Abre el archivo en conflicto y localiza las marcas `<<<<<<<`, `=======` y `>>>>>>>`. Resuelve el conflicto manualmente dejando una única versión final coherente del contenido. Después, añade el archivo al área de preparación y completa el proceso de fusión con el commit correspondiente.

---

## Ejercicio 7. Conflicto con varias líneas

Crea una nueva rama llamada `feature/about` y añade una pequeña sección de presentación en un archivo `about.md`. Después, desde la rama principal, modifica también esa misma sección pero con un texto distinto. Intenta fusionar ambas ramas y resuelve el conflicto combinando parte del contenido de las dos versiones en lugar de quedarte solo con una.

---

## Ejercicio 8. Resolver un conflicto en VSCode o en GitHub

Provoca de nuevo un conflicto entre dos ramas modificando la misma línea de un archivo. Si antes resolviste los conflictos usando VSCode trata de resolverlo diréctamente en GitHub o viceversa.

---

## Ejercicio 9. Tipos de ramas

Investiga brevemente para qué se suelen utilizar ramas de tipo `feature`, `bugfix`, `hotfix` y `release`. Después, propón un ejemplo de nombre válido para cada una dentro de un proyecto web.

---

## Ejercicio 10. Caso práctico completo

Imagina que estás trabajando en equipo y dos personas han editado la misma parte del archivo `index.html`: una ha cambiado el texto del encabezado y otra ha cambiado ese mismo texto en otra rama distinta. Describe paso a paso cómo resolverías el conflicto, indicando qué comandos usarías desde el momento en que Git detecta el conflicto hasta que la fusión queda completada.

---

## Reto final opcional

Crea un pequeño proyecto con una rama principal y al menos dos ramas secundarias. Haz cambios distintos en varios archivos, provoca al menos un conflicto real al fusionarlas y resuélvelo manualmente. Después, revisa el historial de commits y explica qué estrategia has seguido para dejar una versión final correcta del proyecto.
