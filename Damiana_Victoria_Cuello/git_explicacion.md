# ![foo](/images/git.png "title")

---

## GIT de manera "local" vs "la nube"

Es de crucial importancia entender la diferencia que hay entre el repositorio del cual disponemos en la **nube** ("github") y el repositorio que tenemos de manera **local**, estos dos pueden funcionar de manera perfecta **separados**, pero también **podemos complementarlos**.

Ya sea que utilicemos el repositorio de manera **local** o en la **nube**, tendremos a disposición el conjunto de herramientas de **configuration managment**, la ventaja está en complementar el uso local y de la nube para obtener un mayor alcance de trabajo.

Si desean tener un conocimiento mucho más profundo sobre esta herramienta, se recomienda la bibliografía **"Pro GIT segunda edición"** <https://progit2.s3.amazonaws.com/es/2015-03-10-11982/progit-es.388.pdf>

### GIT en la nube

Podemos hacer uso de las herramientas de git en alguno de sus formatos "nube". Para esto hay varias empresas que ponen a nuestra disposición este tipo de herramientas, tales como:

- **github** <https://github.com/>
- **gitlab** <https://about.gitlab.com/>
- **bitbucket** <https://bitbucket.org/product/>

Para entender un poco mejor el alcance de esta tecnología, ver el siguiente video <https://youtu.be/w3jLJU7DT5E>

### GIT local

Por otro lado está el uso de **repositorios locales**, en este caso dispondremos de las **mismas herramientas** que en las propuestas por las empresas nombradas en el ítem anterior, solo que **no podremos compartirlo con nadie**, es decir, todo el registro que llevemos de nuestro código estará a disposición de nosotros y nadie más. Es por esto que a fines del curso **buscaremos integrar ambas modalidades** para poder **compartir los progresos individuales** entre nosotros y en el camino entender los fundamentos de la herramienta.

---

## Puesta en marcha

En este curso, el repositorio **ya está en la nube**, es por eso que deberemos clonarlo de manera local en nuestro espacio de trabajo, eso o haremos de la siguiente manera

    git clone [linck_del_repositoro]

Una ves que el repositorio esta de manera local, podremos encontrarlo como una careta en nuestro sistema.

- Es importante entender que el hecho de que tengamos ahora el repositorio de manera local, **no nos asegura que los cambios realizados en uno u otro estén linckeados de manera constante**, esto tendremos que ir **"haciéndolo a mano"**, *de igual manera que tener un libro en nuestra biblioteca no nos asegura que al salir la nueva versión del libro las páginas del que tenemos en la biblioteca cambien, deberemos ser nosotros quienes salgan a comprar el nuevo libro*.

## Subiendo cambios del repositorio local a la nube

A continuación explicaré **4 comandos** muy importantes para el trabajo con repositorios, estos son **git status**, **git add**, **git commit** y **git push**.

### status

Este comando nos permitirá **saber el estado actual del repositorio**. Este se verá modificado cada vez que **agregue o quite un archivo, o** cuando solamente **lo modifique**.

Por ejemplo, al agregar un archivo nevo al repositorio, o al modificar algún archivo existente nos mostrará algo como esto:

![foo](/images/git_status.png "title")

Aquí podemos ver que **git nos indica que no le está haciendo el trackeo a la nueva modificación**, es por esto que si queremos hacer el cambio efectivo, deberemos usar el **comando add**.

## add

Como vimos en el punto anterior, una ves que se realiza una modificación al estado anterior del repositorio, **este cambio deberá hacerse efectivo mediante el comando add**

    git add [ruta/al/archivo]

Luego de trackear el cambio obtendremos una salida como la siguiente

![foo](/images/gitadd.png "title")

Podemos ver como ahora **git nos indica que ya estamos trackeando los nuevos cambios**, y que lo que **resta es hacer un commit** (*etiquetar el nuevo estado*).

- En caso de querer revertir este trackeo, para no hacer efectivo ningún cambio, git nos indica que con **git restore --staged [ruta/al/archivo]** podemos hacerlo.

## commit

Una ves que ya hemos trackeado todos los cambios que queremos que pertenezcan al nuevo commit, solo resta ejecutar el comando para hacerlo efectivo

    git commit -m "mensaje representativo del nuevo estado"

- podemos ver que en este comando aparece **algo no utilizado anteriormente** (**-m**), esto es un **"parámetro"** que le pasamos al comando **git commmit** para que tenga un comportamiento en particular. En este caso **dicho parámetro** indica que el **mensaje especificado** a continuación sea la **descripción del commit**. Es importante destacar esto, ya que a lo largo del curso y en un futuro como programadores, se encontraran con comandos que necesitaran de parámetros específicos para obtener el comportamiento deseado.

![foo](/images/git-commit.png "title")

Luego de realizado el commit se nos imprimirá un mensaje indicando en primer lugar el id del commit y su nombre referencial. Luego nos indica los detalles del commit.

## push

Ahora que el nuevo commit ya está hecho, podemos decir que tenemos de **manera local** un registro de, hasta ahora, 2 estados (el primero es el repositorio recién clonado, el segundo es el de las modificaciones echas). Solo **nos resta "empujar"** este nuevo commit al **repositorio en la nube**.

    git push

Luego de ejecutar el comando, se **nos pedirá ingresar nuestro usuario y contraseña** de github  (o el repositorio online con el que estemos trabajando) para verificar la validez del push.

![foo](/images/git-push.png "title")

- en la imagen podemos ver como se nos brinda un detalle sobre el push que sé ah realizado. Para los fines de este curso no es necesario conocer a profundidad estos detalles.

## Obteniendo los cambios realzados por otros

Hasta ahora hemos visto la manera de subir nuestros cambios al repositorio en la nube, pero **que sucede cuando otra persona realiza cambios en la nube?**, como hacemos para **tener el último estado del repositorio en la nube de manera local?**... El comando para eso es **"pull"**, este comando actualizará nuestro repositorio local.

    git pull

- Debemos tener en cuenta que al traer de manera local el estado actual de la nube, **podemos encontrarnos con que alguien ah modificado lo mismo que estoy modificando yo**, en estos casos se **generaran conflictos** que **deberemos resolver**. Es por eso que en este curso cada integrante dispone de su carpeta personal para no adentrarnos en esos problemas.

---

## Coandos utiles en BASH

- **pwd**(*print worknig directory*): nos indica la ruta en la que estamos posicionados

        $ pwd
        tu/directorio/actual

- **ls**(*list*): lista los archivos y directorios en la ubicación actual

        $ ls
        archivo1.txt
        archivo2.txt
        directorio-1
        directorio-2

- **cd**(*change directory*): nos permite movernos entre los distintos directorios

        cd ruta/a/la/que/quiero/ir

- **mkdir**(*make directory*): nos permite crear un directorio nuevo

        mkdir nombre-del-directorio

---
---
**Autor:** *Jose Manuel piro*

**Todas las imágenes utilizadas en este documento son solo a fines educativos.**

