# WORKSHOP 8 - Api para web de Tartas

En esta ocasión, como en los ejercicios anteriores, vamos a indicarte la funcionalidad que debe tener el API y tú debes encargate de la implementación.

Vamos a realizar el API para una web de compra de tartas, bienvenido a Tartinchis:

![HOME.jpeg](/assets/HOME.jpeg)

Recuerda que debes aplicar todo lo que has visto en el curso a excepción de SQL:

- Mongo
- Typescript
- Testing
- Arq. Hexagonal
- Swagger
- ...
- etc

**LISTADO DE TARTAS**

Dentro de nuestra web será posible consultar la lista de tartas:

![LISTADO DE TARTAS.jpeg](/assets/LISTADO_DE_TARTAS.jpeg)

**FILTRADO**

Las tartas tendrán una serie de filtros relacionados con las características de las tartas, por ejemplo:

![FILTROS.jpg](/assets/FILTROS.jpg)

Si pulsamos en “Fruta” veremos las tartas que son de tipo fruta, pero no significa que esas tartas no puedan estar en otras categorías, por ejemplo en Sin gluten o en “Las favoritas de Fran”. Es decir que una tarta puede pertenecer a varias categorías.

**DETALLE**

Un usuario puede consultar el detalle de una tarta:

![DETALLE.png](/assets/DETALLE.png)

Es importante tener en cuenta que las tartas tienen una descripción, un título… y muy importante: una lista de alérgenos:

![Untitled](/assets/Untitled.png)

**REGISTRO Y LOGIN**

Si el usuario quiere hacer un pedido deberá obligatoriamente registrarse y hacer login:

![Untitled](/assets/Untitled%201.png)

**CARRITO**

Para hacer un pedido un usuario deberá añadir productos a su carrito:

![Untitled](/assets/Untitled%202.png)

**FINALIZAR COMPRA**

Cuando haya terminado de añadir productos el usuario podrá realizar el pedido, para ello se le pedirán los datos de envío de ese pedido:

![Untitled](/assets/Untitled%203.png)

**PAGO**

El pago deberá realizarse mediante BIZUM, así que cuando termines el pedido se te indicará que hagas un bizum con tu código de pedido 

**EXTRAS**

Las tartas tendrán ingredientes, por ejemplo:

TARTA DE QUESO:

- 6 huevos
- 100g harina
- 600g queso
- 200ml nata

TARTA DE CHOCOLATE:

- 400g de chocolate
- 80g de mantequilla
- 250ml de leche

Cuando finalices el pedido, la API deberá revisar si hay ingredientes suficientes para hacer todas las tartas que se han indicado en el pedido, en caso de que no haya dará un error 400 y se avisará al usuario de que debe quitar alguna tarta.
