# Masteruah

<ol>
<li>creamos una carpeta donde vayamos a hacer git clone con el repositorio masteruah que hemos creado:
git clone</li>
<li>entramos en la carpeta masteruah que hemos creado, le hacemos un add al readme.md y un commit para que se hagan los cambios (no hemos hecho ningun cambio) de prueba:
  cd Masteruah/
  git add README.md
  git commit -m "commit inicial de prueba"</li>
  hacemos un push para subir los cambios:
  git push
<li>ahora creamos un nuevo fichero de texto de prueba lo vamos a añadir y hacerle un commit para que se hagan los cambios en git:
  git add fichero1.txt
  git commit -m "añadir fichero1.txt"</li>
<li>despues de esto vamos a crearle a ese fichero de texto un tag de que versionado tiene (por asi decirlo):
  git tag v0.1</li>
<li>y ahora hacemos un push de los tags con el nombre de la version que le hemos puesto en la anterior actividad:
  git push --tags</li>
<li>seguido de esto vamos a crear una rama a parte de la principal llamada v0.2:
 git branch v0.2
  
  ahora cambiamos a esa rama:
  git checkout v0.2</li>
<li>metemos informacion dentro de un nuevo fichero 2 que vamos a crear en la rama v0.2:
  echo "cosas que tiene este fichero 2" > fichero2.txt</li>
<li>ahora añadimos el fichero 2, le hacemos un commit para comentar la subida y el push para definitivamente subirlo a la red:
  git add fichero2.txt
 git commit -m "añadir fichero 2 a rama v0.2"
  
  aqui hacemos el pusn del origen de la rama v0.2:
  git push -u origin v0.2
</li>
<li>ahora cambiamos a la rama main:
  git checkout main</li>
<li>ahora vamos a fusionar una rama con la otra (mas bien el contenido), estando obviamente desde la rama main:
  git merge v0.2</li>
<li>ahora editamos desde un editor de texto el fichero1.txt, añadiendole algo para hacerle algun cambio, lo añadimos para la subida, hacemos un commit para comentar la modificacion que le hemos hecho:
  git add fichero1.txt
  git commit -m "modificar fichero1.txt con la palabra hola" </li>
<li>despues de eso sin hacer un add y commit cambiamos a la rama 2 y modificamos el fichero 1 haciendole otro add:
  git checkout v0.2
  echo "adios" > fichero1.txt
  git add fichero1.txt 
  git commit -m "agregado adiosen fichero1.txt desde la rama v0.2"
  
  ASI CREAMOS UN CONFLICTO 
  </li>
<li>ahora cambiamos a la main y fusionamos de nuevo la v2:
  git checkout main 
  git merge v0.2</li>
<li>con estos comandos podemos ver que merges se han hecho y cuales no y su informacion:
  git branch --merge
  git branch --no-merge</li>
  <li>tenemos un error cuando vemos el estado de git el cual vamos a arreglar de esta manera:
  abrimos el fichero1.txt reeditamos y quitamos la parte de adios que añadimos antes:
  nano fichero1.txt (editamos) 
  cat fichero1.txt (asi podriamos verificar que se ha cambiado lo que hemos modificado desde nano o vim)</li>
  <li>ahora volvemos a añadir y hacemos un commit del "arreglo":
  git add fichero1.txt 
  git commit -m "resuelto conflicto en fichero1.txt"</li>
  <li>ahora en la rama main hacemos un tag de v2 y borramos la rama 2:
    git tag v0.2
    git branch -D v0.2
  </li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  
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
