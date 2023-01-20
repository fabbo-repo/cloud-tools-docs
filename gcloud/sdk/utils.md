### Inicializar cuenta y proyecto en gcloud sdk (tambien sirve para crear una nueva confiuracion)
~~~
gcloud init
~~~

### Cuentas configuradas
~~~
gcloud auth list
~~~

### Revisar configuracion
~~~
gcloud config list
~~~

### Revisar historial de configuraciones
~~~
gcloud config configurations list
~~~

### Activar una configuración
~~~
gcloud config configurations activate <NAME>
~~~

### Eliminar una configuración (antes de hacerlo hay que activar otra configuracion)
~~~
gcloud config configurations delete <NAME>
~~~

### Revisar proyectos asociados a la cuenta configurada
~~~
gcloud projects list
~~~

### Revisar componentes/modulos instalados
~~~
gcloud components list
~~~

