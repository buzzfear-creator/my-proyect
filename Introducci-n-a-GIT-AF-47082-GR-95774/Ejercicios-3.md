# Ejercicios - Tema 3: Colaboración en Repositorios

A continuación, encontrarás 10 ejercicios prácticos sobre colaboración en repositorios Git. Intenta resolverlos antes de consultar la teoría.

---

## Ejercicio 1. Pull vs Fetch

Explica con tus palabras qué diferencia existe entre `git pull` y `git fetch`. Después, responde en qué situación usarías cada uno y qué ventaja tiene revisar los cambios antes de integrarlos en tu rama local.

---

## Ejercicio 2. Actualizar un repositorio remoto

Clona un repositorio de prueba o utiliza uno que ya tengas. Después, ejecuta el comando necesario para traer los cambios del repositorio remoto sin fusionarlos automáticamente. A continuación, consulta el estado del repositorio y el historial para comprobar qué información nueva ha llegado.

---

## Ejercicio 3. Git Stash

Realiza cambios en uno o varios archivos de tu repositorio sin hacer commit. Después, guarda temporalmente esos cambios con `git stash`. Comprueba que el directorio de trabajo queda limpio y, a continuación, recupera los cambios guardados. Explica para qué puede resultar útil esta herramienta en un entorno colaborativo.

---

## Ejercicio 4. Rebase

Crea una rama nueva a partir de `master`, realiza al menos un commit en ella y después actualiza esa rama utilizando `git rebase` sobre `master`. Explica qué hace exactamente este comando y qué diferencia principal existe entre usar `merge` y usar `rebase`.

---

## Ejercicio 5. Git Fork

Investiga qué es un fork en plataformas como GitHub. Después, explica con tus palabras en qué se diferencia un fork de clonar un repositorio. Por último, describe una situación realista en la que un desarrollador preferiría hacer un fork antes que trabajar directamente como colaborador en el repositorio original.

---

## Ejercicio 6. Repositorios públicos vs privados

Explica qué diferencia existe entre un repositorio público y uno privado. Después, responde qué ventajas e inconvenientes puede tener cada tipo en un proyecto real. Intenta incluir al menos un ejemplo en el que elegirías un repositorio público y otro en el que optarías por uno privado.

---

## Ejercicio 7. Colaboradores

Crea un repositorio remoto en GitHub o imagina uno ya existente. Después, investiga cómo se añade un colaborador a un repositorio. Explica qué permisos puede tener esa persona dentro del proyecto y por qué es importante gestionar correctamente el acceso cuando varias personas trabajan sobre el mismo código.

---

## Ejercicio 8. Resolver un conflicto entre colaboradores

Imagina que dos colaboradores están trabajando sobre el mismo repositorio y ambos modifican la misma línea de un archivo llamado app.js.

El primer colaborador cambia el contenido de una función en su rama y sube los cambios al repositorio remoto. Mientras tanto, el segundo colaborador, desde otra rama o desde su copia local desactualizada, modifica esa misma línea de forma diferente e intenta integrar sus cambios después.

Reproduce esta situación en un repositorio de prueba. Después, provoca el conflicto al intentar hacer pull, merge o rebase, según el caso. Abre el archivo en conflicto, identifica las marcas que añade Git y resuélvelo manualmente dejando la versión final correcta. Finalmente, añade el archivo, completa el proceso y realiza el commit correspondiente.

Explica qué ha ocurrido, qué partes del archivo estaban en conflicto y qué pasos has seguido para resolverlo correctamente sin perder el trabajo de ninguno de los colaboradores.

---

## Ejercicio 9. Forzar subida

Investiga qué hace el comando `git push --force`. Después, explica por qué puede ser peligroso en un repositorio compartido. Finalmente, responde en qué situaciones muy concretas podría utilizarse y qué alternativa más segura existe para evitar sobrescribir el trabajo de otros compañeros.

---

## Ejercicio 10. Borrar un repositorio

Investiga cómo se puede eliminar un repositorio en una plataforma como GitHub. Después, explica qué consecuencias tiene esta acción y qué precauciones tomarías antes de borrar un repositorio remoto en el que ha trabajado más de una persona.

---

## Reto final opcional

Imagina que estás colaborando en un proyecto con otras personas. Describe un flujo de trabajo posible en el que intervengan `fetch`, `stash`, `rebase`, un repositorio remoto y una subida de cambios. Intenta explicar en qué orden realizarías cada paso y por qué.
