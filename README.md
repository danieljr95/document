<a name="readme-top"></a>
<h1>                </h1>

<div align="center">            </div>

<img src="cat.jpg" alt="cat" width="500" height="350"> </img> 
<br>
<h2>Proyecto de GitHub</h2>

# Tabla de contenidos
[⚙️ Configuración](Ajustes)

[📱Acerca de nosotros]()

[📥Instalación]()

[👇Uso]()

[👨‍🔧Soporte técnico]()

# [Proyecto de GitHub] <a name="Acerca del proyecto" > </a>

**[Proyecto de GitHub]** Es el primer proyecto del SENA, como gestión de redes de datos

## 🔨 Construido con <a name="built-with"></a>
<p>
Este proyecto se hizo usando:
HTML, Markdown, Shellscript, Git, GitHub </p>

### Herramientas <a name="Herramientas"></a>

<li>HTML</li>
<li>Markdown</li>
<li>Shellscript</li>
<li>Git</li>
<li>GitHub</li>


<details>
<summary> Client </summary>
    <ul>
    <li><a href="https://developer.mozilla.org/es/docs/Web/HTML">HTML</a></li>    
    </ul>
</details>

<details>
<summary>Markdown</summary>
<ul>
<li><a href="https://markdown.es/sintaxis-markdown/">Markdown</a></li>
</ul>
</details>

### Configuracion
Creando un Directorio con Git Bash 

```sh
comando: mkdir + nombre_directorio
```
Listar para confirmar la creación del directorio 

```sh
comando: ls
```

Para ingresar al directorio creado 
```sh
comando: cd + nombre_directorio
```

Para clonar nuestro repositorio:

```sh

Comando: git clone https://github.com/danieljr95/net.git

Para ingresar:
Comando: cd net
```

Crear un archivo en shell ejemplo.sh

```sh
Comando: touch + Nombre.sh 
```

### Ejecutando el archivo:

 Para ejecutar el archivo, usamos el ./nombre_archivo.sh

```sh
Comando: ./net.sh
```

### Creación de usuarios para vincular al GitHub

Creación de usuario local:

```sh
Comando: git config --global user.name +  Nombre 
```

Creación de correo local: 

```sh
Comando: git config --global user.email + Nombre 
```
ver la creacion de usuario y correo electrónico:

```sh
Comando: git log
```

solicitar una llave publica de ssh en git bash para vincular a la cuenta de GitHub:

```sh
Comando: ssh-keygen
```
Después de generar la clave, nos muestra us script en el cual nos indica el directorio donde se guardó la llave pública:

```sh
Comando: cat /c/users/usuario/.ssh/id_ed25519.pub
```
Posterior a esto, nos dirigimos a la página de GitHub en donde hay una opción para agregar una llave pública, y la vinculamos con nuestra cuenta.

Establecer conexion con el perfil de GitHub

```sh
Comando: git remote add origin + direccion del repositorio http o ssh
```
Para ver la dirección copiada
```sh
Comando: git remote -v
```

### Comandos para subir el archivo del git bash al repositorio de GitHub

Para ver en donde se encuentra el archivo: 

```sh
Comando: git status  
```
Para subir el script al stage
```sh
Comando: git add script.sh  
```
Enviar el script a directorio local, indicando lo que agregamos con el commit: 

```sh
Comando: git commit -m  "mensaje"  
```

Ver los archivos del repositorio local, con las modificaciones:

```sh
Comando: git log --oneline 
```

Para subirlo al repositorio de GitHub vinculado

```sh
Comando: git push -u script.sh 
```
Si nos muestra un mensaje de error, podemos usar el -f para subirlo forzado 

```sh
Comando: git push -f script.sh  
```
### Comando para regresar el repositorio local, al area de trabajo

```sh
Comando: git reset --maxed head~1  
```
Mostrar los archivos que están listo para enviar a repositorio local:

```sh
Comando: git ls-files 
```

Restaurar el script de la zona stage, al repositorio de trabajo:

```sh
Comando: git restore --stage  script.sh
```
Para ver que podemos borrar:

```sh
Comando: git clean -n
```

Borrar todos los comandos realizados:

```sh
Comando: git clean -f
```

Borrar lo más reciente del contenido del script:

```sh
Comando: git reset --hard HEAD~1
```

Mostar que parametros contiene el archivo

```sh
Comando: git diff --staged script.sh
```

### Creación de branch (ramas)

Creación de una rama

```sh
Comando: git checkout -b + nombre_rama  
```
Ver las branch creadas:

```sh
Comando: git branch
```

Cambiar de branch

```sh
Comando: git checkout + nombre_de_la_rama
```

### Subir el script en el branch

Subir el script creado para subirlo al repositorio:

```sh
Comando: git push -u origin + nombre de la rama 
```

### Fusionar las ramas

Para fusionar la información de una rama anterior, con una nueva:

```sh
Comando: git merge + nombre_rama
```

### Comandos tag

Crear un tag para los archivos:

```sh
Comando: git tag + Nombre 
example: git tag v2.0
```

Para subir los tags al repositorio:
```sh
Comando: git push -u origin nombre_rama --tags
```


Ver los tag realizados

```sh
Comando: git tag
```
## Comandos adicionales

Para copiar todos el repositorio local 

```sh
Comando: git fetch + nombre del repositorio
```

Envía todos los archivos que esta en directorio de trabajo a stage area: 

```sh
Comando: git add .
```
Restauración del proyecto en un punto anterior

```sh
Comando: git restore + nombre del archivo 
```

Deshacer el último comentario, manteniendo los cambios en el área de preparación 

```sh
Comando: git reset --soft HEAD~1
```

Deshace los cambios introducidos, por el commit con el hash abc123 que se ven en git log

```sh
Comando: git revert + code hash
```
Resetear el archivo con un hash específico 
```sh
Comando: git reset --hard + code hash
```


### Configuración

Para clonar este repositorio:

```sh
cd 
git clone https://github.com/danieljr95/document.git

Ingresamos al directorio que nos genera el git clone con cd nombre_directorio
```
### Para ejeucurarlo, usamos

```sh
    ./README.md
```

### Comandos creados en shell para Windows

Para correr los comandos, podemos descargar el archivo del repositorio y ejecutarlo en git bash con un ./ :

git clone https://github.com/danieljr95/net.git

O puede copiar y pegar lo siguente:

```sh
#!/bin/bash

# Para pedir una IP
echo "Pedir al usuario una dirección IP"
read -p "Introduce una dirección IP " ip_address

# Mostrar IP ingresada

echo "La dirección IP ingresada es: $ip_address"

# Info del sistema
echo "Info del sistema:"
systeminfo

# Mostrar lista de procesos en ejeucion
echo "Lista de procesos:"
tasklist 
```


<p align="right"><a href="#readme-top">Back to top</a></p>



## 📃 Creación de actividad 1 <a name="license"></a>

Creamos la rama develop con: git checkout -b develop

A continuación, creamos una rama llamada featue-1 y añadimos una clase A con atributos: foo bar.

Para mejor orden, creamos un archivo nuevo llamado a.js, lo añadimos con git add a.js, comentamos los cambios realizados en el documento con git commit -m "Añadida clase A con atributos foo, bar, y javascript"
y lo subimos con git push feature-1

Creamos un archivo a.js, indicando que es para Javascript:
![alt text](image.png)

Repetimos las acciones anteriores, con git add, git commit y git push.

![alt text](image-1.png)

Posteriormente lo mergeamos con la rama develop, y un push para subir los cambios.

![alt text](image-2.png)

A continuación mergeamos la rama develop con Main, y generamos una etiqueta llamada v1.0:

![alt text](image-3.png)

Etiqueta y push, especificando al final los tags para subirlos:

![alt text](image-4.png)

Creamos la rama feature-2 y añadimos la clase B, que es un archivo similar al A, solo cambiando los valores del foo y creando un b.js:

![alt text](image-5.png)

Creación:

![alt text](image-6.png)

Nuevamente creamos otra rama nombrada feature-3, y añadimos una clase C:

![alt text](image-7.png)

Archivo c.js

![alt text](image-8.png)

Mergeamos featute-2 y feature-3 con develop:

![alt text](image-9.png)

Mergeamos develop con main y creamos una nueva etiqueta v2.0:

![alt text](image-10.png)

Creación de rama hotfix-1 a partir de main y añadir un atributo lorem en clase A:

![alt text](image-11.png)

Mergear rama hotfix-1 con main y creación de etiqueta v2.1:

![alt text](image-12.png)

Tag:

![alt text](image-13.png)


<p align="right"><a href="#readme-top">Back to top</a></p>

## 👥 Autores <a name="autores"></a>

Daniel Jara

🧑🏻‍💻 **Autor 1**

 - GitHub: [@danieljr95](https://github.com/danieljr95)

🧑🏻‍💻 **Plantilla tomada de:**

Jeysson Contreras (Instructor SENA)
- GitHub: [@alyconr](https://github.com/alyconr)


## 🤝 Contribuciones <a name="Contribuciones"></a>

Cualquier tipo de sugerencia, comentario, etc son bienvenidos!

Para consultar la página: [Página](https://github.com/danieljr95/document/tree/main)


## ⭐ Muestra tu apoyo

Si te gustó este proyecto, no dudes en comentarlo


## 👏 Agradecimientos <a name="Agradecimientos"></a>

Agradezco al instructor Jeysson Contreras, a mis compañeros del SENA, que me apoyan y me resuelven mís dudas en este proceso de aprendizaje. Especialmente a Daniel Escobar y su página de GitHub [@bulcano720](https://github.com/bulcano720), que me apoya en mis inquietudes.

## 📃 License <a name="license"></a>

This Project is [MIT](./LICENSE.md) licensed

<p align="right"><a href="#readme-top">Back to top</a></p>