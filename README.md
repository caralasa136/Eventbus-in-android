# Event bus in android

**¿Qué es el event bus y para que nos sirve?**

Es un evento de publicar/suscribir optimizado para Android.

![alt text](https://github.com/greenrobot/EventBus/raw/master/EventBus-Publish-Subscribe.png)

+ Simplifica la comunicación entre componentes
+ Desacopla eventos de emisor y receptor
+ Trabaja bien con activities, fragments y background threads
+ Hace el código más simple

>Con **EventBus** se pueden realizar numerosas funcionalidades, incluso generar toda una forma de trabajar basada en estos eventos. Sin embargo, esto puede ser contraproducente, ya que EventBus te permite abstraerte de las herramientas de paso de mensajes y de notificaciones que brinda Android y el lenguaje en general; y, si se abusa, se puede generar una fuerte dependencia de esta herramienta, pudiendo incluso convertirse en el núcleo de nuestra aplicación. Esta no es una buena forma de trabajar, ya que estos eventos no son sencillos de depurar, ni es fácil ver cómo se propagan ni dónde se están capturando y cuándo, aunque posteriormente veremos algunos trucos que sí facilitan esta tarea.

>En cualquier parte se llama al método post de la instancia de **EventBus** y se propaga un evento. En cualquier parte de la app nos suscribimos en el momento que deseemos y, generando un método con una simple anotación, reaccionamos a dicho evento especificando en qué hilo se da la respuesta.

