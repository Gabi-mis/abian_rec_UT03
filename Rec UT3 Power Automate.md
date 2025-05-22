# REC UT\_03 

1. [Explicación de la aplicación. ................................ ...................... 3](#_page2_x69.00_y187.68) 
1. [instalar la aplicación. .............................................................. 4 ](#_page3_x69.00_y72.68)
1. [Explicación del proyecto................................. ........................... 7](#_page5_x69.00_y720.68) 
1. [realización del proyecto ........................................................... 8 ](#_page6_x69.00_y672.68)
1. [subirlo a github. ................................................................... 26](#_page25_x69.00_y72.68) 
1. [Creación del código en markdown ................................ ............ 27](#_page26_x69.00_y72.68)
1. [Explicación del código. ................................ ........................... 28](#_page26_x69.00_y722.68)

instalar la aplicación power automate hacer un pequeño proyecto subir ese proyecto al directorio de github con las imágenes en una carpeta aparte y crear en código markdown la misma presentación y subirlo a github también. 

### 1. Explicación<a name="_page2_x69.00_y187.68"></a> de la aplicación. 

Power Automate es una herramienta de Microsoft que permite automatizar tareas repetitivas sin necesidad de programar. Conecta aplicaciones como Outlook, Excel, Teams, OneDrive, entre muchas otras, para que puedas crear flujos de trabajo que envíen correos, muevan archivos, registren datos o te notifiquen automáticamente, ahorrando tiempo y evitando errores. También puedes usarlo en tu PC con Power Automate Desktop para automatizar acciones locales como abrir programas o mover archivos. 

### 2. instalar<a name="_page3_x69.00_y72.68"></a> la aplicación. 

Usando el siguiente enlace accedemos a la pagina de descargar: [enlace](https://make.powerautomate.com/environments/9e8bfa6d-5cbf-e202-9f18-63b91643c148/create)

ya en la página damos arriba derecha instalar para descargar el exe e instalar la aplicación: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.001.jpeg?raw=true)

damos en el installer y seguimos el asistente: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.002.png?raw=true)

damos en siguiente hasta completar el asistente:  

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.003.jpeg?raw=true)

aceptamos términos: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.004.jpeg?raw=true)

instalada le damos a iniciar aplicación: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.005.jpeg?raw=true)

### 3. Explicación<a name="_page5_x69.00_y720.68"></a> del proyecto. 

El proyecto que he decidido desarrollar consiste en un flujo sencillo pero funcional, cuyo objetivo principal es fusionar archivos PDF de manera rápida y automática mediante Power Automate Desktop. 

Al ejecutar el flujo, el usuario es guiado a través de una interfaz amigable que le solicita seleccionar dos archivos PDF mediante un explorador de archivos. Una vez seleccionados, se le pide que indique la carpeta de destino donde desea guardar el archivo resultante. El sistema genera un nuevo documento PDF que contiene ambos archivos combinados uno debajo del otro, respetando el orden en que fueron seleccionados y muestra un mensaje de confirmación al finalizar el proceso. 

Este flujo puede resultar especialmente útil para tareas administrativas, compilación de informes, entrega de documentación o incluso para resolver imprevistos de última hora en los que se necesiten unificar varios documentos de forma rápida y sin depender de programas externos. 

Aunque se trata de una solución sencilla, demuestra cómo una pequeña automatización puede ahorrar tiempo y mejorar la eficiencia en procesos cotidianos. 

### 4. realización<a name="_page6_x69.00_y672.68"></a> del proyecto. 

lo primero es crear el flujo y ponerle nombre: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.006.jpeg?raw=true)

asi se veria el flujo vacío: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.007.jpeg?raw=true)

empezando con el flujo vamos a la barra de la izquierda buscamos control de flujo> comentario para añadir comentarios que solo se verán en el flujo para ayudar al entendimiento del mismo: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.008.png?raw=true)

lo colocamos y escribimos la utilidad que tendrá el script: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.009.png?raw=true)

volvemos a la parte izquierda y buscamos cuadros de mensaje > mostrar formulario personalizado: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.010.jpeg?raw=true)

aquí nos dice las variables que se crean por defecto y la diseño del formulario: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.011.jpeg?raw=true)

al dar en diseñar nos sale lo siguiente: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.012.jpeg?raw=true)

añadimos un bloque de texto lo llamamos título y le ponemos lo que queramos que contenga:  

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.013.jpeg?raw=true)

ahora a la derecha tenemos el estilo del texto lo decoramos un poco y vemos que la vista previa también cambio: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.014.jpeg?raw=true)

creo otro bloque de texto en el cual pido el primer pdf: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.015.jpeg?raw=true)

ahora creo una inserción de archivo le pongo el id lo pongo en obligatorio y un mensaje de error: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.016.jpeg?raw=true)

hago lo mismo para el segundo archivo: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.017.jpeg?raw=true)

por último creo un boton de submit para poder enviar la orden del formulario: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.018.jpeg?raw=true)

ya con el formulario creado creo un comentario para explicar el siguiente paso: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.019.jpeg?raw=true)

ahora a la izquierda busco condicionales > if lo creo y le pongo en primer operador la variable que se generó en el formulario %ButtonPressed% (los % son para que el flujo tome el entendimiento de que lo que hay en medio es una variable): 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.020.jpeg?raw=true)

creo otro comentario: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.021.jpeg?raw=true)

creó un cuadro de diálogo de selección de carpeta esto nos abrira una ventanita para seleccionar donde dejar el archivo fusionado (observar que se genera una variable llamada destinationfolder): 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.022.jpeg?raw=true)

ahora en la izquierda de nuevo busco PDF > combinar archivos PDF creo una funcion llamada combinar archivos PDF seleccionó la variable del formulario y al lado entre corchetes el id de la selección de archivos que pusimos antes luego en la ruta del combinado ponemos la variable que se generó antes por defecto con el cuadro de diálogo de selección de carpeta y luego un nombre predeterminado como ArchivoFusionado.pdf: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.023.jpeg?raw=true)

ahora por último voy a la izquierda cuadros de mensaje > mostrar mensaje y le pongo el siguiente mensaje para indicar que se creó el archivo: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.024.jpeg?raw=true)

le doy a guardar y luego a ejecutar: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.025.jpeg?raw=true)

nos sale el formulario: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.026.jpeg?raw=true)

doy en el botón y seleccionó el archivo: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.027.jpeg?raw=true)

hago lo mismo con el otro y ahora con dos seleccionados le doy a OK: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.028.jpeg?raw=true)

ahora selecciono la carpeta donde voy a dejar el archivo fusionado: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.029.jpeg?raw=true)

y nos sale el siguiente mensaje: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.030.jpeg?raw=true)

por último voy al escritorio y veo que tengo el archivofusionado: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.031.png?raw=true)

lo abro para comprobar: 

ambos archivos uno frente al otro: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.032.jpeg?raw=true)

segundo archivo comprobación: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.033.jpeg?raw=true)

### 5. subirlo<a name="_page25_x69.00_y72.68"></a> a github. 

creó un nuevo directorio en mi github y meto la carpeta de capturas: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.034.jpeg?raw=true)

compruebo que todas las imagenes esten dentro: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.035.jpeg?raw=true)

### 6. Creación<a name="_page26_x69.00_y72.68"></a> del código en markdown. 

voy creando el código en markdown y usando las imágenes del github: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.036.jpeg?raw=true)

compruebo que va quedando bien usando ctrl+shift+v: 

![](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/md%20ut%2003/Aspose.Words.8fee132c-c070-4eaf-9290-a3ab8a19a8c7.037.jpeg?raw=true)

[link del script](https://github.com/Gabi-mis/abian_rec_UT03/blob/main/Rec%20UT3%20Power%20Automate.md) 

### 7. Explicación<a name="_page26_x69.00_y722.68"></a> del código. 

En Markdown se pueden utilizar varias estructuras básicas para organizar y dar formato al contenido de manera sencilla y legible. Entre las más comunes están los encabezados, que se crean con el símbolo # y sirven para jerarquizar títulos; las listas, tanto ordenadas (con números) como desordenadas (con guiones o asteriscos); el formato de texto, como negritas (\*\*texto\*\*), cursivas (\*texto\*) o tachado (~~texto~~); los enlaces ([texto](URL)) y imágenes (![texto](URL)); así como bloques de código (con triple acento grave    ) y citas (con >). Estas estructuras permiten crear documentos claros y bien estructurados, ideales para documentación, blogs o notas técnicas. 
