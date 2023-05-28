Tarea Microservicios - AREP
Tarea
En grupos de máximo 3.
Diseñe un API y cree un monolito Web en Spark que permita a los usuarios hacer posts de 140 caracteres e ir registrandolos en un stream único de posts (a la Twitter). Piense en tres entidades Usuario, hilo(stream), posts.
Cree un aplicación JS para usar el servicio. Depliegue la aplicación en S3. Asegúrese que esté disponible sobre internet.
Pruebe la aplicación Web
Agregue seguridad usando JWT con el servicio cognito de AWS.
Separe el monolito en tres microservicios independientes.
Despliegue el seervicio en AWS con EC2 y realice pruebas (Puede usar docker o 3 máquinas AWS)
Entregue el código desarrollado en Github, un reporte de la arquitectura, un reporte de las pruebas, y un video con el experimento funcionando y bien configurado (Todo en el README).
Arquitectura
arquitecturaArep

Reporte Arquitectura
Se instancian 3 maquinas en EC2 , una sera para el servicio de login, otra para el back y otra para el front,se utiliza spark en java para el manejo de las entradas y salidas, la instancia que contiene el front se conectara dcon el back y con el servicio de login.

Reporte Pruebas
Se crearon dos usuarios en la base de datos de Mongo para ingresar al twitter


Se alamacenan los tweets generados por cada usuario



