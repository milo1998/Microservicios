## Universidad Distrital Francisco José de Caldas
## Facultad de Ingeniería
## Proyecto Curricular de Ingeniería de Sistemas

## Gestión Tecnológica

### Integrantes:

* Norbey Danilo Muñoz Cañón       20151020050
* Brayan Leonardo Sierra Forero   20151020059
* Camilo Enrique Rocha Calderón   20151020035

### Ejercicio de Microservicios

El presente ejercicio da muestra de la implementación de microservicios mediante la utilización de Docker y Flask. Se realiza una calculadora que hace las cuatro operaciones básicas matemáticas: suma, resta, multiplicación y divisón. Cada operación se ve como un servicio, se implementa con Flask y a su vez se vinculan mediante definición de la arquitectura de microservicios de modo que se logra integrar cada uno de ellos (servicios - operaciones) a un unico propósito.

Con la realización de cada uno de los servicios y su integración, se desarrolla una clase gateway que brinda el acceso a cada servicio de acuerdo con lo que solicite la clase cliente. Todo esto se lleva a cabo en un proceso de dockerización. 

### El contenido del proyecto desribe:

#### app

* app.py hace la veces de gateway. Brinda el acceso al servicio solicitado

* Dockerfile contiene el conjunto de instrucciones que describen las imagenes deseadas y permiten la construcción automática

* requirements.txt contiene las dependencias necesarias ha ser instaladas. Estas se deben entregar a la imagen para ser incorporadas

#### cliente

* cliente.py es la clase que captura los valores y la operación para indicar el servicio requerido al gateway y responder a la solicitud

* Dockerfile contiene el conjunto de instrucciones que describen las imagenes deseadas y permiten la construcción automática

* requirements.txt contiene las dependencias necesarias ha ser instaladas. Estas se deben entregar a la imagen para ser incorporadas

#### suma, resta, multiplicación, división

* {suma, resta, multiplicación, división}.py retorna la operación a realizar

* Dockerfile contiene el conjunto de instrucciones que describen las imagenes deseadas y permiten la construcción automática

* requirements.txt contiene las dependencias necesarias ha ser instaladas. Estas se deben entregar a la imagen para ser incorporadas

#### docker-compose

Incluye la construcción de cada uno de los servicios, el gateway y el cliente. 

