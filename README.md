En mundos tan cambiantes y tecnologicos como en el que estamos viviendo, es importante aprender diferentes aplicaciones y herramientas que nos pueden agilizar y ayudar en nuesytro dia a dia.
Estamos en una industria en la que cada dia, es un dia nuevo, con nuevas formas de trabajar, nuevos caminos para desarrollar y mucho que aprender.
Por eso es tan importante, obtener y limpiar esos datos como saber entregarlos a nuestro publico objetivo.
Ahi, es donde las diferentes herramientas del BI nos van a ayudar y ahora es el momento de empezar a aprender.

Os voy a entregar un codigo de Python, en la extension Jupyter, con la que rapidamente podemos sacar una vision de nuestros datos y poder empezar a obtener insights, con los que posteriormente podremos trabajar mas detenidamente.

## Como crear un correo de empresa 

El proceso es tan simple como rapido, y lo primero de todo, tenemos que crearnos una "cuenta de empresa" con Microsoft, hay diferentes fuentes donde puedes ver tutoriales para hacerlo de una forma mas rapida.

Lo mas importante, es guardar tu nombre de usuario y contraseña(obviamente), porque lo vamos a utilizar seguidamente.

## Como crear un reporte en Jupyter Notebook

Una vez que tengamos una cuenta y seamos usuarios de Microsoft con cuenta de empresa, podemos ya trabajar en nuestro Jupyter Notebook.
1 STEP:

Seguidamente, vamos a importar o leer nuestro dataset 

2 STEP: 

Autentificamos nuestro usuario y conectamos los servidores Jupyter con Power BI
```
from powerbiclient import QuickVisualize, get_dataset_config, Report
from powerbiclient.authentication import DeviceCodeLoginAuthentication

import pandas as pd
```

3 STEP:

Llamamos al dataset que previamente hemos obtenido en la primera celda y generamos un dashboard con Power BI.

```
# Create a Power BI report from your data
PBI_visualize = QuickVisualize(get_dataset_config(df), auth=device_auth)

# Render the new report
PBI_visualize
```

4 STEP

Con esto, vamos a obtener un dashboard iteractivo donde podemos elegir el tipo de grafico que queremos, el tipo de datos que queremos visualizar, la cantidad de datos, y la forma de visualizarlo, en resumida, con esta herramienta, tenemos una vision rapida de nuestos datos y ver donde podemos atacarlos.



