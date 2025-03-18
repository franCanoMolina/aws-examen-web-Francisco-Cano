# CREAR UNA VPC EN AWS
![](./imagenes/image.png)

Configutamos la VPC con:
- Nombre "mi-vpc-Francsico-Cano." 
- el CIDR Block: 10.0.0.0/16

## CREACION DE UNA SUDRET
![](./imagenes/nombre-subred.png)

Escogeremos el id de la VPC creada anteriormente

![alt text](./imagenes/config-real.png)

la configuracion de la primera subred sera la siguiente:
- nombre: "subnet-linux"
- CIDR: 10.0.1.0/24


![](./imagenes/config-2.png)

Para la configuracion de la segunda subred, volveremos a escoger el id de la VPC creada anteriormente y su configuracion sera la siguiente:

- nombre: "subnet-windows:"
- CIDR: 10.0.2.0/24

## CREACION DE UNA INTERNET GATEWAY

![](./imagenes/gatwey.png) 

Para la cmfiguracion de la gateway le pondremos un nombre y 

![](./imagenes/vpc-gatwey.png)

y a continuacion la conectaremos a la VPC

## TABLA DE ENRUTAMINETO

![](./imagenes/tablas-rut.png)

Configuramos la tabla de enrutamiento con: 
 nombre; "tabla-rut-Francisco-Cano" y la 
 
![](./imagenes/edit-ruta.png)

Editaremos la ruta con una en (0.0.0.0/0) y el destino "pueta de enlace internet"
 
# EC2 CREACION DE INSTANCIAS (UBUNTU)

![](./imagenes/configuracion-ec2-1.png)

Para empezar la configuracion pondremos:

- nombre: Instancia-Francisco-Cano
- imagen de SO: ubuntu

![](./imagenes/imagen-pred.png)

Para la imagen dejaremos la predeterminada en la configuracion

![alt text](./imagenes/claves.png)

Creamos el par de claves y la guardmos en nuestro ordenador

![alt text](./imagenes/cong-red-2.png)

Los primeros pasos del apartado de la configuracion de la red es , enlazarlo a la VPC (vendra directamente en la congiguracion) y la subred que deseemos, en este caso "Subnet-linux"

# EC2 CREACION DE INSTANCIAS (WINDOW)

![alt text](./imagenes/ecs-window.png)

Empezamos la configuracion poniendo nombre y SO deseaso, en este caso ahora escogeremos window y de imagen la predeterminada por el programa

![alt text](./imagenes/tipo-instancia-window.png)

En el tipo de instancia escogeremos en este caso: t3.medium

![alt text](./imagenes/par-d-clasves-window.png)

haremos un nuevo par de claves para esta instancia

![alt text](./imagenes/salida-window.png)

de esta forma configuraremos las reglas de salida

![alt text](./imagenes/entradaaa.png)

Y de esta formas las de entrada 








# SECURITY GROUPS AWS 

![alt text](./imagenes/config-seguridad.png)

Empezamos con la configuracion de el grupo de seguridad poniendole un nombre: server-group-Francisco-Cano, y enlazando la VPC deseada

![alt text](./imagenes/entrada.png)

En las reglas de entrada pondremos estas configuraciones 

![alt text](./imagenes/salida.png)

Y en la de salida estas configuraciones
























