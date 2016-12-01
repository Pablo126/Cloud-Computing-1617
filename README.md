# Cloud-Computing-1617

## Proyecto sobre cloud computing

### EchaEquipos

#### - Introducción

EchaEquipos es un sistema que trata de solucionar el problema que puede provocar realizar actividades deportivas en grupo, en las que la diferencia de equipos puede provocar una falta de competitividad, perdida de tiempo o incluso crear problemas personales entre los diferentes participantes. Por lo tanto, se ha pensado en desarrollar servicios dedicados a realizar más facil este tipo de tareas.

#### - Solución

La intención es realizar una aplicación web basada en Python en la que una API REST realiza la conexión con otros microservicios.
Dentro de la gran cantidad de microservicios que se pueden desarrollar para este tipo de aplicación, se han elegido tres:
Gestión de jugadores: Se podrán general perfiles de jugadores para así poder realizar el reparto de equipos.
Gestion de estadísticas: Este servicio se encargará de recopilar datos de los jugadores, pudiendo proporcionar un mejor reparto de equipos u otro tipo de dato útil.
Log: Este servicio será en el encargado de proporcionar información del uso de la aplicación, así como de traza para posibles fallos del funcionamiento habitual.

#### - Tecnologías

En cuanto a la aplicación, se pretende usar algún framework basado en Python, tal como Django o Flask.
Para la gestion de jugadores, es un area que debe de estar muy bien definida, por lo que se usará un tipo de base de datos relacional como MySQL o Postgree.
El area de gestión de estadísticas se puede basar en cualquier tipo de base de datos, desde MongoDB hasta MySQL, depende de los datos que se vayan a manejar.
Por último, para el Log, se pretende usar [PaperTrail]( https://papertrailapp.com/).

#### - Provisionamiento

El sistema se va a desplegar en AWS, bajo un sistema Ubuntu server 14.
La razón de utilizar AWS es que tras probar AWS y Azure para los ejercicios de la asignatura, AWS me parece más rápido de lanzar, conectar y me ha dejado eliminar mi tarjeta de crédito, lo que me da la confianza de que no producirá costes. Tanto la imagen de Azure como la de AWS traen instalado python, que utilizaré para mi aplicación.
En cuanto sistema de provisionamiento, me ha gustado más Chef. Muy sencillo de instalar y la forma de crear las recetas es muy simple.
Para esta parte del proyecto se creará un directorio donde se almacenarán todos los archivos usados. Puede consultar la documentación [aquí](https://github.com/Pablo126/Cloud-Computing-1617/blob/master/provision/README.md).


#### - Licencia

El software está sujeto a la licencia [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/Pablo126/Cloud-Computing-1617/blob/master/LICENSE).
