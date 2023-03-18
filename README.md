# Masteruah

<ol>
<li>creamos una carpeta donde vayamos a hacer git clone con el repositorio masteruah que hemos creado:
git clone</li>
<li>entramos en la carpeta masteruah que hemos creado, le hacemos un add al readme.md y un commit para que se hagan los cambios (no hemos hecho ningun cambio) de prueba:
  cd Masteruah/ <br>
  git add README.md
  git commit -m "commit inicial de prueba"<br></li>
  hacemos un push para subir los cambios:
  git push
<li>ahora creamos un nuevo fichero de texto de prueba lo vamos a añadir y hacerle un commit para que se hagan los cambios en git:<br>
  git add fichero1.txt<br>
  git commit -m "añadir fichero1.txt"</li>
<li>despues de esto vamos a crearle a ese fichero de texto un tag de que versionado tiene (por asi decirlo):<br>
  git tag v0.1</li>
<li>y ahora hacemos un push de los tags con el nombre de la version que le hemos puesto en la anterior actividad:<br>
  git push --tags</li>
<li>seguido de esto vamos a crear una rama a parte de la principal llamada v0.2:<br>
 git branch v0.2<br>
  
  ahora cambiamos a esa rama:<br>
  git checkout v0.2</li>
<li>metemos informacion dentro de un nuevo fichero 2 que vamos a crear en la rama v0.2:<br>
  echo "cosas que tiene este fichero 2" > fichero2.txt</li>
<li>ahora añadimos el fichero 2, le hacemos un commit para comentar la subida y el push para definitivamente subirlo a la red:<br>
  git add fichero2.txt<br>
 git commit -m "añadir fichero 2 a rama v0.2"<br>
  
  aqui hacemos el pusn del origen de la rama v0.2:<br>
  git push -u origin v0.2
</li>
<li>ahora cambiamos a la rama main:<br>
  git checkout main</li>
<li>ahora vamos a fusionar una rama con la otra (mas bien el contenido), estando obviamente desde la rama main:<br>
  git merge v0.2</li>
<li>ahora editamos desde un editor de texto el fichero1.txt, añadiendole algo para hacerle algun cambio, lo añadimos para la subida, hacemos un commit para comentar la modificacion que le hemos hecho:<br>
  git add fichero1.txt<br>
  git commit -m "modificar fichero1.txt con la palabra hola" </li>
<li>despues de eso sin hacer un add y commit cambiamos a la rama 2 y modificamos el fichero 1 haciendole otro add:<br>
  git checkout v0.2<br>
  echo "adios" > fichero1.txt<br>
  git add fichero1.txt <br>
  git commit -m "agregado adiosen fichero1.txt desde la rama v0.2"<br>
  
  ASI CREAMOS UN CONFLICTO 
  </li>
<li>ahora cambiamos a la main y fusionamos de nuevo la v2:<br>
  git checkout main <br>
  git merge v0.2</li>
<li>con estos comandos podemos ver que merges se han hecho y cuales no y su informacion:<br>
  git branch --merge<br>
  git branch --no-merge</li>
  <li>tenemos un error cuando vemos el estado de git el cual vamos a arreglar de esta manera:<br>
  abrimos el fichero1.txt reeditamos y quitamos la parte de adios que añadimos antes:<br>
  nano fichero1.txt (editamos) <br>
  cat fichero1.txt (asi podriamos verificar que se ha cambiado lo que hemos modificado desde nano o vim)</li>
  <li>ahora volvemos a añadir y hacemos un commit del "arreglo":<br>
  git add fichero1.txt <br>
  git commit -m "resuelto conflicto en fichero1.txt"</li>
  <li>ahora en la rama main hacemos un tag de v2 y borramos la rama 2:<br>
    git tag v0.2<br>
    git branch -D v0.2
  </li>
  <li>cambiamos la foto de perfil <br>
  <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/1.png">
  </li>
  <li>le ponemos a la cuenta la verificacion en dos pasos: <br>
    <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/2.png">
  </li>
  <li>tenemos que crear la clave ssh para poder activarlo en nuestro github con las siguientes capturas de estos comandos: <br>
    <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/3.png"> <br>
     <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/4.png"> <br>
     <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/5.png"> <br>
     <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/6.png"> <br>
    <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/7.png"> <br>
  </li>
  <li>nos guardamos en favoritos una publicacion de cualquier compañero:
      <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/8.png"> <br>
   </li>
  <li>seguido de esto vamos a meter una tabla con 3 usuarios dentro del readme.md:
      <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/10.png"> <br>
      <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/11.png"> <br>
  </li>
  <li>en la actividad de los colaboradores vamos a agregar a alvaro como uno:
    <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/12.png"> <br></li>
    <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/13.png"> <br>
    <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/14.png"> <br>
  
  <li>y seguido creamos una organizacion: <br>
    <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/15.png"> <br>
    <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/16.png"> <br></li>
  <li> creamos un equipo admins y otro colabs: <br>
     <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/17.png"> <br>
     <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/18.png"> <br>
     <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/19.png"> <br>
  </li>
  <li>seguido de todos estos pasos vamos a crear un nuevo repositorio sin el readme.md con un nuevo index.md creado por nosotros <br> 
  <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/20.png"> <br>
    
  </li>
  <li>y hacemos los forks para peticiones de edicion a otro usuario, ademas de ver los nuestros: <br>
  <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/21.png"> <br>
      <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/22.png"> <br>
      <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/23.png"> <br>
      <img src="https://github.com/JLFcmd/Masteruah/blob/main/img/24.png"> <br>
  </li>

  
  
</ol>






<table>
<tr>

<td>Nombre</td>
<td>GitHub</td>


</tr>
  <tr>

<td>Cracker</td>
<td>[GitHub](https://github.com/Crackersssss)</td>


</tr>
  <tr>

<td>Forcebrute08</td>
<td>[GitHub](https://github.com/Forcebrute08)</td>


</tr>
  <tr>

<td>KarlPolen</td>
<td>[GitHub](https://github.com/karlpolen)</td>


</tr>


</table>
