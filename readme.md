## Git and GitHub

Este es el repositiorio que hice de un curso profesional de Git y GitHub en Platzi:

- [Curso Profesional de Git y GitHub](https://platzi.com/clases/git-github/).

## Comandos aprendidos


-   `git add .`  Agrega todos los archivos con cambios al área de staging.
    
-   `git commit -m "<this is my message>"` Agrega los cambios del staging al repositorio o **rama master.**
   
    -   `-am` Hace `git add .` y luego `git commit`
-   `git checkout <nameBranch>`
    
-   `git rm --cached <file>` Elimina cambios del staging
    
-   `git log` Historia del repositiorio
    
    -   `--stat` Muestra los bytes agregados o eliminados
    -   `--oneline` Te muestra el id commit y el título del commit.
    -   `--decorate` Te muestra donde se encuentra el head point en el log.
    -   `--stat` - Explica el número de líneas que se cambiaron brevemente.
    -   `-p` Explica el número de líneas que se cambiaron y te muestra que se cambió en el contenido.
    -   `git shortlog` - Indica que commits ha realizado un usuario, mostrando el usuario y el titulo de sus commits.
    -   `--graph` Muestra en diagrama de árbol
    -   `--pretty=format:"%cn hizo un commit %h el dia %cd"` - Muestra mensajes personalizados de los commits.
    -   `-3` Limitamos el número de commits.
    -   `--after=“2018-1-2”`
    -   `--after=“today”`
    -   `--after=“2018-1-2” --before=“today”` - Commits para localizar por fechas.
    -   `--author=“Name Author”` - Commits realizados por autor que cumplan exactamente con el nombre.
    -   `--grep=“INVIE”` - Busca los commits que cumplan tal cual está escrito entre las comillas.
    -   `-grep=“INVIE” –i` Busca los commits que cumplan sin importar mayúsculas o minúsculas.
    -   `– index.html` Busca los commits en un archivo en específico.
    -   `-S “Por contenido”` Buscar los commits con el contenido dentro del archivo.
    -   `> log.txt` - guardar los logs en un archivo txt
-   `git show` muestra los cambios que se han hecho
    
-   `git diff` Compara los cambias entre el _staging_ y el directorio actual
    
    -   `<idcommit> <idanothercommit>` Compara los cambias entre dos commits
-   `git reset` Se devuelve en el tiempo por los commits sin posibilidad de volver al futuro
    
    -   `--hard` Todo vuelve al estado anterior.
    -   `--soft` Todo lo que está en _staging_ sigue ahí.
    -   `HEAD` saca archivos del área de Staging
-   `git checkout <idcommit>` Muestra un commit en especial.
    
-   `git rm`
    
-   `git push` Envía el _Repositorio Local_ a un _Repositorio Remoto_
    
-   `git fetch` Trae los datos del _Repositorio Remoto_ al _Repositorio Local_
    
-   `git merge` Toma los archivos del _Repositorio Local_ (enviados allí por _fetch_) al _Working Directory_
    
    -   El HEAD debe estar en la rama diferente que quiero traer. (En master)
    -   Un merge es un COMMIT
-   `git pull` Hace `git fetch` y luego `git merge`
    
-   `git branch <nameBranch>` Crea una rama nueva justo donde está el HEAD.
    
-   `git remote add origin <urlproyectgit>`
    
    -   Podemos añadir un remote de un proyecto original en caso de haber hecho fork a un proyecto. `git remote add <upstream|nameorigin> <urlgit.git>`
    -   `--allow-unrelated-histories` Forza el pull
    -   `git remote rm destination` Elimina el remote
-   `git push origin master` Lleva los cambios de _MASTER_ al _Repositorio Remoto_
    
-   `git tag`
    
    -   `git tag -a <nametag> -m "message" <idcommit>` Crear TAGS
    -   `git tag <nametag> -d` Elimina un TAG
    -   `git push origin :refs/tags/<nametag>` Eliminar el tag del origin
    -   `git push origin —tags` Enviar los tags al origin
-   `git show-branch --all` Muestra la historia de cada branch
    
-   `gitk`


## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).