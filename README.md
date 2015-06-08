# jOSuMO
jOSuMO is a JOSM based editor for SUMO simulation networks.

JOSM and its plugins installation
 
 
1. Descargar “josm-tested.jar” https://drive.google.com/open?id=0B-M_ACFUaG35Nk54N0lRRE5BLVU&authuser=0
2. Descargar y ejecutar “run-josm.bat” https://drive.google.com/open?id=0B-M_ACFUaG35YVBJZExYem1RYzg&authuser=0
3. Descargar “sumoconvert.jar” 
https://drive.google.com/open?id=0B-M_ACFUaG35em00YndUV1lFWWM&authuser=0y copiar en la carpeta de plugins de JOSM, 
C:\Users\<user>\AppData\Roaming\JOSM\plugins
https://drive.google.com/open?id=0B-M_ACFUaG35em00YndUV1lFWWM&authuser=0
4. Descargar “turnrestrictions.jar” https://drive.google.com/open?id=0B-M_ACFUaG35cTVUSk90b2I2SzQ&authuser=0  y copiar en la carpeta de plugins de JOSM, C:\Users\<user>\AppData\Roaming\JOSM\plugins
5. Dentro del editor, ir a “Editar->Preferencias…”. Seleccionar el icono de Configuración de Complementos sobre la barra lateral izquierda
  5.1. buscar el plugin “sumoconvert” y marcar el checkbox para incluirlo.
  5.2. buscar el plugin “turnrestrictions” y marcar el checkbox para incluirlo.
  Aceptar y reiniciar JOSM. Si todo es correcto, en el menú se verá la opción Sumo.
	 
6. Habilitar los paneles para el manejo de semáforos, restricciones de giro y distritos, seleccionándolos de la barra lateral sobre la izquiera del editor.

 
 
 
#Construcción de una red
 Para construir un mapa sencillo a mano, tener en cuenta las siguientes recomendaciones:

Crear una nueva capa para el mapa(Archivo->nueva capa) y editar su nombre a gusto en el panel “Capas” de la derecha.

Diagramar la red de calles utilizando las diversas herramientas que provee JOSM, y agregarles su etiqueta  de tipo de calle y nombre.

Las opciones de tipos de calles se muestran en la siguiente tabla.

Tipo de calle
Nro. carriles
Velocidad
Prioridad
highway.trunk
2
100 k/h
11
highway.trunk_link
1
80 k/h
10
highway.primary
2
100 k/h
9
highway.primary_link
1
80 k/h
8
highway.secondary
2
100 k/h 
7
highway.secondary_link
1
80 k/h
6
highway.tertiary
1
80 k/h
6
highway.unclassified
1
80 k/h
5
highway.residential
1
50 k/h
4
highway.footway
1
30 k/h
1
railway.rail
1
30 k/h
1
highway.track
1
20 k/h
1
highway.service
1
20 k/h
2
highway.living_street
1
10 k/h
3
highway.path
1
10 k/h
1
highway.steps
1
5 k/h
1

Para agregar semáforos, seleccionar el/los nodos sobre los cuales se va a colocar, e ir a “Predefinidos->Viales->Nodos de Vía->Semáforo”



La lógica por defecto de los semáforos se crea y puede ser editada sólo luego de haber exportado la red a sumo. Si se vuelve a exportar la red a sumo, se sobreescribe toda la lógica de los semáforos con lógica por defecto de sumo, por lo tanto, si se desea conservarla se recomienda utilizar la opción “Sumo->Network Building->Update Network”.   

Para crear restricciones de giro, seleccionar la calles y el nodo involucrado, y luego seleccionar “Crear nueva restricción de giro” en el panel de la derecha.

Si hay errores, en la pestaña de errores pueden solucionarse(en gral. hay que partir las calles en el nodo donde se intersecan).

Para crear los distritos, 
Para agregar access points,
Para agregar induction loops,

#Descargar una red de OpenStreetMap
 
 
#Modelar la demanda
 
 
#Ejecutar una simulación
