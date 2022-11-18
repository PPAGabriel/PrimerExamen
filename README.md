# examenDAM
Para utilizarlo en el examen

## Primera modificación hecha por Gabriel Pérez :smile:

**Explicación del primer apartado:**

*Para este punto, se creó una carpeta con el comando "mkdir Examen1COD"* ubicado en la direccion de mis Documentos. Simultaneamente se creó un repositorio privado en GitHub (el presente), y para clonar el referente al examen se usó el comando "*git clone: URL*".
Luego, se eliminó el origin anterior con *"git remote rm origin" del repositorio clonado y conecta con el propio con los siguientes comandos:*

###### git remote add origin (URL del propio) -> git add README.md (en este punto se habia modificado el README con el comando "touch "contenido" >> archivo") -> git commit: -m "descripción del commit" -> git branch -M main ->  git -u push origin main. 

**Explicación del segundo apartado:**

*Para añadir un programa existente (en este caso Boletin 8) y lo copie a la carpeta destino, y a partir de allí sólo añadí la carpeta src que es la que contiene los archivo java. Antes de realizar el commit para cambiar el nombre del usuario apliqué el siguiente comando:*

###### git config --global user.name "Nuevo nombre"

**Explicación del diagrama**

*El diagrama recopila por medio de un switch las posibles respuestas del usuario*

```mermaid
graph TD;
    I-->mostrarMenu;
    mostrarMenu-->introducirOpcion;
    introducirOpcion-->B{switch};
    B--=1-->introducirLado;
    B--=2-->introducirb,h;
    B--=3-->introducirR;
    B--=default-->opcionIncorrecta;
    introducirLado-->sup=l*l;
    sup=l*l-->VisualizarSup;
    VisualizarSup-->Fin
    introducirB,H-->sup=b*h/2;
    sup=b*h/2-->VisualizrSup;
    VisualizrSup-->Fin;
    introducirR-->sup=PI*r2;
    sup=PI*r2-->VisualizaSup;
    VisualizaSup-->Fin;
    opcionIncorrecta-->Fin;