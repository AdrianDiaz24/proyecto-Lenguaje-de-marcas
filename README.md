# 1º Análisis de requisitos y objetivos del proyecto:

**Requisitos Funcionales:**

  1º Menu desplegable:
  - Tiene que mostrar los componentes disponibles en la tienda
  - Tiene que ser intuitivo y fácil de usar

  2º Barra de busqueda:
  - Barra de busqueda en el header centrada que te permita buscar los diferentes tipos de productos

  3º Carrito:
  - imagend e un carrito que al clickarla te rediriga a la pagina del carrito con todos los productos añadidos por el usuario.

  4º Usuario:
  - Imagen de usuario que te redirigha a la pagina para iniciar sesion o registrarte y una vez lo haga te mande al menu de usuario

  5º Catalogo de productos:
  - Tiene que mostrar las fotos de los productos, su nombre y producto, ademas de haber un boton que te lleve a la cesta, y cuando clike el nombre o la foto del producto me lleve a su pagina donde vendran todas las caracteristicas

  6º Diseño adaptable:
  - El diseño de la pagina se debe adaptar a la vista de otros dispositivos o tamaños de pantaña

  7º Footer:
  - Pie de pagina con informacion sobre la empresa (aviso legal, redes sociales, entre otra informacion util.)

**Requisitos no funcionales:**

  1º Compatibilidad:
  - Compatible con los diferentes tipos de navegadores
  - Compatible con diferentes tipos de resolucion

  2º Rendimiento:
  - Debe estar optimizado para cargar rapido las paginas

  3º Mantenimiento:
  - El codigo debe estar limpio y organizado

**Tecnologias seleccionadas**

  HTML
  - Esencial para la creacion de cualquier pagina web, algunas de las ventaja que ofrecen son:
    - Sintaxis facil de entender y estructura simple.
    - Lenguaje estandar y compatibles con todos lo navegadores.
    - Facil de aprender.
   
  CSS
  - Esencial para el diseño de cualquier pagina web, algunas de sus ventajas son:
    - Cracion de diseños adaptables a la resolucion
    - Editar el diseño sin la necesidad de tocar el HTML, dejando este aun mas limpio
   
  Herramientas de desarrollo:
  - IDE: Visual Studio Code - Por su compatibilidad con HTML y CSS a travez de una facil instalacion de las extensiones disponibles, personalizacion, facil de usar e intuitivo
  - Validador: Validador de W3C - Que permitia comprobar la entandarizacion del codigo
  - Sistema de control de versiones: GitHub - Que permite llevar un control del progreso del proyecto y sus cambios

# 2º Creación de un wireframe en Balsamiq:

1º Pagina principal

![Wireframe del index.html](Images/Inicio.png)

Se decide agregar tambien una seccion donde mostras los producctos que se encuentran de oferta y el footer con la informacion necesaria.

2º Pestaña del producto

![Wireframe de la pestaña del producto](Images/Producto.png)

Se decide al final realizar un cambio dejando en el lado derecho los productos recomendados y abajo la descripcion y caracteristicas del producto.

3º Pestaña del carrito

![Wireframe de la pestaña del carrito](Images/Carrito.png)

Al final se decide cambiar el recuadro para en vez de englobar todos los produtos englobe cada producto un recuadro diferente, ademas de añadir un boton para retirar del carrito el producto.

4º Pestaña de incio de sesion

![Wireframe de la pestaña de inicio de sesion](Images/Iniciar_sesion.png)

Se crea tambien una variante para el registro de nuevos usuarios

5º Pestaña de usuario

![Wireframe de la pestaña del usuario](Images/Usuario.png)

Se decide que cada opcion este recuadrada y sea despregable, en la seccion pedido se añaden la fecha en la que se realizo y un boton para gestionar incidencias, y se cambian la opcion de otros ajustes por metodos de pago

# 3º Estructura HTML planificada:

**1º Index**

- Lang = "es": Se define el idioma principal al español
- Head:
  - Title: Se define el nombre de la pagina en este caso Componentes Manolo
  - Link: Se linkea el HTML con el CSS para poder hacer el diseño a la pagina
  - Meta: se define la codificacion de los caracteres para poder escribir los acentos y la ñ
- Body:
  - Header:
    -  Input (Checkbox) y label: Para crear la funcion de un menu hamburgesa desplegable
    -  Ul, Li y A para la creacion de lo que mostrara el menu hamburguesa y que rediriga a las paginas necesarias
    -  Imput (text): Para la creacion de la barra de busqueda
    -  Img y A: Para añadir las imagenes necesarias y que te redirigieran a las pestañas necesarias
  - Main:
    - Div: Uso del div para alinear en columnas las diferentes lienas de productos, las cuales son ordenadas por otro div con una clase, y dentro de estas lineas se encuentras los productos que son difenrenciados con div para cada uno de ellos
    - A y Img para añadir las fotos y los nombres de los productos y sea redireccionados a la pestaña del producto
    - Div y A: se usa dentro de los productos para alinear el boton que se realiza con CSS y te redirige a la cesta y el precio 
  - Footer:
    - Div: se uso para la creacion de las columnas de cada apartado del footer
    - H4: se usa para definir que se encontrara en cada columna
    - P y A: se usa para definir los apartados de cada columna y que los necesarios sean capaces de redirigirte a otra pagina
   
  **2º Pestaña del producto**

  - Lang = "es": Se define el idioma principal al español
- Head:
  - Title: Se define el nombre de la pagina en este caso Componentes Manolo
  - Link: Se linkea el HTML con el CSS para poder hacer el diseño a la pagina
  - Meta: se define la codificacion de los caracteres para poder escribir los acentos y la ñ
- Body:
  - Header:
    -  Input (Checkbox) y label: Para crear la funcion de un menu hamburgesa desplegable
    -  Ul, Li y A para la creacion de lo que mostrara el menu hamburguesa y que rediriga a las paginas necesarias
    -  Imput (text): Para la creacion de la barra de busqueda
    -  Img y A: Para añadir las imagenes necesarias y que te redirigieran a las pestañas necesarias
  - Main:
    - Section (grid): Se crea la seccion con el atributo class para poner esta zona de forma "grid" donde iria el producto principal en grande acompañado al lado de los productos recomendados
    - Article: Cada articulo corresponde al de un producto, donde se colocan los img para las fotos de los productos, el nombre que en caso de ser de uno producto recomendado al clickearlo te redirigiria a la pestaña de ese producto, el boton de comprar que te redirige al carrito y su precio
    - Section: Se usa de nuevo una seccion pero esta vez para la creacion de la informacion del producto junto a sus carracteristicas donde con Ul y Li se va identificando la diferente informacion del producto
  - Footer:
    - Div: se uso para la creacion de las columnas de cada apartado del footer
    - H4: se usa para definir que se encontrara en cada columna
    - P y A: se usa para definir los apartados de cada columna y que los necesarios sean capaces de redirigirte a otra pagina
   
  **3º Pestaña del carrito**

  - Lang = "es": Se define el idioma principal al español
- Head:
  - Title: Se define el nombre de la pagina en este caso Componentes Manolo
  - Link: Se linkea el HTML con el CSS para poder hacer el diseño a la pagina
  - Meta: se define la codificacion de los caracteres para poder escribir los acentos y la ñ
- Body:
  - Header:
    -  Input (Checkbox) y label: Para crear la funcion de un menu hamburgesa desplegable
    -  Ul, Li y A para la creacion de lo que mostrara el menu hamburguesa y que rediriga a las paginas necesarias
    -  Imput (text): Para la creacion de la barra de busqueda
    -  Img y A: Para añadir las imagenes necesarias y que te redirigieran a las pestañas necesarias
  - Main:
  - Footer:
    - Div: se uso para la creacion de las columnas de cada apartado del footer
    - H4: se usa para definir que se encontrara en cada columna
    - P y A: se usa para definir los apartados de cada columna y que los necesarios sean capaces de redirigirte a otra pagina
   
  **4º Pestaña de inicio de sesion**

  - Lang = "es": Se define el idioma principal al español
- Head:
  - Title: Se define el nombre de la pagina en este caso Componentes Manolo
  - Link: Se linkea el HTML con el CSS para poder hacer el diseño a la pagina
  - Meta: se define la codificacion de los caracteres para poder escribir los acentos y la ñ
- Body:
  - Header:
    -  Input (Checkbox) y label: Para crear la funcion de un menu hamburgesa desplegable
    -  Ul, Li y A para la creacion de lo que mostrara el menu hamburguesa y que rediriga a las paginas necesarias
    -  Imput (text): Para la creacion de la barra de busqueda
    -  Img y A: Para añadir las imagenes necesarias y que te redirigieran a las pestañas necesarias
  - Main:
  - Footer:
    - Div: se uso para la creacion de las columnas de cada apartado del footer
    - H4: se usa para definir que se encontrara en cada columna
    - P y A: se usa para definir los apartados de cada columna y que los necesarios sean capaces de redirigirte a otra pagina
   
  **5º Pestaña del usuario**

  - Lang = "es": Se define el idioma principal al español
- Head:
  - Title: Se define el nombre de la pagina en este caso Componentes Manolo
  - Link: Se linkea el HTML con el CSS para poder hacer el diseño a la pagina
  - Meta: se define la codificacion de los caracteres para poder escribir los acentos y la ñ
- Body:
  - Header:
    -  Input (Checkbox) y label: Para crear la funcion de un menu hamburgesa desplegable
    -  Ul, Li y A para la creacion de lo que mostrara el menu hamburguesa y que rediriga a las paginas necesarias
    -  Imput (text): Para la creacion de la barra de busqueda
    -  Img y A: Para añadir las imagenes necesarias y que te redirigieran a las pestañas necesarias
  - Main:
  - Footer:
    - Div: se uso para la creacion de las columnas de cada apartado del footer
    - H4: se usa para definir que se encontrara en cada columna
    - P y A: se usa para definir los apartados de cada columna y que los necesarios sean capaces de redirigirte a otra pagina

# 4º Informe de accesibilidad y mejoras aplicadas
