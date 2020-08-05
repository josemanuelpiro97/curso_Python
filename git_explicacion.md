# GIT

--- 

## GIT de manera "local" vs "la nube"

Es de crucial imprtancia entender la diferencia que hay entre el repositorio del cual disponemos en la **nube** ("github") y el repositorio que tenemos de manera **local**, estos dos pueden funcionar de manera perfecta **separados**, pero tambien **podemos complementarlos**.

Ya sea que utilicemos el repositorio de manera **local** o en la **nube**, tendremos a disposicion el conjunto de erramientas de **configuration managment**, la ventaja esta en complementar el uso local y de la nube para obtener un mayor alcance de trabajo.

Si desean tener un conocimient mucho mas profundo sobre esta herramienta, se recomienda la bibliografia **"Pro GIT segunda edicion"** <https://progit2.s3.amazonaws.com/es/2015-03-10-11982/progit-es.388.pdf>

### GIT en la nube

Podemos hacer uso de las herramientas de git en alguno de sus formatos "nube". Para esto hay varias empresas que ponen a nuestra disposicion este tipo de herramientas, tales como:

- **github** <https://github.com/>
- **gitlab** <https://about.gitlab.com/>
- **bitbucket** <https://bitbucket.org/product/>

Para entender un poco mejor el alcance de esta tecnologia, ver el siguiente video <https://youtu.be/w3jLJU7DT5E>

### GIT local

Por otro lado esta el uso de **repositorios locales**, en este caso dispondremos de las **mismas herramientas** que en las propuestas por las empresas nombradas en el item anterior, solo que **no podremos compartirlo con nadie**, es decir, todo el registro que llevemos de nuestro codigo estara a disposicon de nosotros y nadie mas. Es por esto que a fines del curso **buscaremos intengrar ambas modalidades** para poder **compartir los progresos individuales** entre nosotros y en el camino entender los fundamentos de la herramienta.

---

## Puesta en marcha

En este curso, el repositorio **ya esta en la nube**, es por eso que deberemos clonarlo de manera local en nuestro espacio de trabajo, eso o haremos de la siguiente manera

    git clone [linck_del_repositoro]

Una ves que el repositoro esta de manera local, podremos encontrarlo como una careta en nuestro sistema.

- Es importante entender que el echo de que tengamos ahora el repositorio de manera local, **no nos asegura que los cambios realizados en uno u otro esten linckeados de manera constante**, esto tendremos que ir **"haciendolo a mano"**, *de igual manera que tener un libro en nuestra biblioteca no nos asegura que al salir la nueva version del libro las paginas del que tenemos en la biblioteca cambien, deberemos ser nosotros quienes salgan a comprar el nuevo libro*.

## Subiendo cambios del repostorio local a la nube

A continucacion explicare **4 comandos** muy importantes para el trabajo con repositorios, estos son **git status**, **git add**, **git commit** y **git push**

### status

Este comando nsos permitira saber el estado actual del repositorio. este se vera modificado cada ves que agregue o quite un archivo, o cuando solamente lo modfique.

Pr ejemplo, al agregar un achivo nevo al repositorio, o al modificar algun archivo existente nos mostrara algo como esto:




