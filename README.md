# AZ900-WebApp
"App Service" es un servicio que se utiliza para las aplicaciones de grado empresarial este servivcio es un servicio web.

Guía para crear una Web App dentro de Azure.

Lo primero que debemo hacer, es dirigirnos al portal de [Azure](https://portal.azure.com/#home).

## Paso 1
En en la vista de Home seleccionamos la opcion "Crear un recurso".

![1W](https://user-images.githubusercontent.com/99112892/173209337-dd01e7e0-29f6-40d3-ad7e-33c6290a6f3a.png)

## Paso 2
Nos aparaceran distintos servicios, elegimos 'Aplicación Web'.

![2W](https://user-images.githubusercontent.com/99112892/173213894-2d35c5ee-80d9-43da-b2ea-a42dcb9ebe46.png)


## Paso 3
### Pestaña:Datos básicos
- Nos aseguramos de que la suscripción es de tipo 'student'.
- Creamos un nuevo grupo de recursos, el cual sería un folder donde vamos a guardar nuestra aplicación web dentro de la nube, lo nombramos como: lab02-dr.
- Le damos un nombre a nuestra aplicación web, en este caso la nombro: lab002-dr.
- En la sección publicar, marcamos la que dice 'Código' ya que utilizaremos el código desde un repositorio de GitHub el cual se obtuvo mediante un fork de la Sherpa [Fer](https://github.com/FernandaOchoa).
- La 'pila del entorno en tiempo de ejecución' es con el lenguaje/codigo con el que esta realizada
nuestra aplicacion, en este caso pondre: Node 14 LTS.

![3W_Basics1](https://user-images.githubusercontent.com/99112892/173209436-aca75777-d83e-4abe-9f3c-ddad7acbbcc6.png)

- El sitema operativo en este ejemplo lo dejo en Linux.
- En Región seleccionamos Central US.
- Dentro del "Plan de App service" dejaremos el SKU y tamaño con la opción ´Básico B1'.

![3W_Basics2](https://user-images.githubusercontent.com/99112892/173209449-94c57b4c-c91b-4608-ad76-39d89cdff568.png)

### Pestaña:Implementación(Deployment)
- En el apartado de "Configuración de Acciones de Github' elegimos "habilitar", de inmediato nos saldra una ventana emergente, donde nos pedira que autorizemos el acceso o conexión a nuestro perfil de GitHub.

![3W_Imple1](https://user-images.githubusercontent.com/99112892/173209606-491b4696-0b20-41c7-976f-b3a849e642af.png)

![3W_Imple1 1](https://user-images.githubusercontent.com/99112892/173209612-07124036-bb1c-4e4a-9324-364012112358.png)

- La organización ponemos el perfil de nuestro GitHub.
- En repositorio tendremos acceso a todos lo que tenemos en nuestro perfil, incluyendo a los forks, seleccionare 'lab1'.
- La rama/branch es 'master'.

![3W_Imple2](https://user-images.githubusercontent.com/99112892/173209640-8da76110-5acc-477f-b099-d1d687619126.png)

- Nos da una vista previa del archivo y su configuracion de flujo de trabajo. 

![3W_Imple3](https://user-images.githubusercontent.com/99112892/173209648-8f3730c7-21bf-46e4-9b1f-5949b56244fa.png)

### Pestaña:Redes(Networking)
- Se queda con la configuración predeterminada. 

![3W_Redes](https://user-images.githubusercontent.com/99112892/173209666-723bbc89-60ea-49db-9091-ab0e929bcebd.png)

### Pestaña:Supervisión(Monitoring)
- Como no utilizaremos 'Insights' lo dejamos con la configuración predeterminada.

![3W_Supervision](https://user-images.githubusercontent.com/99112892/173209689-8c207e33-65d4-4808-a08c-7f4cac0c98a1.png)

### Pestaña:Tags(Etiquetas)
Las etiquetas nos sirven para cuando hay muchas personas trabajando dentro de una organización, es importante saber quien esta subiendo que cambios.
-En el campo nombre es muy usual poner: CreatedBy y para el campo valor ponemos por quien fue creado.
- Podemos observar que hay 12 recursos que se crean de manera automatica.
- Agregamos otra etiqueta con Nombre:Area y Valor:Rivan.
- Finalizamos con una ultima Nombre:Ciclo y Valor:7maEd.

![3W_Etiquetas](https://user-images.githubusercontent.com/99112892/173209750-a35c90d1-3afa-47e0-91e8-fc217b94ae36.png)

### Pestaña:Review+Create(Revisar y Crear)
Va a tomar el codigo de la aplicación hecha(GitHub) y se lo traera a Azure para empezar a trabajar sobre de él.
- Pulsamo en 'crear'.

![3W_RevisarCrear](https://user-images.githubusercontent.com/99112892/173209780-b715ec5a-ad81-4d64-bfd5-291b8efce3ee.png)

- Podemos ver que se completo la implementación y nuestra aplicación esta lista.

![3W_Finalizada](https://user-images.githubusercontent.com/99112892/173209793-d7d40c2f-bbf5-41f1-bd90-e1eaca22fa9a.png)
