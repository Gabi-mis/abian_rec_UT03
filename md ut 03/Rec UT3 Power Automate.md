REC UT\_03 



instalar la aplicación power automate hacer un pequeño proyecto subir ese proyecto al directorio de github con las imágenes en una carpeta aparte y crear en código markdown la misma presentación y subirlo a github también. 

1. Explicación de la aplicación. 

Power Automate es una herramienta de Microsoft que permite automatizar tareas repetitivas sin necesidad de programar. Conecta aplicaciones como Outlook, Excel, Teams, OneDrive, entre muchas otras, para que puedas crear flujos de trabajo que envíen correos, muevan archivos, registren datos o te notifiquen automáticamente, ahorrando tiempo y evitando errores. También puedes usarlo en tu PC con Power Automate Desktop para automatizar acciones locales como abrir programas o mover archivos. 

2. instalar la aplicación. 

Usando el siguiente enlace accedemos a la pagina de descargar: [enlace](https://make.powerautomate.com/environments/9e8bfa6d-5cbf-e202-9f18-63b91643c148/create)

ya en la página damos arriba derecha instalar para descargar el exe e instalar la aplicación: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.001.jpeg)

damos en el installer y seguimos el asistente: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.002.png)

damos en siguiente hasta completar el asistente:  

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.003.jpeg)

aceptamos términos: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.004.jpeg)

instalada le damos a iniciar aplicación: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.005.jpeg)

3. Explicación del proyecto. 

El proyecto que he decidido desarrollar consiste en un flujo sencillo pero funcional, cuyo objetivo principal es fusionar archivos PDF de manera rápida y automática mediante Power Automate Desktop. 

Al ejecutar el flujo, el usuario es guiado a través de una interfaz amigable que le solicita seleccionar dos archivos PDF mediante un explorador de archivos. Una vez seleccionados, se le pide que indique la carpeta de destino donde desea guardar el archivo resultante. El sistema genera un nuevo documento PDF que contiene ambos archivos combinados uno debajo del otro, respetando el orden en que fueron seleccionados y muestra un mensaje de confirmación al finalizar el proceso. 

Este flujo puede resultar especialmente útil para tareas administrativas, compilación de informes, entrega de documentación o incluso para resolver imprevistos de última hora en los que se necesiten unificar varios documentos de forma rápida y sin depender de programas externos. 

Aunque se trata de una solución sencilla, demuestra cómo una pequeña automatización puede ahorrar tiempo y mejorar la eficiencia en procesos cotidianos. 

4. realización del proyecto. 

lo primero es crear el flujo y ponerle nombre: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.006.jpeg)

asi se veria el flujo vacío: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.007.jpeg)

empezando con el flujo vamos a la barra de la izquierda buscamos control de flujo> comentario para añadir comentarios que solo se verán en el flujo para ayudar al entendimiento del mismo: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.008.png)

lo colocamos y escribimos la utilidad que tendrá el script: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.009.png)

volvemos a la parte izquierda y buscamos cuadros de mensaje > mostrar formulario personalizado: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.010.jpeg)

aquí nos dice las variables que se crean por defecto y la diseño del formulario: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.011.jpeg)

al dar en diseñar nos sale lo siguiente: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.012.jpeg)

añadimos un bloque de texto lo llamamos título y le ponemos lo que queramos que contenga:  

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.013.jpeg)

ahora a la derecha tenemos el estilo del texto lo decoramos un poco y vemos que la vista previa también cambio: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.014.jpeg)

creo otro bloque de texto en el cual pido el primer pdf: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.015.jpeg)

ahora creo una inserción de archivo le pongo el id lo pongo en obligatorio y un mensaje de error: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.016.jpeg)

hago lo mismo para el segundo archivo: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.017.jpeg)

por último creo un boton de submit para poder enviar la orden del formulario: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.018.jpeg)

ya con el formulario creado creo un comentario para explicar el siguiente paso: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.019.jpeg)ahora a la izquierda busco condicionales > if lo creo y le pongo en primer operador la variable que se generó en el formulario %ButtonPressed% (los % son para que el flujo tome el entendimiento de que lo que hay en medio es una variable): 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.020.jpeg)

creo otro comentario: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.021.jpeg)

creó un cuadro de diálogo de selección de carpeta esto nos abrira una ventanita para seleccionar donde dejar el archivo fusionado (observar que se genera una variable llamada destinationfolder): 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.022.jpeg)

ahora en la izquierda de nuevo busco PDF > combinar archivos PDF creo una funcion llamada combinar archivos PDF seleccionó la variable del formulario y al lado entre corchetes el id de la selección de archivos que pusimos antes luego en la ruta del combinado ponemos la variable que 

se generó antes por defecto con el cuadro de diálogo de selección de carpeta y luego un nombre predeterminado como ArchivoFusionado.pdf: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.023.jpeg)

ahora por último voy a la izquierda cuadros de mensaje > mostrar mensaje y le pongo el siguiente mensaje para indicar que se creó el archivo: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.024.jpeg)

le doy a guardar y luego a ejecutar: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.025.jpeg)

nos sale el formulario: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.026.jpeg)

doy en el botón y seleccionó el archivo: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.027.jpeg)

hago lo mismo con el otro y ahora con dos seleccionados le doy a OK: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.028.jpeg)

ahora selecciono la carpeta donde voy a dejar el archivo fusionado: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.029.jpeg)

y nos sale el siguiente mensaje: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.030.jpeg)

por último voy al escritorio y veo que tengo el archivofusionado: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.031.png)

lo abro para comprobar: 

ambos archivos uno frente al otro: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.032.jpeg)

segundo archivo comprobación: 

![](Aspose.Words.9ff07682-276b-4f5f-b9c8-a0a452ccac22.033.jpeg)

5. subirlo a github. 
5. Creación del código en markdown. 
5. Comprobación del código. 
