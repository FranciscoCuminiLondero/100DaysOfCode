# Diseño Web Responsivo (Responsive Web Design)

### [**HTML**](https://www.freecodecamp.org/espanol/learn/2022/responsive-web-design/learn-html-by-building-a-cat-photo-app/step-1)

#### **Step 1**  
Los elementos HTML tienen etiquetas ("_tags_") de **apertura** `<h1>` y etiquetas de **cierre** `</h1>`. 
```html
<h1>Hola Mundo!</h1>
```

#### **Step 2**   
Existen 6 elementos de encabezado: desde el `<h1>` al `<h6>`, utilizados para indicar la importancia del contenido debajo de ellos. Cuanto menor sea el número, mayor será la importancia.

```html
<h1>Título</h1> <!-- Uno solo -->
<h2>Subtitulo</h2> <!-- Dos o Tres -->
<h3>subtitulos</h3> <!-- Los que querramos -->
<h4>subtitulos</h4> <!-- Los que querramos -->
<h5>subtitulos</h5> <!-- Los que querramos -->
<h6>subtitulos</h6> <!-- Los que querramos -->
```

#### **Step 3** 
Los elementos `<p></p>` se usan para crear parrafos.

```html
<p>
	Esto es un párrafo!
</p>
```

#### **Step 4** 
Comentar permite dejar mensajes que no vea el usuario, y también para hacer que parte del código este inactivo. En HTML se utiliza: `<!-- -->`.

```html
<!-- Soy un comentario -->
```

#### **Step 5**
HTML5 tiene elementos que identifican áreas de contenido, permitiendo que el código sea más fácil de leer y ayuda con la optimización de motores de búsqueda (SEO) y la accesibilidad.
Con el `<main></main>` identificamos la **sección principal** de la página.

```html
<body>
  <h1>Título</h1>
  <main>
    <h2>Subtítulo</h2>
    <!-- Comentario -->
    <p>Soy un Párrafo</p>
  </main>
</body>
```

#### **Step 6**
En la **step 5**, anidamos elementos al `<main></main>`. Un elemento **anidado** es un elemento secundario del principal, y decimos que se encuentra _dentro_ de este.

#### **Step 7** 
Podemos agregar imagenes usando el elemento `<img>`, los cuales tienen una etiqueta de apertura pero no una de cierre, llamadas **etiquetas de cierre automático**.

#### **Step 8**
Los **atributos** son palabras especiales que se usan dentro de las etiquetas de apertura de un elemento para controlar el comportamiento del mismo. El atributo 'src' en una `<img>` especifíca la URL de la imagen (dónde se encuentra).

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg">
```

#### **Step 9**
Todos los elemento `<img>` deben tener un atributo 'alt', que se usa para que los lectores de pantalla mejoren la accesibilidad y es lo que se muestra si la imagen no carga.

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back">
```

#### **Step 10**
Podemos vincular nuestra página a otra con el elemento ancla (_anchor_) `<a><a>`.

```html
<a href="https://freecatphotoapp.com"></a>
```
_**NOTA**_: En este ejemplo no visualizaremos nada en el navegador.

#### **Step 11**
El texto, para que aparezca enlazado, debe colocarse entre las etiquetas `<a></a>`.

```html
<a href="https://freecatphotoapp.com">cat photos</a>
```

#### **Step 12**
Además, podemos colocar `<a></a>` en una parte de un parrafo, imagen, título, etc... para vincularlo.

```html
<p>Click here to view more <a href="https://freecatphotoapp.com">cat photos</a>.</p>
```
_**NOTA**_: Solo vincula el "cat photos".

#### **Step 13**
Con el atributo 'target' con el valor _blank_ en el elemento `<a></a>` abre el enlace en una nueva pestaña.

```html
<p>Click here to view more <a href="https://freecatphotoapp.com" target="_blank">cat photos</a>.</p>
```

#### **Step 14**
Además, podemos colocar el elemento `<a></a>` alrededor de una etiqueta `<img>` para vincularla.

```html
<a href="https://freecatphotoapp.com" target="_blank"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
```

#### **Step 15**
Antes de agregar contenido nuevo, tenemos que usar el elemento `<section></section>` para separar el contenido anterior del nuevo.

```html
<main>
      <section>
        <h2>Cat Photos</h2>
        <!-- TODO: Add link to cat photos -->
        <p>Click here to view more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a>.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>
    </main>
```

#### **Step 16**
Agregamos una nueva sección, debajo de la anterior.

```html
	  <section>
        <h2>Cat Photos</h2>
        <!-- TODO: Add link to cat photos -->
        <p>Click here to view more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a>.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>
      <section>
        
      </section>
```

#### **Step 17**
Agregamos un `<h2></h2>` en la nueva `<section></section>`.

```html
	  <section>
        <h2>Cat Lists</h2>
      </section>
```

#### **Step 18**
Cuando agregamos un elemento de encabezado de rango inferior, se da a entender que comienza una nueva sección.

```html
      <section>
        <h2>Cat Lists</h2>
        <h3>Things cats love:</h3> <!-- Nueva Sección -->
      </section>
```

#### **Step 19**
Dentro de las etiquetas `<ul></ul>` creamos una lista **desordenada**.

```html
        <h2>Cat Lists</h2>
        <h3>Things cats love:</h3>
        <ul>
                <!--NO va a aparecer nada porque no le asignamos elementos-->
        </ul>
```
***NOTA***: La lísta **desordenada** se muestra en la página con puntitos '**·**'

#### **Step 20**
Con los elementos `<li></li>` agregamos "items" a la lista.

```html
        <ul>
          <li>cat nip</li>
          <li>laser pointers</li>
          <li>lasagna</li>
        </ul>
```

#### **Step 21**
Agregamos una nueva `<img>` al documento.

#### **Step 22**
El elemento `<figure></figure>` permite asociar una imagen con un pie de foto.

```html
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
        </figure>
```

**Step 23**
El elemento `<figcaption></figcaption>` se usa para agregar una **leyenda** para describir la imagen dentro del elemento `<figure></figure>`.

```html
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
          <figcaption>Cats love lasagna</figcaption>
        </figure>
```

#### **Step 24**
Con la etiqueta `<em></em>` transformamos el texto, que rodea, en _itálica_ o _cursiva_, y sirve para enfatizar texto.

```html
          <figcaption>Cats <em>love</em> lasagna.</figcaption>
```

#### **Step 25**
Agregamos un nuevo `<h3></h3>`.

#### **Step 26**
Dentro de las etiquetas `<ol></ol>` creamos una lista **ordenada**.

```html
        <h3>Top 3 things cats hate:</h3>
        <ol>
          <li>flea treatment</li>
          <li>thunder</li>
          <li>other cats</li>
        </ol>
```
***NOTA***: La lista **ordenada** se muestra enumaradas "1. , 2. , 3. , ..."

#### **Step 27**
Agregamos otro elemento `<figure></figure>`.

#### **Step 28**
Agregamos otra `<img>`.

#### **Step 29**
Le agregamos a `<img>` el atributo 'alt'.

#### **Step 30**
Agregamos un elemento `<figcaption></figcaption>`.

#### **Step 31**
Con la etiqueta `<strong></strong>` ponemos el texto en **negrita**, y sirve indicar que es de mucha importancia.

```html
<figcaption>Cats <strong>hate</strong> other cats.</figcaption>
```

#### **Step 32**
Agregamos una nueva `<section></section>`.

#### **Step 33**
Agregamos un `<h2></h2>`.

#### **Step 34**
Agregaremos un formulario con las etiquetas: `<form></form>`, que permitirá recopilar información de los usuarios.

```html
        <h2>Cat Form</h2>
        <form>
          
        </form>
```

**Step 35**
El atributo 'action' dentro de `<form>` indica dónde se deben enviar los datos recojidos en el formulario.

```html
        <form action="https://freecatphotoapp.com/submit-cat-photo"> <!-- El '/submit-cat-photo' es a donde se va a enviar -->
        </form>
```

#### **Step 36**
Los elementos `<input>` permiten en los formularios recopilar datos de distintas formas. Al igual que `<img>` se cierra automáticamente.

```html
        <form action="https://freecatphotoapp.com/submit-cat-photo">
          <input>
        </form>
```

#### **Step 37**
Hay varios tipos de `<input>` que podemos crear usando el atributo 'type' (campo de texto, campo de constraseña, botón de reinicio, un control para que los usuarios puedan seleccionar un archivo local de su computadoras, etc).

```html
        <input type="text">
```

#### **Step 38**
Para que la ubicación especificada en el atributo 'action' en el `<form></form>` acceda a los datos del formulario, se le debe otorgar al `<input>` un atributo 'name' y asignarle un valor que representen los datos que toma. 

```html
        <input type="text" name="catphotourl">
```

#### **Step 39**
El atributo 'placeholder' se usa para informarle al usuario qué tipo de información debe ingresar en el `<input>`.

```html
        <input type="text" name="catphotourl" placeholder="cat photo URL">
```

#### **Step 40**
Para evitar que los usuarios envién formularios cuando falta información, se debe agregar el atributo 'required' en el `<input>`, se coloca sin ningún valor.

```html
        <input type="text" name="catphotourl" placeholder="cat photo URL" required>
```

#### **Step 41**
Usamos el elemento `<button></button>` para crear un botón clicable.
El comportamiento predeterminado que tiene un botón, dentro de un formulario sin ningún atributo, es enviar el formulario a la ubicación especificada en el atributo 'action' del `<form></form>`.

```html
        <input type="text" name="catphotourl" placeholder="cat photo URL" required>
        <button>Submit</button>
```

#### **Step 42**
Aunque agregamos el `<button></button>` debajo del `<input>`, el primero aparece al lado del segundo, y esto se debe a que ambos son **elementos en línea**.
El `<button></button>`, como ya vimos, envía el formulario de forma predeterminada, pero si le agregamos el atributo 'type' con el valor _submit_ queda más claro.

```html
        <button type="submit">Submit</button>
```

#### **Step 43**
Podemos usar `<input>` con el atributo 'type' con el valor _radio_ para que solo se pueda seleccionar una opción entre múltiples. 

```html
        <input type="radio"> Indoor
```

#### **Step 44**
Los elementos `<label></label>` se usan para asociar **el texto de un `<input>`** con el propio `<input>` (principalmente para lectores de pantalla). Es una etiqueta para un elemento.

```html
        <label><input type="radio"> Indoor</label>
```

#### **Step 45**
El atributo 'id' se usa para identificar un elemento en HTML. El valor de cada 'id' debe ser único, no puede haber dos elementos con el mismo 'id'.

```html
        <label><input type="radio" id="indoor"> Indoor</label>
```
***NOTA***: Cuando los elemento tienen múltiples atributos no importa el orden de los mismos.

#### **Step 46**
Agregamos una nueva `<label></label>` con un `<input>`.

#### **Step 47**
Tengamos en cuenta que ambos botones se pueden seleccionar al mismo tiempo. Para evitar esto, tenemos que hacer que ambos botones tenga un atributo 'name' con el mismo valor, permitiendo que al seleccionar uno se deseleccione el otro. 

```html
        <label><input id="indoor" type="radio" name="indoor-outdoor"> Indo</label>
        <label><input id="outdoor" type="radio" name="indoor-outdoor"> Outdoor</label>
```

#### **Step 48**
Si seleccionamos, por ejemplo, el botón de radio con la opción "_Indoor_" y enviamos el formulario, los datos que se envían se basan en sus atributos 'name' y 'value'.
En el caso anterior solo contamos con el 'name' por lo tanto en ambos casos se enviará "indoor-outdoor", para evitar esto debemos colocar un 'value' con el mismo valor del 'id' y así en cada caso se enviará con su valor correspondiente.

```html
          <label><input id="indoor" value="indoor" type="radio" name="indoor-outdoor"> Indoor</label>
          <label><input id="outdoor" value="outdoor" type="radio" name="indoor-outdoor"> Outdoor</label>
```

#### **Step 49**
Los elementos `<fieldset></fieldset>` se usan para agrupar `<input>` y `<label></label>` en un formulario. Son elementos en **bloque**, es decir aparecen en una línea nueva.

```html
          <fieldset>
            <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
            <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
          </fieldset>
```
***NOTA***: Coloca los `<input>` como en un "recuadro".


#### **Step 50**
El elemento `<legend></legend>` se comporta como un título para el elemento `<fieldset></fieldset>`.

```html
          <fieldset>
            <legend>Is your cat an indoor or outdoor cat?</legend>
            <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
            <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
            </fieldset>
          </fieldset>
```

#### **Step 51**
Agregamos un nuevo `<fieldset></fieldset>`.

#### **Step 52**
Agregamos una `<legend></legend>` al `<fieldset></fieldset>` anterior.

#### **Step 53**
Los formularios suelen utilizar casillas de verificación o "_checkboxes_" para preguntas que pueden tener más de una respuesta.
Para crear una casilla de verificación le debemos dar al `<input>` en su propiedad 'type' un valor de _checkbox_.

```html
            <legend>What's your cat's personality?</legend>
            <input type="checkbox"> Loving
```

#### **Step 54**
Agregamos al `<input>` anterior un 'id'.

#### **Step 55**
Hay otra manera de asociar **el texto de un `<input>`** con el propio elemento. Lo que podemos hacer, es anidar el texto dentro de un `<label>` y agregarle el atributo 'for' con el mismo valor que el atributo 'id' del `<input>`. 

```html
            <input id="loving" type="checkbox"> <label for="loving">Loving</label>
```

#### **Step 56**
Para asociar todos los `<input>` de 'type' _checkbox_ debemos darles a todos el mismo atributo 'name', así facilitaremos a los servidores procesar el formulario, espcialmente cuando hay varias casillas de verificación (No se notará el cambio en el navegador).

```html
            <input id="loving" type="checkbox" name="personality"> <label for="loving">Loving</label>
```

#### **Step 57**
Agregamos otra casilla de verifiación con otro 'id' y con el valor de 'name' igual que el anterior. Y agregamos otra `<label>` asociada con la nueva casilla de verificación mediante el atributo 'for'.

```html
            <input id="loving" name="personality" type="checkbox"> <label for="loving">Loving</label>
            <input id="lazy" name="personality" type="checkbox"> <label for="lazy">Lazy</label>
```

#### **Step 58**
Agregamos otra casilla de verifiación con otro 'id' y con el valor de 'name' igual que el anterior. Y agregamos otra `<label>` asociada con la nueva casilla de verificación mediante el atributo 'for'.

```html
            <input id="loving" name="personality"type="checkbox"> <label for="loving">Loving</label>
            <input id="lazy" name="personality" type="checkbox"> <label for="lazy">Lazy</label>
            <input id="energetic" name="personality" type="checkbox"> <label for="energetic"> Energetic </label>
```

#### **Step 59**
Al igual que los **botones de radio**, los datos extraidos de los formularios de tipo _checkbox_ son pares de atributos 'name'/'value'. Si bien el atributo 'value' es opcional, se recomienda incluirlo con las casillas de verificación y botones de radio. Además, es buena práctica ponerle a 'value' el mismo valor del 'id' del `<input>`.

```html
          <fieldset>
            <legend>Is your cat an indoor or outdoor cat?</legend>
            <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
            <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
          </fieldset>
          <fieldset>
            <legend>What's your cat's personality?</legend>
            <input id="loving" type="checkbox" name="personality" value="loving"> <label for="loving">Loving</label>
            <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
            <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic"> Energetic</label>
          </fieldset>
```

#### **Step 60**
Para marcar una **casilla de verificación** o un **botón de radio** de forma predeterminada, debemos agregarle el atributo 'checked'.

```html
          <fieldset>
            <legend>Is your cat an indoor or outdoor cat?</legend>
            <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
            <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
          </fieldset>
          <fieldset>
            <legend>What's your cat's personality?</legend>
            <input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving">Loving</label>
            <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
            <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic"> Energetic</label>
          </fieldset>
```

#### **Step 61**
Agregamos el `<footer></footer>` a la página.

```html
    </main>
    <footer>
      
    </footer>
  </body>
</html>
```

#### **Step 62**
Agregamos un `<p></p>` con información de Copyright.

```html
    <footer>
      <p>No Copyright - freeCodeCamp.org</p>
    </footer>
```

#### **Step 63**
Agregamos un enlace `<a></a>`.

```html
        No Copyright - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>

```

#### **Step 64**
Todos los elementos de la página que querramos que sean vistos por el usuario van dentro de las etiquetas `<body></body>`. Sin embargo, otra información importante va dentro del elemento `<head></head>`.

```html
  <head></head>
  <body>
    <h1>CatPhotoApp</h1>
    <main>
      <section>
        <h2>Cat Photos</h2>
        <!-- TODO: Add link to cat photos -->
        <p>Click here to view more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a>.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>
      <section>
        <h2>Cat Lists</h2>
        <h3>Things cats love:</h3>
        <ul>
          <li>cat nip</li>
          <li>laser pointers</li>
          <li>lasagna</li>
        </ul>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
          <figcaption>Cats <em>love</em> lasagna.</figcaption>  
        </figure>
        <h3>Top 3 things cats hate:</h3>
        <ol>
          <li>flea treatment</li>
          <li>thunder</li>
          <li>other cats</li>
        </ol>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Five cats looking around a field.">
          <figcaption>Cats <strong>hate</strong> other cats.</figcaption>  
        </figure>
      </section>
      <section>
        <h2>Cat Form</h2>
        <form action="https://freecatphotoapp.com/submit-cat-photo">
          <fieldset>
            <legend>Is your cat an indoor or outdoor cat?</legend>
            <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
            <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
          </fieldset>
          <fieldset>
            <legend>What's your cat's personality?</legend>
            <input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving">Loving</label>
            <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
            <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic">Energetic</label>
          </fieldset>
          <input type="text" name="catphotourl" placeholder="cat photo URL" required>
          <button type="submit">Submit</button>
        </form>
      </section>
    </main>
    <footer>
      <p>
        No Copyright - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>
      </p>
    </footer>
  </body>
```
***NOTA***: El `<head></head>` va por encima del `<body></body>`.

#### **Step 65**
El elemento `<title></title>` determina lo que los navegadores muestran en la barra de título o en la pestaña de la página.

```html
  <head>
    <title>CatPhotoApp</title>
  </head>
```

#### **Step 66**
Observemos que todo el contenido de la página esta anidado dentro de un elemento `<html></html>`, es decir que todos los demás elementos deben ser descendientes de este.
Al colocarle a la etiqueta `<html>` el atributo 'lang' con el valor _es_ le decimos que el idioma predeterminado de la página será el español.

```html
<html lang="es">
```
#### **Step 67**
Toda la página dee comenzar con `<!DOCTYPE html>`, que es una declaración que garantiza que el navegador cumpla con las especificaciones de la industria.

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <title>CatPhotoApp</title>
  </head>
```

### [CSS](https://www.freecodecamp.org/espanol/learn/2022/responsive-web-design/learn-basic-css-by-building-a-cafe-menu/step-1)

#### **Step 1**
Comenzamos la nueva página con los elementos `<!DOCTYPE html>` y `<html></html>`.

#### **Step 2**
Agregamos el `<head></head>`, y dentro un `<title></title>`.

#### **Step 3**
El `<title></title>` es uno de los elementos que brindan información adicional que no se ve en la página web, pero es útil para los motores de busqueda o para cómo se muestra la página.
Otro elemento del `<head></head>` es el `<meta>` que con el atributo 'charset' con un valor _utf-8_ le decimos cómo codificar los caracteres de la página. Los `<meta>` tienen cierre automático.

```html
  <head>
    <title>Cafe Menu</title>
    <meta charset="utf-8">
  </head>
```

#### **Step 4**
Agregamos el `<body></body>` debado del `<head></head>`.

#### **Step 5**
Agregamos el `<h1></h1>` a la página.

#### **Step 6**
Agregamos un `<p></p>` debajo del `<h1></h1>`.

#### **Step 7**
Anidamos los elementos `<h1></h1>` y `<p></p>` dentro del <header></header>.

```html
    <header>
      <h1>CAMPER CAFE</h1>
      <p>Est. 2020</p>
    </header>
```

#### **Step 8**
Agregamos el `<main></main>`.

```html
    <header>
      <h1>CAMPER CAFE</h1>
      <p>Est. 2020</p>
    </header>
    <main>
      
    </main>
```

#### **Step 9**
Agregamos una `<section></section>` dentro del `<main></main>`.

#### **Step 10**
Agregamos un `<h2></h2>` a la `<section></section>`.

#### **Step 11**
Hasta ahora, estuvimos limitados en cuanto a la presentación y apariencia del contenido (sólo estructuramos), para comenzar a controlar esto, agreguemos un elemento `<style></style>` en el `<head></head>`.

```html
  <head>
    <meta charset="utf-8" />
    <title>Cafe Menu</title>
    <style> <!-- Apertura -->
      
    </style> <!-- Cierre -->
  </head>
  <body>
    <header>
      <h1>CAMPER CAFE</h1>
      <p>Est. 2020</p>
    </header>
    <main>
      <section>
        <h2>Coffee</h2>
      </section>
    </main>
  </body>
```

#### **Step 12**
Podemos agregarle estilo a un elemento con `<style></style>`, de la siguiente forma:

```html
    elemento {
     propiedad: valor;
    }
```

```html
    <style>
      h1 {
        text-align: center;
      }
    </style>
```
***NOTA***: Centramos el texto del elemento `<h1></h1>` con la propiedad 'text-align' con el valor _center_.

#### **Step 13**
Alineamos también, hacia el centro, los elementos `<h2></h2>` y `<p><p>`.

```html
    <style>
      h1 {
        text-align: center;
      }
      h2 {
        text-align: center;
      }
      p {
        text-align: center;
      }
    </style>
```

#### **Step 14**
Como podemos ver, tenemos tres selectores (**`h1` `h2` `p`**) con el mismo estilo, entonces lo que podemos hacer, es agregar el mismo grupo de estilos a varios elementos al mismo tiempo creando una lista de selectores. Cada selector se separa con una coma (','):
```html
    selector1, selector2 {
      propiedad: valor;
    }
```

```html
    <style>
      h1, h2, p {
        text-align: center;
      }
    </style>
```

#### **Step 15**
Creamos un documento "styles.css" separado para darle estilo al archivo "index.html", y vamos a comenzar reeescribiendo los estilos ya definidos.

```css
h1, h2, p {
  text-align: center;
}
```
***NOTA**: Se coloca directamente en el documento "styles.css" sin las etiquetas `<style></style>`.

#### **Step 16**
Eliminamos el elemento `<style></style>` del documento "index.html".

#### **Step 17**
Ahora necesitamos vincular el archivo "styles.css" para que los estilos se apliquen nuevamente al "index.html". Lo vamos a hacer anidando un elemento `<link>` de cierre automático en el `<head></head>`.
El elemento `<link>` debe contener un atributo 'rel' con el valor _stylesheet_, un atributo 'type' con el valor _text/css_ y un atributo 'href' con el valor _styles.css_ (el nombre del documento que queremos vincular).

```html
  <head>
    <meta charset="utf-8" />
    <link rel="stylesheet" type="text/css" href="styles.css">
    <title>Cafe Menu</title>
  </head>
```

#### **Step 18**
Para que el estilo de la página se vea igual en un celular, tablet, notebook o computadora de escritorio, se debe agregar un `<meta>` con un conjunto de atributos: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`.

```html
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Cafe Menu</title>
    <link href="styles.css" rel="stylesheet" type="text/css" />
  </head>
```

#### **Step 19**
Le asignamos al **`body`** una propiedad 'background-color' la cual cambia el color de fondo del elemento seleccionado.

```css
h1, h2, p {
  text-align: center;
}

body {
  background-color: brown;
}
```

#### **Step 20**
Cambiamos el 'background-color' nuevamente del **`body`**.

#### **Step 21**
El elemento `<div></div>` se utiliza principalmente con fines de diseños.

```html
  <body>
    <div>
      <header>
        <h1>CAMPER CAFE</h1>
        <p>Est. 2020</p>
      </header>
      <main>
        <section>
          <h2>Coffee</h2>
        </section>
      </main>
    </div>
  </body>
```

#### **Step 22**
Lo que debemos lograr es que el **`div`** no ocupe todo el ancho ("_width_") de la página, justamente la propiedad 'width' de CSS se utiliza para esto.

```css
body {
  background-color: burlywood;
}

h1, h2, p {
  text-align: center;
}

div {
  width: 300px;
}
```

#### **Step 23**
Comentar en CSS se ve así:
```css
/* comente aquí */
```

#### **Step 24**
Colocamos la propiedad 'background-color', que previamente establecimos en el **`body`**, en el **`div`** con el mismo valor.

```css
div {
  width: 300px;
  background-color: burlywood;
}
```

#### **Step 25**
Actualmente, el ancho del **`div`** se especifica en píxeles (px), ahora lo vamos a cambiar a 80%, para que sea el 80% del ancho de su elemento principal o contenedor (en este caso el `<body></body>`).

```css
div {
  width: 80%;
  background-color: burlywood;
}
```

#### **Step 26**
Ahora vamos a centrar el **`div`** horizontalmente, modificando sus propiedades 'margin-left' y 'margin-right' y dandoles el valor _auto_.
Veamos al **margen** como un espacio invisible alrededor de un elemento, usando estas dos propiedades de margen, centra el elemento (horizontalemente) en el elemento principal o contenedro `<body></body>`.

```css
div {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
}
```

#### **Step 27**
Hasta ahora en CSS usamos el **selector** de ***tipo de elemento*** para asignar estilos a los mismos. Pero también existen los **selectores** de ***clases***, que se definen por un nombre con un punto delante ("**.**""), y previamente establecida la propiedad 'class' en el elemento:
```css
.nombre-clase {
  propiedad: valor;
}
```

```css
.menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
}
```
***NOTA***: Cambiamos el selector **`div`** por un **`.menu`**.

#### **Step 28**
Le asiganmos al elemento `<div></div>` en HTML el atributo 'class' y le asignamos el valor _menu_ que es el nombre de la clase que utilizamos en la hoja de estilo.

```html
    <div class="menu">
```

#### **Step 29**
Le asignamos al selector **`body`** una propiedad 'background-image' la cual cambia el fondo del elemento pero en este caso con una _imagen_ y no un color solido.

```css
body {
  background-image: url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg);
}
```
***NOTA***: Para esto el **valor** de la propiedad 'background-image' es la url de la imagen.

#### **Step 30**
Agregamos un elemento `<article></article>` abajo del `<h2></h2>`.

#### **Step 31**
Los elemento `<article></article>` comúnmente contienen elementos en su interior que tienen información relacionada.
Y agregamos 2 `<p></p>` dentro del <article></article>.

```html
          <article>
            <p>French Vanilla</p>
            <p>3.00</p>
          </article>
```

#### **Step 32**
Agregamos 4 `<article></article>` con 2 `<p></p>` cada uno.

```html
          <article>
            <p>French Vanilla</p>
            <p>3.00</p>
          </article>
          <article>
            <p>Caramel Macchiato</p>
            <p>3.75</p>
          </article>
          <article>
            <p>Pumpkin Spice</p>
            <p>3.50</p>
          </article>
          <article>
            <p>Hazelnut </p>
            <p>4.00</p>
          </article>
          <article>
            <p>Mocha </p>
            <p>4.50</p>
          </article>
```

#### **Step 33**
Le asignamos el atributo 'class' al primer `<p></p>` del primer `<article></article>`.

```html
            <p class="flavor">French Vanilla</p>
            <p>3.00</p>
```

**Step 34**
Le asignamos con el selector **`.flavor`** la propiedad 'text-align' con el valor _left_.

```css
.flavor {
  text-align: left;
}
```

#### **Step 35**
Le asignamos el atributo 'class' al segundo `<p></p>` del primer `<article></article>`.

```html
            <p class="price">3.00</p>
```

#### **Step 36**
Le asignamos con el selector **`.price`** la propiedad 'text-align' con el valor _right_.

```css
.price {
  text-align: right;
}
```

#### **Step 37**
Ya podemos visualizar que el "sabor" se encuentra a la izquierda y el "precio" a la derecha, pero en líneas distintas. Esto sucede porque los elementos `<p></p>` son **en bloque**, por lo que ocupa todo el ancho su contenedor.
Entonces, para poder colocar ambos elementos en la misma línea, debemos haer que se comporten como elementos **en línea**.
Primero, agregaremos un atributo 'class' con el valor _item_ en el primer `<article></article>`.

```html
          <h2>Coffee</h2>
          <article class="item">
            <p class="flavor">French Vanilla</p>
            <p class="price">3.00</p>
          </article>
```

#### **Step 38**
Los elementos `<p></p>` que queremos modificar están anidados dentro del `<article></article>` (su contenedor) que tiene 'class' _item_. Entonces, podremos darle estilo a todos los elementos `<p></p>` dentro `<article></article>` utilizando su 'class' seguida de un espacio y el nombre de los otros elementos a modificar.

```css
.item p { }
```

Así, usamos el selector **`.item p`** para darle estilo a todos los parrafos dentro de ese artículo y le asignamos la propiedad 'display' con el valor _inline-block_ para que los elementos se comporten más como elementos **en línea**.

```css
.item p {
  display: inline-block;
}
```

#### **Step 39**
Ya se encuentra un elemento al lado de otro, pero no están centrados. Debido a que los elementos **en línea** solo ocupan el ancho de su contenido.
Para solucionar esto, podemos colocarle a cada selector de parrafo (**`.flavor`**/**`.price`**) una propiedad 'width' con un valor de _50%_.

```css
.flavor {
  text-align: left;
  width: 50%;
}

.price {
  text-align: right;
  width: 50%;
}
```

#### **Step 40**
Pero sigue sin funcionar, porque al diseñar elementos `<p></p>` como **bloques en línea** y colocarlos en líneas separadas en el código, crea un espacio en el primer elemento, lo que hace que el segundo se desplace a la siguiente línea.
Una solución para esto es asignarle un 'width' a cada elemento menor a _50%_.

```css
.flavor {
  text-align: left;
  width: 49%;
}

.price {
  text-align: right;
  width: 49%;
}
```

#### **Step 41**
Ahora juntamos ambos `<p></p>` en la misma línea de código HTML.

#### **Step 42**
Y le asignamos nuevamente un 'width' del _50%_ a **`.flavor`** y **`.price`**.

#### **Step 43**
Le asignamos a todos los `<article></article>` la 'class' _item_.

#### **Step 44**
Colocamos en cada uno de los `<article></article>` dos `<p></p>` uno al lado del otro sin espacios.

#### **Step 45**
Le asignamos a cada par de `<p></p>` sus 'class' correspondientes (_flavor_ y _price_).

#### **Step 46**
Si reducimos el ancho de la página, en algún momento, parte del texto de la izquierda pasará a la siguiente línea. Debido a que el ancho de los `<p></p>` solo pueden ocupar el 50% del espacio.
Entonce debemos cambiar el valor del 'width' tanto de los **`.flavor`** como de los **`.price`**, y el de los últimos debe ser significativamente menor ya que como podemos observar ocupa menos espacio.

```css
.flavor {
  text-align: left;
  width: 75%;
}

.price {
  text-align: right;
  width: 25%;
}
```

#### **Step 47**
Agregamos una nueva `<section></section>`.

#### **Step 48**
Agregamos un `<h2></h2>` a la nueva sección.

#### **Step 49**
Agregamos un nuevo `<article></article>` con la 'class' nuevamente _item_.

#### **Step 50**
Agregamos 2 `<p></p>` dentro del `<article></article>`.

#### **Step 51**
Le agregamos a cada par de `<p></p>` las 'class' por un lado _dessert_ y por el otro _price_, respectivamente.

#### **Step 52**
Agregamos en CSS junto a **`.flavor`**, el selector **`.dessert`** separados por una coma, para que tome las mismas propiedades y valores.

#### **Step 53**
Creamos 3 `<article></article>` más, debajo del anterior, con 2 `<p></p>` cada uno.

#### **Step 54**
Podemos darle a **`.menu`** (el `<div></div>`) espacio entre su contenido y los lados, con las propiedades 'padding'.

```css
.menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
  padding-left: 20px;
  padding-right: 20px;
}
```
***NOTA***: Con 'padding-left' creamos un espacio entre el borde de su contenedor y el contenido de izquierda a derecha; y con 'padding-rigth' creamos un espacio entre el borde de su contenedor y el contenido de derecha a izquierda.


#### **Step 55**
Le damos al **`.menu`** 'padding-top' y 'padding-bottom'

```css
.menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
  padding-left: 20px;
  padding-right: 20px;
  padding-top: 20px;
  padding-bottom: 20px;
}
```
***NOTA***: Con 'padding-top' creamos un espacio entre el borde del contenedor y el contenido de arriba hacia abajo; y con 'padding-bottom' creamos un espacio entre el borde del contenedor y el contenido de abajo hacia arriba.

#### **Step 56**
Dado que los 4 lados del contenedor tiene el mimso espacio interno, eliminemos las cuatro propiedades y usemos una sola propiedad 'padding' (al ser un _shorthand_ abrevia las cuatro propiedades: top-right-bottom-left).

```css
.menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
  padding: 20px;
}
```

#### **Step 57**
El ancho actual del **`.menu`** es el 80% del ancho del `<body></body>` (su contenedor), en una pantalla muy ancha, por esto los tipos de café y postres aparecerán muy lejos de sus precios.
Para evitar esto usaremos la propiedad 'max-width' (ancho máximo) en el **`.menu`** para evitar que crezca demasiado.

```css
.menu {
  width: 80%;
  max-width: 500px;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
  padding: 20px;
}
```

#### **Step 58**
Podemos cambiar la fuente de texto con la propiedad 'font-family'.

```css
body {
  background-image: url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg);
  font-family: sans-serif;
}
```

#### **Step 59**
Cambiamos la 'font-family' de los **`.h1`** y **`.h2`**.

#### **Step 60**
Podemos agregar un valor alternativo para 'font-family' con otro nombre de fuente separado por una coma. Los respaldos o fuente alternativa, se utilizan cuando la establecida no se encuentra disponible.

```css
h1, h2 {
  font-family: Impact, serif;
}
```

#### **Step 61 / Step 62**
Le asignamos a `<p>Est. 2022</p>` una 'class' con el valor _established_, y le asignamos un 'font-style' con un valor _italic_. Con esta propiedad le asignamos un estilo a la fuente.

```html
      <header>
        <h1>CAMPER CAFE</h1>
        <p class="established ">Est. 2020</p>
      </header>
```

```css
.established {
  font-style: italic;
}
```

#### **Step 63**
La tipografía de los elementos de encabezado (h1, h2, h3...) se establecen según valores predeterminados por el navegador del usuario. Evitemos esto asignandole a los selectores de cada uno un 'font-size', propiedad encaragada del tamaño de la fuente.

```css
h1 {
  font-size: 40px
}

h2 {
  font-size: 30px;
}
```

#### **Step 64**
Le agregamos el `<footer></footer>` a la página.

#### **Step 65**
Agregamos un `<p></p>` con un `<a></a>` en el `<footer></footer>`.

```html
      <footer>
        <p><a href="https://www.freecodecamp.org">Visit our website</a></p>
      </footer>
```

#### **Step 66**
Agregamos otro `<p></p>` en el `<footer></footer>`.

#### **Step 67**
Podemos usar el elemento `<hr>` para mostrar un divisor entre secciones de diferente contenido. Se cierran automáticamente.
Agregamos un `<hr>` entre `<header></header>` y `<main></main>`.

#### **Step 68**
Por defecto, el elemento `<hr>` aparece como una línea delgada de color gris claro. Podemos cambiar el ancho de la línea especificando su 'height' en CSS.

#### **Step 69**
Cambiamos el 'background-color' del elemento `<hr>`.

**Step 70**
Todavia el contorno del `<hr>` sigue siendo gris claro aunque hayamos cambiado su 'background-color', ya que ese contorno se conoce como 'border' y es independiente. 
Le ponemos a los bordes del `<hr>` el mismo color que el fondo.

```css
hr {
  height: 3px;
  background-color: brown;
  border-color: brown;
}
```

#### **Step 71**
El valor predeterminado de la propiedad 'border-width' es _1px_ para todos los bordes del elemento `<hr>`. Al cambiar el borde al mismo color que el fondo, la altura total de la línea es de _5px_ (3px más el ancho del borde superior de 1px e inferior de 1px).

#### **Step 72**
Agregamos otro `<hr>` entre `<main></main>` y `<footer></footer>`.

**Step 73**
Vamos a darle más espacio alrededor del menú, agregandole 'padding' al **`body`**.

#### **Step 74**
Entre los elementos de "Coffee" y "Deserts", hay una distancia bastante grande entre cada línea. Para reducir esto establezcamos un 'margin-top' y un 'margín-bottom' menor a **`.item p`**.

#### **Step 75**
Le establecemos un 'font-size' a **`.item p`**.

#### **Step 76**
Creamos un clase **`.bottom-line`** con una propiedad 'margin-top' de _25px_, y la asignaremos para separar el último elemento de Desserts con el `<hr>` final.

#### **Step 77**
Le asignamos al segundo `<hr>` un 'class' con el valor _bottom-line_.

#### **Step 78**
Agregamos un comentario al final de CSS.

#### **Step 79**
Le asignamos un 'font-size' al `<footer></footer>`.

#### **Step 80**
El color predeterminado de un enlace al que todavía no se le dio click es azul, y el del que ya fue visitado suele ser violeta.
Para hacer que los enlaces tengan el mismo color independientemente de si se visitaron o no, usemos el selector y asignemosle un 'color'.

```css
a {
  color: black;
}
```

#### **Step 81**
Si queremos asignarle una propiedad cuando el sitio web sea visitado, usamos un pseudo-selector llamado **`...:visited`** luego del selector:
```css
a:visited {
  propiedad: valor;
}
```

```css
a:visited {
  color: grey;
}
```
***NOTA***: Si se visitó el sitio, el link se pondrá en gris.

#### **Step 82**
Si queremos cambiar las propiedades cuando el mouse pasa sobre el o los elementos, usamos un pseudo-selector llamado **`...:hover`** luego del selector:
```css
a:hover {
  propiedad: valor;
}
```

```css
a:hover {
  color: brown;
}
```

#### **Step 83**
Si queremos cambiar las propiedades de un enlace cuando se hace click en el elemento, usamos un pseudo-selecotr **`...:active`**:
```css
a:active {
  propiedad: valor;
}
```

```css
a:active {
  color:white;
}
```

#### **Step 84**
Cambiamos colores de los pseudo-selectores.

#### **Step 85**
El navegador tiene un margen superior predeterminado para el elemento **`h1`**. Se lo sacamos asignando en 'margin-top' con valor _0px_.

#### **Step 86**
También, le sacamos un poco de 'margin-bottom' al **`h1`** para que el texto de abajo este más pegado a él.

#### **Step 87**
Creamos una clase **`.address`** que se la vamos a asignar a un elemento para disminuir el espacio debajo del último `<p></p>` del HTML (colocando un 'margin-bottom'). 

#### **Step 88**
Le asignamos la clase al segundo elemento `<p></p>` del `<footer></footer>` con la supuesta dirección.

#### **Step 89**
Agregamos una imagen debajo de `<h2>Coffee</h2>`.

#### **Step 90**
Las `<img></img>` se comportan como elementos **en líne**. Para hacer que dicho elemento se comporte como un elemento **en bloque**, le asignaremos a través de su selector la propiedad 'display' con valor _block_ y luego para centrar horizontalmente su contenido le daremos un 'margin-left' y 'margin-right' _auto_.

```css
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
```

#### **Step 91**
Agregamos una imagen debajo de `<h2>Desserts</h2>`.

#### **Step 92**
Reduciremos el espacio entre los elementos `<h2></h2>` y sus íconos. Los elementos `<h2></h2>` tienen un espacio de 'margin' predeterminado, por lo que para solucionar esto podemos darle un valor de _0px_ al 'margin-bottom'.
Por otra parte, hay otra forma, que es agregandole un 'margin-top' negativo a los elementos `<img></img>` para sacarlos de sus posiciones actuales.

```css
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: -25px;
}
```

### Colores CSS 

#### **Step 1**
Iniciamos el nuevo "_index.html_" con el `<!DOCTYPE html>` y `<html></html>`.

#### **Step 2**
Agregamos el `<head></head>` y el `<body></body>`.

#### **Step 3**
Agregamos en el `<head></head>` el `<title></title>`.

#### **Step 4**
Agregamos el elemento `<meta>` en el `<head></head>` con el atributo 'charset' y un valor _utf-8_.

#### **Step 5**
Agregamos un `<meta>` en el `<head></head>` con los atributos 'name' y 'content', con los valores _viewport_ y _width=device-width, initial-scale=1.0_ respectivamente, para que la página se vea igual en todos los dispositivos.

#### **Step 6**
Agregamos un `<h1></h1>` en el `<body></body>`.

#### **Step 7**
Agregamos un elemento `<link>` con los atributos 'rel', 'type' y 'href' con los valors _stylesheet_, _text/css_ y _styles.css_ respectivamente, para aplicarle estilos al documento _index.html_.
 
#### **Step 8**
Alineamos el **`h1`** con 'text-align' _center_ en CSS.

#### **Step 9**
Dentro del `<body></body>` agregamos un `<div></div>` con 'class' _container_, debajo del `<h1></h1>`.

#### **Step 10**
Luego, dentro del `<div class="container"></div>` anidamos otro `<div></div>` con 'class' _marker_.

#### **Step 11**
Le damos a **`.marker`** una propiedad 'background-color' _red_.

#### **Step 12**
Le damos a **`.marker`** un 'width' (ancho) y un 'height' (alto) de _200px_ y _25px_, respectivamente.

#### **Step 13**
Utilizaremos el "_shorthand_" 'margin' para centrar el **`.marker`** en la página, dandole un valor _auto_.

```css
.marker {
  width: 200px;
  height: 25px;
  background-color: red;
  margin: auto;
}
```

#### **Step 14**
Agregamos dos `<div class="marker"></div>` dentro del `<div class="container"></div>`.

#### **Step 15**
Si no le damos ninguna propiedad más, se van a ver 3 marcadores pegados unos con otros. Para evitar esto vamos a darle un espacio entre ellos, para esto vamos a usar la propiedad 'margin' con 2 valores:
Cuando la propiedad 'margin' tiene solo dos valores, en un primer lugar se establece el 'margin-top' y 'margin-bottom' (en Y); y luego 'margin-left' y 'margin-right' (en X).

```css
.marker {
  width: 200px;
  height: 25px;
  background-color: red;
  margin: 10px auto;
}
```

#### **Step 16**
Los colores primarios (rojo, amarillo y azul) se utilizan para crear colores nuevos mezclandolos, pero en la informática este es un modelo obsoleto. Nosotros, para darle colores a los elementos en los dispositivos electrónicos usaremos el modelo aditivo RGB (Red-Green-Blue).

Dentro de una 'class' si separamos con un espacio y agregamos otra palabra le agregamos otra clase al mismo elemento.

```css
      <div class="marker one">
      </div>
      <div class="marker">
      </div>
      <div class="marker">
      </div>
```

#### **Step 17**
Eliminamos de **`.marker`** la propiedad 'background-color' y su valor.

**Step 18**
Con la nueva 'class' **`.one`** le asiganmos la propiedad 'background-color' _red_.

```css
.one {
  background-color: red;
}
```

#### **Step 19**
Le asignamos a los demás `<div class="marker"></div>` su otra clase respectivamente.

```html
      <div class="marker one">
      </div>
      <div class="marker two">
      </div>
      <div class="marker three">
      </div>
```

#### **Step 20**
Le asignamos a **`.two`** y **`.three`** la propiedad 'background-color' con los valores _green_ y _blue_.

```css
.two {
  background-color: green;
}
.three {
  background-color: blue;
}
```

#### **Step 21**
Como vimos anteriormente el modelo de color RGB es **aditivo**, es decir, que los colores comienzan en negro y cambian a medida que se introducen diferentes niveles de rojo, verde y azul.
Se utiliza la función **rgb(0, 0, 0)**.

```css
.container {
  background-color: rgb(0, 0, 0);
}
```

#### **Step 22**
Una **función** es una porción de código que puede tomar una entrada de datos y realizar una acción específica. La función **rgb()** acepta valores o argumentos para rojo, verde y azul, y produce un color: **rgb(red, green, blue)**.
Cada valor rojo, verde y azul es un número del 0 al 255. 0 significa que hay un 0% de ese color, y 255 significa que hay un 100% de ese color.

```css
.one {
  background-color: rgb(255,0,0);
}
```
***NOTA***: Cambiamos el _red_ por _rgb(255, 0, 0)_ que es exactamente el mismo color.

#### **Step 23**
Les cambiamos los colores a rgb a **`.two`** y **`.three`**.

#### **Step 24**
Mientras que los marcadores rojos y azul están exactamente igual, el verde es más claro. Esto se debe a que la palabra clave _green_ es un tono más oscuro y está en medio del negro y el valor máximo del verde.
Por esto disminuimos el verde a _127_.

#### **Step 25**
Agregamos espacio vertical entre los marcadores y el borde del elemento contenendor. Para esto usamos la _shorthand_ 'padding' para agregar 10px de relleno superior e inferior y 0px de relleno de izquierda y derecha. Funciona de la misma manera que 'margin'.

```css
.container {
  background-color: rgb(0, 0, 0);
  padding: 10px 0px;
}
  ```

#### **Step 26**
En el modelo RGB, los colores  RGB primarios son colores que, cuando los combinamos en su máxima intensidad crea un blanco puro.

#### **Step 27**
Cambiamos el 'background-color' del **`.container`** a blanco con _rgb (255, 255, 255)_.

#### **Step 28**
Cambiamos en el item **`.one`** el 'background-color' a amarillo (color **secundario**) _rgb (255, 255, 0)_.

#### **Step 29**
Cambiamos en el item **`.two`** el 'background-color' a cian (color **secundario**) con _rgb (0, 255, 255)_.

#### **Step 30**
Cambiamos en el item **`.three`** el 'background-color' a magenta (color **secundario**) con _rgb (255, 0, 255)_.

#### **Step 31**
Cambiamos en el item **`.one`** el 'background-color' a naranja (color **terciario**) con _rgb (255, 127, 0)_.

#### **Step 32**
Cambiamos en el item **`.two`** el 'background-color' a verde agua (color **terciario**) con _rgb (0, 255, 127)_.

#### **Step 33**
Cambiamos en el item **`.three`** el 'background-color' a violeta (color **terciario**) con _rgb (127, 0, 255)_.

#### **Step 34**
Hay 3 colores **terciarios** más "_chartreuse green_" (verde + amarillo), "_azure_" (azul + cian) y "_rose_" (rojo + magenta).

* "_chartreuse green_" → rgb (127, 255, 0); Un tipo de verde
* "_azure_" → rgb (0, 127, 255); Un tipo de azul
* "_rose_" → rgb (0, 127, 255); Rosa

#### **Step 35**
Ahora que ya vimos todos los colores **primarios** (rojo, verde y azul), los colores **secundarios** (amarillo, cian y magenta) y los **terciarios** (naranja, verde agua, violeta, _chartreuse green_, _azure_ y rosa) en una rueda de colores, será más fácil entender otros conceptos de teoría de color y cómo impactan en el diseño.
Primero, le damos a **`.one`**, **`.two`** y **`.three`** un 'background-color' con un valor _rgb (0, 0, 0)_ para que comience desde negro.

#### **Step 36**
Una rueda de colores es un círculo donde los colores o tonos similares están creca uno de otros y los diferentes más alejados. Por ejemplo, el rojo puro se encuentra entre las tonalidades rosa y naranja.
Dos colores que son opuestos en el círculo cromático se denominan **colores complementarios**, si se combinan ambos producen un gris. Pero cuando se colocan uno al lado del otro, se produce un fuerte contraste visual y parecen más brillantes.

#### **Step 37**
Si colocamos por ejemplo, un rojo junto con un cian, generara un contraste muy brillante. Este puede distraer si se usa demasiado en un sitio web y puede dificultar la lectura del texto se se coloca en un fondo de color complementario.
Es una mejor práctica elegir un color como el dominante y usar su color complementario como acento para llamar la atención sobre cierto contenido.

#### **Step 38**
Cambiamos el 'background-color' de **`.one`** y **`.two`** a _rgb(0,0,0)_ y _rgb(255,0,0)_.

#### **Step 39**
Volvemos a poner el 'background-color' de **`.two`** a negro.

#### **Step 40**
Le quitamos a **`h1`** su 'background-color'.

#### **Step 41**
Ahora vamos a agregar otros detalles a los marcadores, comenzando por cambiar la segunda 'class' _one_ a _red_.

#### **Step 42**
Cambiamos el **`.one`** por **`.red`** en CSS.

#### **Step 43**
Cambiamos el 'background-color' de **`.red`** por rojo puro en rgb().

#### **Step 44**
Luego, cambiamos la segunda de 'class' de _two_ a _green_ y de _three_ a _blue_.

#### **Step 45**
Cambiamos el **`.two`** por **`.green`** y el **`.three`** por **`.blue`** en CSS.

#### **Step 46**
Una forma muy común de aplicar color a un elemento en CSS es con valores **hexadecimales** o en hexadecimal. Estos valores de color comienzan con un caracter "#" y toman 6 caracteres del 0 al 9 y de la A a la F. El primer par de caracteres representa el **rojo**, el segundo al **verde** y el tercero al **azul**. Por ejemplo: #4B5323.

#### **Step 47**
El sistema **Hexadecimal** es un sistema de base 16:
0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | A | B | C | D | E | F
Con valor 00 es 0% de ese color y FF es 100%. Entonces #00FF00 se traduce como 0% **rojo**, 100% **verde** y 0% **azul**; es lo mismo que rgb(0,255,0).

#### **Step 48**
El modelo de color **HSL** (tono, saturación y luminosidad), es otra forma de representar colores.
La función **hsl** acepta 3 valores: un número de 0 a 360 para **tono**, un porcentaje de 0 a 100 para **saturación** y un porcentaje de 0 a 100 para **luminosidad**.
Si imaginamos una rueda de colores, el **tono** rojo esta a 0 grados, el verde a 120 grados y el azul a 240 grados.
La **saturación** es la intensidad de un color desde 0%, o gris, hasta %100, para un color puro.
La **luminosidad** es lo brillante que aparece un color, desde 0%, negro completo, hasta el 100%, blanco completo ó 50% neutral.

```css
.blue {
  background-color: hsl(240,100%,50%);
}
```
***NOTA***: Muestra el azul como rgb(0,0,255).

#### **Step 49**
Ya aprendimos formas de establecer colores planos, pero también podemos usar un **degradado**.
Un **degradado** es cuando un color pasa a otro, y con la función _linear-gradient()_ se controla la dirección del degradado a lo largo de una línea y qué colores se usan.
La función en realidad crea un elemento de imagen y generalmente se combina con una propiedad 'background' que puede aceptar una imagen como valor.

Cambiamos la propiedad 'background-color' de **`.red`** por solo 'background':
```css
.red {
  background: rgb(255, 0, 0);
}
```

#### **Step 50**
La función _linear-gradient()_ utiliza la siguiente sintaxis:
`linear-gradient(direcciónDegradado, color1, color2, ...);`
El primer argumento de la función 'direcciónDegradado' es la dirección de la línea usada para la transición; y 'color1'/'color2' son argumentos de color que se usarán para la transición (pueden ser de cualquier tipo color: hexadecimal, rgb o hsl).

Le asignamos al 'background' de **`.red`** una 'dirección de degradado' de _90deg_ (deg son grados).

```css
.red {
  background: linear-gradient(90deg);
}
```

#### **Step 51**

Le asignamos al 'background' de **`.red`** un primer color _rgb(255,0,0)_.

```css
.red {
  background: linear-gradient(90deg, rgb(255,0,0));
}
```
#### **Step 52**
Le asignamos al 'background' de **`.red`** un segundo color _rgb(0,255,0)_.

```css
.red {
  background: linear-gradient(90deg, rgb(255, 0, 0), rgb(0,255,0));
}
```
***NOTA***: Hará un efecto de degradado de rojo a verde.

#### **Step 53**
la función _linear-gradient_ necesita un mínimo de 2 colores, pero puede aceptar múltiples argumentos de color.

#### **Step 54**
Podemos asignar dónde se colocan los colores a lo largo de la línea de degradado. Son una unidad de longitud como px o porcentaje que siguen a un color en la función _linear-gradient()_.

```css
.red {
  background: linear-gradient(90deg, rgb(255, 0, 0) 75%, rgb(0, 255, 0), rgb(0, 0, 255));
}
```
***NOTA***: En este degradado rojo-verde-azul, la transición comienza en el punto del 75% a lo largo de la línea de degradado, por lo que el rojo ocupa la mayor parte del espacio.

#### **Step 55**
Le asignamos a **`.red`** _180deg_ de 'direcciónDegradado'.

#### **Step 56**
Le asignamos a cada color su parada:

```css
.red {
  background: linear-gradient(180deg, rgb(255, 0, 0) 0%, rgb(0, 255, 0)50%, rgb(0, 0, 255)100%);
}
```

#### **Step 57**
Vamos a darle tonos en los bordes superiores e inferiores del marcador que sean más oscuros, mientras que el del medio será más claro, como si hubiera una luz encima.
Comenzamos, dandole al primer argumento de color un valor rgb():

```css
.red {
  background: linear-gradient(180deg, rgb(122, 74, 14) 0%, rgb(0, 255, 0) 50%, rgb(0, 0, 255) 100%);
}
```

#### **Step 58**
En segundo lugar, le damos al segundo argumento de color otro valor rgb():

```css
.red {
  background: linear-gradient(180deg, rgb(122, 74, 14) 0%, rgb(245, 62, 113) 50%, rgb(0, 0, 255) 100%);
}
```

#### **Step 59**
Y por último, le damos al tercer argumento de color otro valor rgb():
```css
.red {
  background: linear-gradient(180deg, rgb(122, 74, 14) 0%, rgb(245, 62, 113) 50%, rgb(162, 27, 27) 100%);
}
```

#### **Step 60**
El marcador rojo ahora se ve más realista, vamos a seguir con el verde, cambiandole la propiedad 'background-color' por solo 'background'.

#### **Step 61**
Al marcador verde le asignamos dentro del 'background' un _linear-gradient_, con 180deg de dirección de degradado y el primer argumento de color con el valor _#55680D_. 

#### **Step 62**
Asignamos el segundo argumento de color _#71F53E_.

#### **Step 63**
Y asignamos el tercer y último argumento de color _#116C31_

#### **Step 64**
La función _linear-gradient()_ calcula automáticamente los valores y coloca los colores uniformemente a lo largo de la línea de degradado, es decir coloca automáticamente la parada de cada color, si no la asignamos manualmente.

#### **Step 65**
Si no especificamos ningún argumento de dirección de degradado a la función _linear-gradient()_, organiza los colores de arriba hacia abajo, o a lo largo de una línea de 180 grados.

#### **Step 66**
Ahora, cambiamos la propiedad 'background-color' por 'background' del **`.blue`**.

#### **Step 67**
Le asignamos la función _linear-gradient()_, y le asignamos el primer argumento de color en hsl().

#### **Step 68**
Le damos el segundo argumento de color hsl().

#### **Step 69**
y le damos el tercer y último argumento de color en hsl().

```css
.blue {
  background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
}
```

#### **Step 70**
Ahora que cada marcador tiene los colores correctos, vamos a darle un contorno a los mismos. Empecemos por el marcador _marker red_.
Dentro del `<div class="marker red"></div>` anidamos otro `<div></div>` con 'class' _sleeve_.

```html
      <div class="marker red">
        <div class="sleeve">

        </div>
      </div>
```

#### **Step 71**
Le asignamos al **`.sleeve`** un 'width' de _110px_ y un 'height' de _25px_.

#### **Step 72**
Al **`.sleeve`** le asignamos un 'background-color' con el valor _white_.

#### **Step 73**
Con la propiedad 'opacity', podemos controlar qué tan opaco o **transparente** es un elemento. Con el valor 0 o 0% el elemento es completamente transaparente, y con el valor 1 o 100%, el elemento será completamente opaco (valor por defecto).

```css
.sleeve {
  width: 110px;
  height: 25px;
  background-color: white;
  opacity: 0.5;
}
```

#### **Step 74**
Otra forma de establecer la opacidad es con el "canal alfa" (_alpha channel_), y se hace agrendolo dentro de las otras propiedades de color.

#### **Step 75**
Para agregarle un canal alfa a la función _rgb()_ ya vista, usaremos la misma función pero con una "a" al final: _rgba()_.
Funcionan iguales, pero la última toma un número más del 0 al 1 para el canal alfa:
`rgba(red, green, blue, alpha);`

```css
.sleeve {
  width: 110px;
  height: 25px;
  background-color: rgba(255, 255, 255, .5);
}
```

#### **Step 76**
Para mover el `<div class="sleeve"></div>` hacia la derecha creamos otro `<div class="cap"></div>` por encima.

```html
      <div class="marker red">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
``` 

#### **Step 77**
Le asignamos propiedades a **`.cap`**.

```css
.cap {
  width: 60px;
  height: 25px;
}
```

#### **Step 78**
Cuando aplicamos los cambios anteriores, parece que la manga o **`.sleeve`** desaparecio, pero no es así. Lo que sucedio es que su nuevo `<div class="cap"></div>` está ocupando todo el ancho del marcador y está empujando la manga hacia la línea siguiente debido a que la propiedad por defecto del 'display' de  los `<div></div>` es _block_, es decir, **elemento en bloque**. 
Entonces, cuando dos elementos en bloque están uno al lado del otro, se apilan.
Para colocar dos elementos `<div></div>` en la misma línea, le debemos cambiar su 'display' a _inline-block_ (bloque en línea).

```css
.sleeve, .cap {
  display: inline-block;
}
```

#### **Step 79**
Todos los elementos HTML tiene bordes, aunque no tienen ningún valor predeterminado. Con CSS, podemos controlar los aspectos de los bordes.

#### **Step 80**
Los bordes pueden ser una línea solida (solid), una línea discontinua (dashed) o una línea punteada (dotted), entre otros.

#### **Step 81**
Le establecemos un color al borde:

```css
.sleeve {
  width: 110px;
  height: 25px;
  background-color: rgba(255, 255, 255, 0.5);
  border-left-width: 10px;
  border-left-style: solid;
  border-left-color: black;
}
```

#### **Step 82**
El _shorthand_ 'border-left' permite establecer el ancho, estilo y color del borde izquierdo, todo al mismo tiempo:
`border-left: width style color;`

```css
.sleeve {
  width: 110px;
  height: 25px;
  background-color: rgba(255, 255, 255, 0.5);
  border-left: 10px solid black;
}
```

#### **Step 83**
Cambiamos el estilo de borde a _double_:

```css
.sleeve {
  width: 110px;
  height: 25px;
  background-color: rgba(255, 255, 255, 0.5);
  border-left: 10px double black;
}
```

#### **Step 84**
Asignamos un color en _rgba()_ para darle más transparencia al borde:

```css
.sleeve {
  width: 110px;
  height: 25px;
  background-color: rgba(255, 255, 255, 0.5);
  border-left: 10px double rgba(0, 0, 0, .75);
}
```

#### **Step 85**
Le agregamos `<div class="cap"></div>` y `<div class="sleeve"></div>` a los marcadores verde y azul.

```html
      <div class="marker red">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
      <div class="marker green">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
      <div class="marker blue">
        <div class="cap"></div>
        <div class="sleeve"></div>
      </div>
```

#### **Step 86**
Lo último que vamos a hacer es agregar una sombra a cada marcador. La propiedad 'box-shadow' permite aplicar una o más sombras alrededor de un elemento:
`box-shadow: desplazamientoEnX desplazamientoEnY color;`

```css
.red {
  background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
  box-shadow: 5px 5px red;
}
```
***NOTA***: Agregamos una sombra roja alrededor del marcador rojo que estará 5px a la derecha y 5px hacia abajo.

#### **Step 87**
Para que la sombra esta hacia arriba y a la izquierda debemos colocar sus valor de forma negativa (con un - adelante).

```css
.red {
  background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
  box-shadow: -5px -5px red;
}
```

#### **Step 88**
Observemos que la sombra es muy nítida, debido a que hay un valor de _blurRadius_ opcional para la propiedad 'box-shadow':
`box-shadow: desplazamientoEnX desplazamientoEnY blurRadius color;`
Si no se incluye un valor _blurRadius_, el valor predeterminado es 0, cuanto mayor sea, mayor será el efecto de desenfoque.

```css
.green {
  background: linear-gradient(#55680D, #71F53E, #116C31);
  box-shadow: 5px 5px 5px green;
}
```

#### **Step 89**
Si queremos expandir la sombra podemos hacerlo con el valor opcional _spreadRadius_:
`box-shadow: desplazamientoEnX desplazamientoEnY blurRadius spreadRadius color;`
Al igual que _blurRadius_, _spreadRadius_ tiene un valor por defecto de 0, si no está incluido.

```css
.blue {
  background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
  box-shadow: 0 0 0 5px blue;
}
```

#### **Step 90**
Ahora le colocamos un sombreado correcto al marcador rojo:

```css
.red {
  background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
  box-shadow: 0 0 20px 0 red;
}
```

#### **Step 91**
Le cambiamos el valor de color dentro del 'box-shadow' al marcador rojo:

```css
.red {
  background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
  box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);
}
```

#### **Step 92**
Le colocamos un sombreado correcto a los marcadores verde y azul (igual al del rojo).

#### **Step 93**
Le cambiamos el valor de color dentro del 'box-shadow' al marcador verde:

```css
.green {
  background: linear-gradient(#55680D, #71F53E, #116C31);
  box-shadow: 0 0 20px 0 #3B7E20CC;
}
```

#### **Step 94**
Le cambiamos el valor de color dentro del 'box-shadow' al marcador azul:

```css
.blue {
  background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
  box-shadow: 0 0 20px 0 hsla(223, 59%, 31%, 0.8);
}
```

### Formularios HTML

#### **Step 1**
Iniciamos el nuevo "_index.html_" con el `<!DOCTYPE html>`, para que el navegador sepa que tipo de documento está leyendo.

#### **Step 2**
Agregamos `<html></html>`.

#### **Step 3**
Agregamos el `<head></head>` y `<body></body>`.

#### **Step 4**
Agregamos un `<title></title>`, y un `<link rel="stylesheet" type="text/css" href="styles.css">` para vincular el "_index.html_" con el documento "_styles.css_", en el `<head></head>`.

#### **Step 5**
Agregamos un `<h1></h1>` en el `<body></body>`.

#### **Step 6**
Agregamos un `<p></p>`.

#### **Step 7**
Le damos al **`body`** un 'width' del _100%_ y un 'height' de _100vh_ para que ocupe todo el ancho y alto del display.

#### **Step 8**
Le sacamos el margen predeterminado al **`body`**, establecido por los navegadores con un 'margin' en _0_:

#### **Step 9**
Le agregamos al **`body`** un 'background-color' para establecer el color de fondo y un 'color' para darle un color a la letra.

#### **Step 10**
Agregamos un `<form></form>` con el atributo 'action'.

```html
  <body>
    <h1>Registration Form</h1>
    <p>Please fill out this form with the required information</p>
    <form action="https://register-demo.freecodecamp.org">
    
    </form>
  </body>
```

#### **Step 11**
Agregamos 3 `<fieldset></fieldset>` (conjunto de campos) dentro del `<form></form>`.

#### **Step 12**
Agregamos 4 `<label></label>` (etiqueta) en el primer `<fieldset></fieldset>`.

#### **Step 13**
Le asignamos texto a cada una de las `<label></label>`.

#### **Step 14**
De forma predeterminada los elementos `<label></label>` son **en línea**, pero para que aparezcan en líneas separadas, le damos al elemento **`label`** un 'display' _block_, y para separalos entre ellos le asignamos un 'margin'.

#### **Step 15**
Dentro de cada `<label></label>` anidamos un `<input>`, despúes del texto dentro de cada uno.

```html
      <fieldset>
        <label>Enter Your First Name: <input></label>
        <label>Enter Your Last Name: <input></label>
        <label>Enter Your Email: <input></label>
        <label>Create a New Password: <input></label>
      </fieldset>
```

#### **Step 16**
Especificar el atributo 'type' de los elementos del formulario dentro de los `<input>`, es importante para que el navegador sepa que tipo de dato esperar. Si no se especifica, el navegador utilizará el _text_ como predeterminado.

```html
      <fieldset>
        <label>Enter Your First Name: <input type="text"></label>
        <label>Enter Your Last Name: <input type="text"></label>
        <label>Enter Your Email: <input type="email"></label>
        <label>Create a New Password: <input type="password"></label>
      </fieldset>
```

#### **Step 17**
El `<input type="submit">` se configura para enviar el `<form></form>` más cercano.
Para manejar el envio del formulario, despues del último elemento de `<fieldset></fieldset>`, agregamos un `<input>` con el atributo 'type' y un valor _submit_ y un atributo 'value' también con el valor _submit_.

#### **Step 18**
Para que el formulario sea más interactivo, agregamos el atributo 'required' en los `<input>`. Ahora, si se intenta enviar el formulario sin completar los campos obligatorios (con 'required'), se mostrará un mensaje de error.

#### **Step 19**
Ciertos valores de atributo 'type' vienen con una validación de formulario integrada. Como `<input type="email"> que requiere que el valor sea una dirección de correo electrónico válida.
Otra puede ser, agregarle al `<input type="password">` un atributo 'minlength' con un valor de _8_, entonces evitamos que se envie la entrada con menos de 8 caracteres.

```html
        <label>Create a New Password: <input type="password" minlength="8" required></label>
```

#### **Step 20**
En `<input type="password">` podemos usar el atributo 'pattern' para definir una expresión regular que la contraseña debe coincidir para que se considere válida.

```html
        <label>Create a New Password: <input type="password" pattern="[a-z0-5]{8,}" required></label>
```
***NOTA***: La expresión regular _[a-z0-5]{8,}_ hace referencia a que la contraseña debe tener por lo menos 8 caracteres de letras minusculas o los dígitos del 0 al 5. 

#### **Step 21**
Agregamos 3 `<label></label>` dentro del segundo `<fieldset></fieldset>`.

#### **Step 22**
Agregamos a las dos primeras `<label></label>` un `<input type="radio">`.

#### **Step 23**
Agregamos al tercer `<label></label>` un `<input type="checkbox" required>`.

#### **Step 24**
Agregamos texto a cada `<label></label>`.

#### **Step 25**
En las **entrada de radio** queremos que se seleccione una sola opción, pero el formulario no sabe que estan relacionadas. Para relacionarlas, debemos darle el mismo atributo 'name'.

```html
      <fieldset>
        <label><input type="radio" name="account-type"/> Personal Account</label>
        <label><input type="radio" name="account-type"/> Business Account</label>
        <label><input type="checkbox" required /> I accept the terms and conditions</label>
      </fieldset>
```

#### **Step 26**
Creamos un vinculo alrededor de "terms and conditions".

#### **Step 27**
En el tercer y último `<fieldset></fieldset>` colocamos una `<label></label>` con texto y un `<input type="file">` para permitir que el usuario suba un archivo (en este supuesto caso una "foto de perfil").

```html
      <fieldset>
        <label>Upload a profile picture: <input type="file"></label>
      </fieldset>
```

#### **Step 28**
Luego de la primera etiqueta agregamos una segunda con texto e `<input type="number">`. Le asignaremos un 'min' y un 'max', para que no se pueda ingresar un número menor o mayor a los establecidos.

```html
      <fieldset>
        <label>Upload a profile picture: <input type="file" /></label>
        <label>Input your age (years): <input type="number" min="13" max="120"></label>
      </fieldset>
```

#### **Step 29**
Agregar un elemento desplegable al formulario se hace con un elemento `<select></select>`. Este elemento es un contenedor para un grupo de elementos `<option></option>`. Estos últimos actuan como una etiqueta para cada opción desplegable.
Agregamos un elemento `<select></select>` con 5 `<option></option>`.

```html
      <fieldset>
        <label>Upload a profile picture: <input type="file" /></label>
        <label>Input your age (years): <input type="number" min="13" max="120" /></label>
        <select>
          <option></option>
          <option></option>
          <option></option>
          <option></option>
          <option></option>
        </select>
      </fieldset>
```

#### **Step 30**
Anidamos todo el `<select></select>` dentro de un `<label></label>` con texto.

#### **Step 31**
Le agregamos texto a cada una de las `<option></option>`.

#### **Step 32**
Enviar el formulario con una `<option></option>` seleccionada no enviará un valor útil al servidor. Se le debe asignar a cada opción un atributo 'value'.

```html
      <fieldset>
        <label>Upload a profile picture: <input type="file" /></label>
        <label>Input your age (years): <input type="number" min="13" max="120" />
        </label>
        <label>How did you hear about us?
          <select>
            <option value="">(select one)</option>
            <option value="1">freeCodeCamp News</option>
            <option value="2">freeCodeCamp YouTube Channel</option>
            <option value="3">freeCodeCamp Forum</option>
            <option value="4">Other</option>
          </select>
        </label>
      </fieldset>
```

#### **Step 33**
El elemento `<textarea></textarea>` actúa como un elemento de entrada de texto, pero puede recibir texto de varias líneas.

#### **Step 34**
El `<textarea></textarea>` de forma predeterminada aparece muy chico, para darle un tamaño inicial podemos agregar los atributos 'rows' (filas) y 'cols' (columnas).

```html
        <label>Provide a bio:
          <textarea rows="3" cols="30"></textarea>
        </label>
```

#### **Step 35**
Para darle una idea a los usuarios que colocar dentro de la biografía, utilizaremos el atributo 'placeholder'. El mismo acepta un valor de texto, que se muestra hasta que el usuario empieza a escribir.

```html
        <label>Provide a bio:
          <textarea rows="3" cols="30" placeholder="I like coding on the beach..."></textarea>
        </label>
```

#### **Step 36**
Es buena práctica, que con los envios de formulario proporcionemos a cada elemento que se puede enviar un atributo 'name'. Este atributo se utiliza para identificar el elemento en el envio del formulario.

#### **Step 37**
Terminamos el HTML del formulario. Ahora vamos a darle un poco de estilo.
Comenzamos cambiandole al **`body`** su 'font-family' y 'font-size'.

#### **Step 38**
Tomamos los elementos **`h1`** y **`p`** y le asignamos un 'margin' y un 'text-align'.

#### **Step 39**
Le asignamos al **`form`** un 'max-width' un 'min-width' y un ancho general con 'width'.

#### **Step 40**
Le sacamos los bordes a los **`fieldset`** y le agregamos 'padding-bottom' y 'padding-top'.

```css
fieldset {
  border: none; /*Le sacamos los bordes*/
  padding: 2rem 0;
}
```

#### **Step 41**
Le asignamos a todos los **`fieldset`** un 'border-bottom', menos al último.

```css
fieldset:not(:last-of-type) {
  border-bottom: 3px solid #3B3B4F;
}
```
***NOTA***: Con la pseudo-clase **`...:not(:last-of-type)`** no incluimos el último elemento de la clase establecida antes del `:not`.

#### **Step 42**
Vamos a hacer que el texto de las `<label></label>` aparezca por encima de los elementos del formulario.
Para esto, tomaremos todos los elemento `<input>`, `<textarea></textarea>` y `<select></select>`, y haremos que ocupen todo el ancho de sus elementos principales.

```css
input, textarea, select {
  margin: 10px 0 0 0;
  width: 100%;
}
```

#### **Step 43**
Le agregamos a los `<input>` del segundo conjunto de campos (`<fieldset></fieldset>`) una 'class' _inline_. (Lo que queremos lograr es que en el segundo conjunto de campos es que los `<input>` y` <label></label>` aparezcan en la misma línea).

#### **Step 44**
Le asignamos a la clase **`.inline`** un 'width' con el valor _unset_, el cual elimina la regla anterior de 'width' _100%_.

#### **Step 45**
Le damos a **`.inline`** un margen derecho.

```css
.inline {
  width: unset;
  margin: 0 0.5em 0 0;
}
```

#### **Step 46**
Alineamos de forma vertical a los elementos **`.inline`** con la propiedad 'vertical-align' y asignandole un valor _middle_.

```css
.inline {
  width: unset;
  margin: 0 0.5em 0 0;
  vertical-align: middle;
}
```

#### **Step 47**
Le asignamos un 'background-color' y 'border' a los `<input>` y `<textarea></textarea>`.

#### **Step 48**
Le asignamos un 'color' y 'min-height' para la letra de los `<input>` y `<textarea></textarea>`.

```css
input, textarea {
  background-color: #0a0a23;
  border: 1px solid #0a0a23;
  color: #ffffff;
  min-height: 2em;
}
```

#### **Step 49**
Reasignamos el 'min-height' para que abarque tanto los `<input>`, `<textarea></textarea>` y `<select></select>`.

#### **Step 50**
Para darle estilo al `<button></button>`, podemos usar un **selector de atributos**, que selecciona un elemento en función del valor de un atributo:
`input[name="password"]`

***NOTA***: Selecciona elementos **input** con un valor de atributo de 'name' _password_.  

Le asignamos al `<input>` que contiene el botón "Submit" un 'display' y 'width'

```css
input[type="submit"] {
  display: block;
  width: 60%;
}
```

#### **Step 51**
Centramos el botón.

#### **Step 52**
Le asignamos al botón un 'height' y 'font-size'.

#### **Step 53**
Le asignamos un 'background-color' y un 'border-color'.

#### **Step 54**
Le modificamos el 'margin' para darle mayor margen arriba y abajo; y por otro lado le establecimos un ancho mínimo con 'min-width'.

```css
input[type="submit"] {
  display: block;
  width: 60%;
  margin: 1em auto 1em auto;
  height: 2em;
  font-size: 1.1rem;
  background-color: #3b3b4f;
  border-color: white;
  min-width: 300px;
}
```

#### **Step 55**
La mayoría de los navegadores establecen sus propias propiedades y valores CSS. Si observamos, podemos notar que los `<input>` de archivos (que no son texto) son más chicas que los otros. A los que se les introduce texto, tienen de forma predeterminada un 'padding' de _1px 2px_.
Entonces para solucionar esto, utilizando el **selector de atributos**, tomamos los **`input[type="file"]`**.

```css
input[type="file"] {
  padding: 1px 2px;
}
```

#### **Step 56**
Le agregamos _2em_ de 'padding-bottom' al botón "Submit"

#### **Step 57**
Le cambiamos el color al enlace de términos y condiciones.

### [Modelo de Cajas CSS](https://www.freecodecamp.org/espanol/learn/2022/responsive-web-design/learn-the-css-box-model-by-building-a-rothko-painting/step-1)

#### **Step 1**
Agregamos la estructura básica de `<hmtl></hmtl>` con su `<head></head>` y `<body></body>`, primeramente el `<!DOCTYPE html>`.

#### **Step 2**
Agregamos dentro del `<head></head>` un `<meta charset="utf-8">` y dentro del `<body></body>` una `<img>`.

#### **Step 3**
En el **modelo de cajas CSS**, cada elemento se trata como una **caja** con 4 áreas.
El contenido de la **caja** son elementos (encabezado, párrafo, imagen).

#### **Step 4**
El contenido de la caja, está rodeado por un espacio llamado **'padding'**, que lo separa de la caja que lo contiene, y luego tenemos el **'border'** que es el contorno de la caja misma.

#### **Step 5**
El **'margin'** es el área exterior de la caja y se puede utilizar para controlar el espacio entre otros elementos.

#### **Step 6**
Anidamos un `<div></div>` dentro del `<body></body>` con la 'class' _canvas_. Para establecer el "lienzo" o lugar donde nos vamos a desarrollar.

```html
  <body>
    <div class="canvas">
    </div>
  </body>
```

#### **Step 7**
Agregamos el `<link>` para darle estilo al documento hmtl.

```html
  <link rel="stylesheet" href="./styles.css">
```

#### **Step 8**
Le damos a la clase **`.canvas`** un 'width' de _500px_.

#### **Step 9**
Le damos a la clase **`.canvas`** un 'height' de _600px_.

#### **Step 10**
Le damos a la clase **`.canvas`** un 'background-color'.

#### **Step 11**
Anidamos el `<div class="canvas"></div>` dentro de otro `<div></div>` con 'class' _frame_.

```html
    <div class="frame">
      <div class="canvas"></div>
    </div>
```

#### **Step 12**
Le damos a la clase **`.frame`** un 'border' de _50px solid balck_.

#### **Step 13**
Le damos **`.frame`** un 'width' de _500px_.

#### **Step 14**
Le damos **`.frame`** un 'padding' de _50px_.

#### **Step 15**
Le damos a **`.frame`** un 'margin' de _20px auto_.

#### **Step 16**
Anidamos dentro del `<div class="canvas">` otro `<div></div>` con 'class' _one_.

```html
  <body>
    <div class="frame">
      <div class="canvas">
        <div class="one"></div>
      </div>
    </div>
  </body>
```

#### **Step 17**
Le damos a la clase **`.one`** un 'width' de _425px_.

#### **Step 18**
Le damos a **`.one`** un 'height' de _150px_.

#### **Step 19**
Le damos a  **`.one`** un 'background-color'.

#### **Step 20**
Le damos a **`.one`** un 'margin' de _20px auto_.

#### **Step 21**
Le damos a **`.canvas`** un 'padding' de _1px_.

#### **Step 22**
Para evitar que cambien las dimensiones de **`.canvas`**, ya que al agregarle un 'padding' aumenta el relleno arriba, a la derecha, hacia abajo y hacia la izquierda, eliminamos esta propiedad y en su lugar colocamos 'overflow' con el valor _hidden_. Esta propiedad de **desbordamiento oculto**, lo que hace es mantener las dimensiones originales del lienzo o **`.canvas`**

#### **Step 23**
Agregamos otro `<div></div>` dentro de `<div class="canvas">`, con 'class' _two_.

```html
    <div class="frame">
      <div class="canvas">
        <div class="one"></div>
        <div class="two"></div>
      </div>
    </div>
```

#### **Step 24**
Le damos al **`.two`** un 'width' de _475px_.

#### **Step 25**
Le damos al **`.two`** un 'height' de _200px_.

#### **Step 26**
Le damos al **`.two`** un 'background-color'.

#### **Step 27**
Le damos al **`.two`** un 'margin' con un valor _auto_.

#### **Step 28**
Agregamos un tercer `<div></div>` dentro de `<div class="canvas">`, con 'class' _three_.

```html
    <div class="frame">
      <div class="canvas">
        <div class="one"></div>
        <div class="two"></div>
        <div class="three"></div>
      </div>
    </div>
```

#### **Step 29**
Además de usar los píxeles para dimensionar un elemento, también podemos usar, por ejemplo, porcentajes.
Le damos al **`.three`** un 'width' con un valor del _91%_. 

#### **Step 30**
Le damos al **`.three`** un 'height' con un valor del _28%_. 

#### **Step 31**
Le damos al **`.three`** un 'background-color'. 

#### **Step 32**
Le damos al **`.three`** un 'margin' con un valor _auto_. 

#### **Step 33**
El margen inferior del elemento **`.one`** está empujando al elemento **`.two`** 20 píxeles hacia abajo.
Para solucionar esto, vamos a eliminar el margen superior, centrar horizontalmente y establecer el margen inferior en 20px de **`.two`**. Utilizando la propiedad 'margin'.

```css
.two {
  width: 475px;
  height: 200px;
  background-color: #8f0401;
  margin: 0 auto 20px auto; /* ← */
}
```

#### **Step 34**
Vamos a desenfocar la "pintura" con la propiedad 'filter' con un valor en _blur_ en el elemento **`.canvas`**.

```css
.canvas {
  width: 500px;
  height: 600px;
  background-color: #4d0f00;
  overflow: hidden;
  filter: blur(2px); /* ← */
}
```

#### **Step 35**
Aumentamos el desenfoque en los elementos **`.one`** y **`.two`**.

```css
.one, .two {
  filter: blur(1px);
}
```

#### **Step 36**
Aumentamos el desenfoque en **`three`**.

#### **Step 37**
Aumentamos el área y suavizamos los bordes de **`.one`** con 'box-shadow'.

```css
.one {
  width: 425px;
  height: 150px;
  background-color: #efb762;
  margin: 20px auto;
  box-shadow: 0 0 3px 3px #efb762; /* ← */
}
```

#### **Step 38**
Usamos los mismo valores del 'box-shadow' de **`.one`** para **`.two`**, sólo cambiando el color.

#### **Step 39**
Usamos los mismo valores del 'box-shadow' de **`.one`** y **`.two`**, para **`.three`**, sólo cambiando el color.

#### **Step 40**
Redondeamos cada esquina del elemento **`.one`**, usando la propiedad 'border-radius'.

```css
.one {
  width: 425px;
  height: 150px;
  background-color: #efb762;
  margin: 20px auto;
  box-shadow: 0 0 3px 3px #efb762;
  border-radius: 9px; /* ← */
}
```

#### **Step 41**
Usamos la propiedad 'border-radius' en **`.two`**.

#### **Step 42**
La propiedad 'border-radius' acepta cuatri valores para redondear: superior-izquierda, superior-derecha, inferior-derecha e inferior-izquierda, en ese orden.
Usamos la propiedad 'border-radius' en **`.three`**.

#### **Step 43**
Usamos la propiedad 'transform' con un valor _rotate_ para girar (en sentido contrario de las agujas del reloj) el elemento **`.one`**.

```css
.one {
  width: 425px;
  height: 150px;
  background-color: #efb762;
  margin: 20px auto;
  box-shadow: 0 0 3px 3px #efb762;
  border-radius: 9px;
  transform: rotate(-0.6deg); /* ← */
}
```

#### **Step 44**
Rotamos el elemento **`.two`** (a favor de las agujas del reloj).

```css
.two {
  width: 475px;
  height: 200px;
  background-color: #8f0401;
  margin: 0 auto 20px;
  box-shadow: 0 0 3px 3px #8f0401;
  border-radius: 8px 10px;
  transform: rotate(0.4deg) /* ← */
}
```

#### **Step 45**
Rotamos el elemento **`.three`** (en sentido anti-horario).

### [Flexbox CSS](https://www.freecodecamp.org/espanol/learn/2022/responsive-web-design/learn-css-flexbox-by-building-a-photo-gallery/step-1)

#### **Step 1**
Agregamos la estructura básica HTML comenzando con el `<!DOCTYPE html>` y continuando con el elemento `<hmtl></hmtl>` con su `<head></head>` y `<body></body>`.

#### **Step 2**
Agregamos dentro del `<head></head>` los elementos `<meta name="viewport" content="width=device-width, initial-scale=1">` y `<meta charset="utf-8">`.

#### **Step 3**
Agregamos dentro del `<head></head>` el `<title></title>` y `<link rel="stylesheet" type="text/css" href="styles.css">` para vincular el documento "_index.html_" con el "_styles.css_".

#### **Step 4**
Dentro del `<body></body>` creamos un `<div></div>` con 'class' con valor _header_ y dentro de este colocamos un `<h1></h1>`.

```html
  <body>
    <div class="header">
      <h1>CSS FLEXBOX PHOTO GALLERY</h1>
    </div>
  </body>
```

#### **Step 5**
Dentro del `<body></body>` y debajo del `<div class="header"></div>`, creamos un nuevo `<div></div>` con 'id' con valor _gallery_ y dentro de este colocamos diez elementos `<img>`.

#### **Step 6**
Le asignamos a cada `<img>` un 'src'.

#### **Step 7**
El asterisco (*) selecciona todo el contenido del documento al que le va a modificar su estilo.
Usamos la propiedad 'box-sizing con el valor _border-box_.

```css
* {
  box-sizing: border-box;
}
```

#### **Step 8**
Seleccionamos las imagenes con el selector **`#gallery img`**, le asignamos un 'width' del _25%_ y un 'height' de _300px_, para poder verlas.

```css
#gallery img {
  width: 25%;
  height: 300px;
}
```

#### **Step 9**
Le sacamos al **`body`** el margin y le asingnamos un 'font-family' y un 'background-color'.

#### **Step 10**
Alineamos el texto del **`.header`** hacia el centro, le agregamos un 'padding' y un 'background-color'.

#### **Step 11**
Flexbox es un tipo de diseño CSS que se centra en el flujo de contenido, nos ofrece la posibilidad de controlar la forma en que los elementos se esapcian y alinean dentro de un **contenedor**.
Para configurar un elemento para que sea una "caja flexible" (flexbox), le asignamos la propiedad 'display' con un valor _flex_. Le vamos a asignar dicha propiedad a **`#gallery`**

```css
#gallery {
  display: flex;
}
```

#### **Step 12**
Se puede decir que **flexbox** tiene dos ejes: el **eje principal** y el **eje transversal**. El **eje principal** está determinado por la propiedad 'flex-direction'. Si 'flex-direction' se establece en _row_ o _row-reverse_, el eje principal es **horizontal**; si 'flex-direction' se establece en _column_ o _column-reverse_, el eje principal es **vertical**.
Le damos **`#gallery`** un 'flex-direction' con un valor _row_.

```css
#gallery {
  display: flex;
  flex-direction: row;
}
```

#### **Step 13**
La propiedad 'flex-wrap' determina cómo se deben comportar los elementos cuando el flex container es muy chico. Establecer dicha propiedad con el valor _wrap_ permitirá que sus elementos se ajusten a la siguiente fila/columna (dependiendo de su eje principal), y si le asignamos _nowrap_ evitará que sus elementos se ajusten. Cuando se establece _nowrap_, los elementos pueden encogerse para ajustarse o desbordarse.
Le damos a **`#gallery`** un 'flex-wrap' con un valor _wrap_, lo que hace que se creen cuatro columnas dependiendo del 'width que le dimos.

```css
#gallery {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
```

#### **Step 14**
La propiedad 'justify-content' determina cómo se colocan los elementos dentro de un **contenedor flexible** a lo largo del eje principal, lo que afecta su posición y el espacio que lo rodea.
Le asignamos a **`#gallery`** la propiedad 'justify-content' con el valor _center_.

```css
#gallery {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}
```

#### **Step 15**
La propiedad 'align-items' posiciona el **contenido flexible** a lo largo del eje transversal. En este caso, con su 'flex-direction' establecida en _row_, su eje trasnversal será vertical.
Vamos a centrar vereticalmente las imágenes, dandole al selector **`#gallery`** una propiedad 'align-items' con el valor _center_.

```css
#gallery {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
}
```

#### **Step 16**
Le damos a **`#gallery`** un 'padding'.

#### **Step 17**
Podemos usar la propiedad 'object-fit' para determinar cómo deben comportarse las imágenes.
Vamos a asignarle a **`#gallery img`** la propiedad 'object-fit' con el valor _cover_, para indicarle a la imagen que llene el contenedor `<img>` mientras mantiene su relación de aspecto, que hará que se recorte para ajustarse.

```css
#gallery img {
  width: 25%;
  height: 300px;
  object-fit: cover;
}
```

#### **Step 18**
Vamos a darle un poco de espacio entre las imágenes dandole un 'margin-top' y un 'padding' a **`#gallery img`**.

#### **Step 19**
Redondeamos un poco los bordes de las imágenes con 'border-radius' con el selector **`#gallery img`**.

#### **Step 20**
Creamos una "consulta de medios" o **`@media`** con un 'max-width' de _800px_, y detro le creamos una regla **`#gallery img`** y le establecemos la propiedad 'width' del _50%_. Esto convertirá la galería en un diseño de dos columnas.

```css
@media (max-width: 800px) {
  #gallery img {
  width: 50%;
  }
}
```

#### **Step 21**
Por último, creemos otra "consultas de medio" para pantallas de menos de 600 píxeles de ancho. Dentro de ese **`@media`**, creamos la regla **`#gallery img`** y le establecemos la propiedad 'width' de un _100%_. Esto le dará a la galería un diseño de una sola columna, para pantalla menores de 600 píxeles.

```css
@media (max-width: 600px) {
  #gallery img {
    width: 100%;
  }
}
```

### [Tipografías](https://www.freecodecamp.org/espanol/learn/2022/responsive-web-design/learn-typography-by-building-a-nutrition-label/step-1)

#### **Step 1**
Ya con el modelo básico de HTML creado, le asignamos al `<body></body>` un `<h1></h1>`.

#### **Step 2**
En el `<body></body>` debajo del `<h1></h1>` creamos un `<p></p>`.

#### **Step 3**
En el `<body></body>` debajo del `<p></p>` anterior, creamos otro `<p></p>`.

#### **Step 4**
Dentro del <head></head> agregamos un elemento <link> con el atributo 'rel' con el valor _stylesheet_ y otro 'href' con el valor _https://fonts.googleapis.com/css?family=Open+Sans:400,700,800_. Esto último, importará la 'font-family' **Open Sans**, con los valores _400_, _700_ y _800_.
Por otra parte, agregamos el `<link>` que vincula al documento "_styles.css_".

```html
  <head>
    <meta charset="UTF-8">
    <title>Nutrition Label</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:400,700,800">
    <link rel="stylesheet" href="./styles.css">
  </head>
```

#### **Step 5**
Le asignamos al **`body`** la 'font-family' de _"Open Sans"_ con un respaldo de _sans-serif_.

```css
body {
  font-family: "Open Sans", sans-serif;
}
```
***NOTA***: Las fuentes con espacios deben colocarse entre comillas (" " ó ' '). 

#### **Step 6**
Le asignamos al selector **`hmtl`** un 'font-size'.

#### **Step 7**
Rodeamos los elementos `<h1></h1>` y ambos `<p></p>` con un `<div></div>` con un atributo 'class' con valor _label_.

#### **Step 8**
Le colocamos unos bordes al **`.label`**.

#### **Step 9**
Le asignamos un 'width' al **`.label`**.

#### **Step 10**
Le asignamos un 'margin' y 'padding' al **`.label`**.

#### **Step 11**
De forma predeterminada, el navegador incluye el borde y el relleno al determinar el tamaño de un elemento.
Para evitar esto, vamos a restablecer el modelo de caja, a través del selector **`*`** con la propiedad 'box-sizing' ("tamaño de caja") con un valor _border-box_ ("borde de caja").

```css
* {
  box-sizing: border-box;
}
```

#### **Step 12**
Le asignamos a **`h1`** la propiedad 'font-weight' para darle mayor **grosor** a la fuente.

```css
h1 {
  font-weight: 800;
}
```

#### **Step 13**
Le damos a **`h1`** un 'text-align' con un valor _center_.

#### **Step 14**
Le asignamos a **`h1`** un 'margin'.

#### **Step 15**
Le sacamos a **`p`** los 'margin'.

#### **Step 16**
Creamos un `<div></div>` con un atributo 'class' con un valor _divider_ y lo colocamos por debajo del `<h1></h1>`.

#### **Step 17**
Le asignamos a **`.divider`** un 'border-bottom' y un 'margin' para crear una línea divisoria, entre el título y los párrafos.

#### **Step 18**
La propiedad 'letter-spacing' se puede usar para ajustar el espacio entre cada carácter de texto en un elemento. Le asignamos un 'letter-spacing' a **`h1`**.

```css
h1 {
  font-weight: 800;
  text-align: center;
  margin: -4px 0;
  letter-spacing: 0.15px;
}
```

#### **Step 19**
Le asignamos el atributo 'class' con un valor _bold_ al segundo `<p></p>`, dentro del **`.label`**.

#### **Step 20**
Le asignamos al selector **`bold`** la propiedad 'font-weight' con un valor _800_ y le sacamos la misma propiedad a **`h1`**.

#### **Step 21**
Le asignamos el atributo 'class' con un valor _bold_ a `<h1></h1>`, y así tomará las propiedades de dicho selector.

#### **Step 22**
El espaciado horizontal entre elementos con la misma importancia puede aumentar la legibilidad de su texto. 
Rodeamos el texto "2/3 de taza (55g)" en un elemento `<span></span>` con un atributo 'class' y un valor _right_.

```html
    <div class="label">
      <h1 class="bold">Nutrition Facts</h1>
      <div class="divider"></div>
      <p>8 servings per container</p>
      <p class="bold">Serving size <span class="right">2/3 cup (55g)</span></p>
    </div>
```

#### **Step 23**
La propiedad 'float' se usa para colocar un elemento a la izquierda o derecha de su **contenedor**, permitiendo que otro contenido (como el texto) lo rodee.
Creamos el selector **`.right`** y le asignamos 'float' con un valor _right_.

```css
.right {
  float: right;
}
```

#### **Step 24**
Colocamos el `<header></header>` envolvinedo todo lo que se encuentra dentro del `<div class="label"></div>`.

```html
    <div class="label">
      <header>
        <h1 class="bold">Nutrition Facts</h1>
        <div class="divider"></div>
        <p>8 servings per container</p>
        <p class="bold">Serving size <span class="right">2/3 cup (55g)</span></p>
      </header>
    </div>
```

#### **Step 25**
Actualizamos el selector **`h1`** a **`header h1`**, para apuntar especificamente al **`h1`** dentro del encabezado.

#### **Step 26**
Creamos un nuevo `<div></div>` con un 'class' con valor _divider lg_, debajo del `<header></header>`.

#### **Step 27**
Le asignamos al nuevo selector **`.lg`** la propiedad 'height'. También creamos un selector **`.lg, .md`** y le asignamos un 'background-color'.

#### **Step 28**
Le asignamos al selector **`.lg, .md`** un 'border' con un valor _0_, para quitarle los bordes al elemento.

#### **Step 29**
Debajo del `<div class="divider lg"></div>`, creamos otro `<div></div>` con eñ atributo 'class' con un valor _calories-info_.

#### **Step 30**
Dentro del elemento **`.calories-info`** anidamos un <p></p> con un atributo 'class' con un valor _bold sm-text_.

#### **Step 31**
La unidad **rem** significa "_root em_", y es relativa al tamaño de la fuente del elemento html.
Le asignamos al selector **`.sm-text`** un 'font-size' de _0.85rem_ (que son aproximadamente 13,6 px, recordemos que configuramos el html para que tenga un 'font-size' de 16px).

#### **Step 32**
Debajo del elemento `<p class="bold sm-text"></p>` creamos un nuevo `<h1></h1>` con una parte de su texto rodeada por un `<span></span>` con una 'class' con un valor _right_.

#### **Step 33**
Asignamos con el selector **`.calories-info h1`** la propiedad 'margin'.

#### **Step 34**
Asignamos con el selector **`.calories-info span`** la propiedad 'font-size'.

#### **Step 35**
El tamaño de 'font-size' del número **230** hace que se desborde y se superponga el número al border del contenedor. Para evitar esto, le asignamos a **`.calories-info h1`** un 'overflow' (desbordamiento) con el valor _hidden_ (oculto).

#### **Step 36**
Le asignamos a **`.calories-info span`** un 'margin-top'.

#### **Step 37**
Creamos debajo del `<div class="calories-info"></div>` un nuevo `<div></div>` con el atributo 'class' con un valor _divider md_. 

#### **Step 38**
Le asignamos al selector **`.md`** un 'height'.

#### **Step 39**
Creamos debajo del `<div class="divider md"></div>` un nuevo `<div></div>` con un atributo 'class' con valor _daily-value sm-text_ y, dentro de este, creamos un nuevo `<p></p>` con una 'class' con un valor _right bold_. 

#### **Step 40**
El 'float' hace que el nuevo elemento `<p></p>` esté fuera del borde de la etiqueta. Colocamos un nuevo `<div class="divider"></div>` debajo del `<p class="right bold"></p>`.

#### **Step 41**
Le asignamos al selector **`.divider`** la propiedad 'clear' con un valor _right_, para borrar la propiedad 'float', empujando el divisor y cualquier contenido siguiente debajo del texto flotante.

```css
.divider {
  border-bottom: 1px solid #888989;
  margin: 2px 0;
  clear: right; /* Agregamos */
}
```

#### **Step 42**
Luego del elemento `<div class="divider"></div>` agregamos otro `<p></p>` con dos `<span></span>` seleccionando partes del texto.

```html
    <p><span class="bold">Total Fat</span> 8g <span class="bold right">10%</span></p>
```

#### **Step 43**
Luego del `<p></p>` anterior agregamos uno nuevo con `<span></span>` en una parte del texto.

#### **Step 44**
Le asignamos al `<p></p>` anterior, un atributo 'class' con un valor _indent_.

#### **Step 45**
Creamos el selector **`.indent`** y le asignamos un 'margin-left' para simular una sangría.

#### **Step 46**
Creamos el selector **`.daily-value p`** para apuntar a todos los elementos `<p></p>` dentro de la sección **`.daily-value`**; y le asignamos un 'border-bottom'.

#### **Step 47**
Le agregamos a dos `<p></p>` otra 'class'.

```html
      <div class="daily-value sm-text">
        <p class="right bold no-divider">% Daily Value *</p> <!-- no-divider -->
        <div class="divider"></div>
        <p><span class="bold">Total Fat</span> 8g<span class="bold right">10%</span></p>
        <p class="indent no-divider">Saturated Fat 1g <span class="bold right">5%</span></p>
      </div> <!-- no-divider -->
```

#### **Step 48**
El **pseudo-selector** **`...:not`** se usa para seleccionar todos los elementos que no coincidan con la regla CSS dada.

```css
div:not(#ejemplo) {
  color: red;
}
```  

Esto selecciona todos los elementos `<div></div>` sin un 'id' con valor _ejemplo_.  
Vamos a modificar el selector **`.daily-value p`** para que excluya los elementos **`.no-divider`**.

```css
.daily-value p:not(.no-divider) {
  border-bottom: 1px solid #888989;
}
```

#### **Step 49**
Vamos a crear otro `<div class="divider"></div>` debajo del segundo **`no-divider`**.

#### **Step 50**
Debajo del `<div class="divider"></div>` anterior, creamos un nuevo `<p></p>`.

```html
        <div class="divider"></div>
        <p class="indent no-divider"><i>Trans</i> Fat 0g</p>
```

#### **Step 51**
Vamos a crear otro `<div class="divider"></div>` debajo del `<p></p>` anterior.

#### **Step 52**
Creamos un nuevo `<p></p>` con un par de `<span></span>`.

```html
        <div class="divider"></div>
        <p><span class="bold">Cholesterol</span> 0mg <span class="bold right">0%</span></p>
```

#### **Step 53**
Creamos otro `<p></p>` con un par de `<span></span>`.

```html
        <p><span class="bold">Sodium</span> 160mg <span class="right bold">7%</span></p>
```

#### **Step 54**
Creamos otro `<p></p>` con un par de `<span></span>`.

```html
        <p><span class="bold">Total Carbohydrate</span> 37g <span class="right bold">13%</span></p>
```

#### **Step 55**
Creamos otro `<p></p>` pero con el atributo 'class' con un valor _indent no-divider_ y luego creamos otro `<div class="divider"></div>`.

#### **Step 56**
Creamos otro `<p></p>` con el atributo 'class' con un valor _indent no-divider_ y luego creamos otro `<div class="divider"></div>`.

#### **Step 57**
La ventaja de crear estos **divisores** es que podemos aplicarles clases específicas para diseñarlos individualmente. Agregamos _dbl-indent_ a la 'class' del último **`.divider`**.

#### **Step 58**
Creando el selector **`.dbl-indent`** le asignamos un 'margin-left' específico a dicho divisor.

#### **Step 59**
Creamos otro `<p></p>` pero con el atributo 'class' con un valor _dbl-indent no-divider_ y con una parte seleccionada por un `<span></span>`;  y luego creamos otro `<div class="divider"></div>`.

```html
        <p class="dbl-indent no-divider">Includes 10g Added Sugars <span class="right bold">20%</span></p>
        <div class="divider dbl-indent"></div>
```

#### **Step 60**
Creamos otro `<p></p>` pero solo con el atributo 'class' con un valor no-divider_ y con una parte seleccionada por un `<span></span>`;  y luego creamos otro `<div class="divider lg"></div>`.

#### **Step 61**
Luego agregamos otro `<p></p>` con solo una parte seleccionada por un `<span></span>`.

#### **Step 62**
Agregamos otros dos `<p></p>` con solo una parte seleccionada por un `<span></span>`.

#### **Step 63**
Agregamos otro `<p></p>` con solo una parte seleccionada por un `<span></span>`, pero al `<p></p>` le asignamos la 'class' con un valor _no-divider_.

#### **Step 64**
Creamos un divisor mediano con `<div class="divider md"></div>` y agregamos un `<p></p>` con un 'class' con valor _note_.

#### **Step 65**
Le asignamos a **`.note`** las propiedades 'font-size' y 'margin'.

#### **Step 66**
Le asignamos a **`.note`** las propiedades 'padding' y 'text-indent', esta última es para asignarle sangría al texto.

```css
.note {
  font-size: 0.6rem;
  margin: 5px 0;
  padding: 0 8px;
  text-indent: -8px;
}
```
### [Accesibilidad](https://www.freecodecamp.org/espanol/learn/2022/responsive-web-design/learn-accessibility-by-building-a-quiz/step-1)

#### **Step 1**
Creamos la estructura básica de un documento HTML.

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>

  </body>
</html>
```

#### **Step 2**
Asignamos un elemento `<meta>` con el atributo 'charset' con un valor _utf-8_, dentro del `<head></head>`.

#### **Step 3**
Agregamos el `<meta name="viewport" content="width=device-width, initial-scale=1">`  para que sea adaptable a otros dispositivos, dentro del `<head></head>`.

#### **Step 4**
Otro elemento `<meta>` importante para la accesibilidad y el SEO, es la definición de la **descripción**. Se utiliza el valor del atributo 'content' para proporcionar una descripción de la página.

```html
    <meta name="description" content="Proyecto de práctica del cuestionario de accesibilidad freeCodeCamp">
```

#### **Step 5**
Asignamos el `<title></title>` de la página, dentro del `<head></head>`

#### **Step 6**
La navegación es fundamental para la **accesibilidad**, y los lectores de pantalla dependen de nosotros para proporcionar la estructura de la página. Esto se logra con elementos HTML semánticos.
Agregamos los elementos `<header></header>` y `<main></main>`.
El elemento `<header></header>` o **encabezado**, se usa para presentar la página y proporcionar un menú de navegación.
El elemento `<main></main>` contendrá el contenido central de la página.

#### **Step 7**
Agregamos dentro del elemento `<header></header>` los elementos `<img>`, `<h1></h1>` y `<nav></nav>`. Además, le asignamos a la imagen un atributo 'id' con valor _logo_.

#### **Step 8**
Una propiedad útil de un SVG ("_Scalable Vector Graphics_" ó Gráficos Vectoriales Escalables) es que contiene un atributo 'path' que permite escalar la imagen sin afectar la resolución de la misma.
Actualmente, la imagen que colocamos toma su tamaño predeterminado, el cual es muy grande. Entonces, usando su 'id' como selector, vamos a configurar el ancho o 'width'.

```css
#logo {
	width: max(100px, 18vw);
}
```

#### **Step 9**
El **logotipo** debe conservar una relación de aspecto 35/4 y tener relleno alrededor del texto.
Dentro del selector **`#logo`** asignamos un 'bakcground-color', un 'aspect-ratio' con el valor _35 / 4_ para establecer la relación de aspecto, y un 'padding'.

```css
#logo {
  width: max(100px, 18vw);
	background-color: #0a0a23;
	aspect-ratio: 35 / 4;
	padding: 0.4rem;
}
```

#### **Step 10**
Vamos a hacer que el **encabezado** ocupe todo el ancho de su **contenedor principal**, establecerle un 'height', un 'background-color' y por último un 'display' para usar *flebox*.

```css
header {
	display: flex;
	width: 100%;
	height: 50px;
	background-color: #1b1b32; 
}
```

#### **Step 11**
Le asignamos a **`h1`** un 'color' para cambiar el color de la fuente y un 'font-size'.

#### **Step 12**
Para habilitar la navegación dentro de la página, vamos a agregar una **lista desordenada** con tres elementos (cada uno de estos elementos debe tener anidado un "anchor"). Todo esto va dentro de las etiquetas `<nav></nav>`.

```html
      <nav>
        <ul>
          <li><a>INFO</a></li>
          <li><a>HTML</a></li>
          <li><a>CSS</a></li>
        </ul>
      </nav>
```

#### **Step 13**
Apuntando a los elementos de lista desordenada dentro del elemento de navegación, vamos a darle un 'display' con el valor _flex_ y un 'justify-content' con  el valor _space-evenly_  para espaciar uniformemente los elementos. 

```css
nav > ul {
	display: flex;
	justify-content: space-evenly; 
}
```

#### **Step 14**
Como es un ***cuestionario***, necesitaremos un **formulario** para que los usuario envíen respuestas. Para separar semánticamente el contenido del formulario podemos usar elementos ``<section></section>`.
Entonces, dentro del `<main></main>` anidamos un `<form></form>` con tres `<section></section>`.
Luego con el atributo 'action' en `<form>` asignamos la url donde quremos enviar el formulario y le asignamos el método correcto con el atributo 'method' con un valor _post_.

```html
    <main>
      <form method="post" action="https://freecodecamp.org/practice-project/accessibility-quiz">
        <section></section>
        <section></section>
        <section></section>
      </form>
    </main>
```

#### **Step 15**
Para aumentar la accesibilidad de la página, el atributo 'role' se puede usar para indicar el proposito de un elemento para las tecnologías de asistencia. Este atributo forma parte de la "_Web Accessibility Initiative_" (WAI ó Iniciativa de Accesibilidad Web).
Le vamos a asignar a cada una de las `<section></section>` un 'role' con valor _region_.

```html
      <form method="post" action="https://freecodecamp.org/practice-project/accessibility-quiz">
        <section role="region"></section>
        <section role="region"></section>
        <section role="region"></section>
      </form>
```

#### **Step 16**
Cada atributo 'role' requiere de una etiqueta visible, a la que debe hacer referencia el atributo 'aria-labelledby'. A cada `<section></section>` le asignamos un 'aria-labelledby'. Luego, anidamos dentro de cada `<section></section>` un `<h2></h2>` con un valor de 'id' identico al del 'arial-labelledby' de la `<section></section>`.

```html
      <form method="post" action="https://freecodecamp.org/practice-project/accessibility-quiz">
        <section role="region" aria-labelledby="student-info">
          <h2 id="student-info">Student Info</h2>
        </section>
        <section role="region" aria-labelledby="html-questions">
          <h2 id="html-questions">HTML</h2>
        </section>
        <section role="region" aria-labelledby="css-questions">
          <h2 id="css-questions">CSS</h2>
        </section>
      </form>
```


#### **Step 17**
La tipografía es muy importante en la accesibilidad de una página. Vamos a cambiar las fuentes de los `<h1></h1>` y `<h2></h2>`, y a colocarle una fuente segura como alternativa. Además de agregarle a los `<h2></h2>` un 'border-bottom' para diferenciar las secciones.

#### **Step 18**
Para poder navegar dentro de la página, vamos a asignarles a cada elemento de anclaje (`<a></a>`) un 'href' con el mismo valor que el 'id' de los `<h2></h2>`.

```html
        <ul>
          <li><a href="#student-info">INFO</a></li>
          <li><a href="#html-questions">HTML</a></li>
          <li><a href="#css-questions">CSS</a></li>
			  </ul>
```

#### **Step 19**
Abajo del  primer `<h2></h2>` agregamos tres `<div></div>` con el atributo 'class' con un valor _info_. Dentro de cada `<div></div>` colocamos una `<label></label>` y debajo un `<input>`.

```html
        <section role="region" aria-labelledby="student-info">
          <h2 id="student-info">Student Info</h2>
          <div class="info">
            <label></label>
            <input>
          </div>
          <div class="info">
            <label></label>
            <input> 
          </div>
          <div class="info">
            <label></label>
            <input>
          </div>
        </section>
```

#### **Step 20**
Es importante vincular cada `<input>` con su `<label></label>` correspondiente. Esto le proporcionar a las tecnologías de asistencia una referencia visual a la entrada.
Esto se hace dandole al `<label></label>` un atributo 'for' con el mismo valor que el 'id' del `<input>`. Vamos a vincular los `<input>` con su `<label></label>` correspondiente dentro de **Student Info**.

```html
        <section role="region" aria-labelledby="student-info">
          <h2 id="student-info">Student Info</h2>
          <div class="info">
            <label for="student-name">Name:</label>
            <input id="student-name" />
          </div>
          <div class="info">
            <label for="student-email">Email:</label>
            <input id="student-email" />
          </div>
          <div class="info">
            <label for="birth-date">D.O.B.:</label>
            <input id="birth-date" />
          </div>
        </section>
```

#### **Step 21**
Es buena práctica asignarle a cada `<input>` un atributo 'type' y 'name' apropiadas. Además vamos a asignarle al primer `<input>` el atributo 'placeholder'.

#### **Step 22**
Aunque colocamos el atributo 'placeholder' en la etapa anterior, no es buena práctica ya que suele confundir. Vamos a confiar en que solo la `<label></label>` o etiqueta es la mejor práctica, y eliminaremos dicho atributo.

#### **Step 23**
Podriamos decir que "D.O.B" no es lo suficientemente descriptivo, y esto es especialmente correcto para los usuarios con discapacidad visual. Para evitar este problema, sin tener que agregar texto visible a la etiqueta, es agregar texto que sólo pueda leer un lector de pantalla.
Para esto, agregamos un elemento `<span></span>` con un 'class' con un valor _sr-only_ (después del "D.O.B." dentro del `<label></label>`).

```html
            <label for="birth-date">D.O.B.<span class="sr-only"></span></label>
```

#### **Step 24**
Dentro del elemento `<span></span>` colocamos "Date of Birth" entre parentesis.

```html
            <label for="birth-date">D.O.B.<span class="sr-only">(Date of Birth)</span></label>
```

#### **Step 25**
El texto de **`.sr-only`** es visible, podemos ocultarlos para que solo lo lean los lectores de pantalla. 
Este patrón es para establecer las siguientes propiedades CSS:

```css
position: absolute;
width: 1px;
height: 1px;
padding: 0;
margin: -1px;
overflow: hidden;
clip: rect(0, 0, 0, 0);
white-space: nowrap;
border: 0;
```

Se lo aplicamos a **`.sr-only`**.

#### **Step 26**
Dentro del segundo elemento `<section></section>` agregamos dos elementos `<div></div>` con un atributo 'class' con un valor _question-block_.
Luego dentro de cada `<div></div>` agregamos un elemento `<p></p>` con números de forma creciente, comenzando con el 1, y un `<fieldset></fieldset>` con 'class' con valor _question_.

```html
        <section role="region" aria-labelledby="html-questions">
          <h2 id="html-questions">HTML</h2>
          <div class="question-block">
            <p>1</p>
            <fieldset class="question"></fieldset>
          </div>
          <div class="question-block">
            <p>2</p>
            <fieldset class="question"></fieldset>
          </div>
        </section>
```

#### **Step 27**
Cada `<fieldset></fieldset>` contendrá una pregunta de verdadero/falso. Dentro de cada `<fieldset></fieldset>`, vamos a anidar un elemento `<legend></legend>` y un `<ul></ul>` con dos opciones.

#### **Step 28**
Le asignamos a cada `<fieldset></fieldset>` un atributo 'name' adecuado. Luego, le asignamos a cada lista desordenada el atributo 'class' con el valor _answers-list_.
Por último, le asignamos texto a `<legend></legend>`.

#### **Step 29**
Necesitamos crear un conjunto de inputs que no permitan seleccionar ambas respuestas al mismo tiempo.
Para esto, anidamos un elemento `<label></label>` dentro de cada elemento de la lista, y, a su vez, dentro de cada `<label></label>` anidamos un `<input>` con el 'type' adecuado (_radio_).

#### **Step 30**
Es buena práctica vincular una `<label></label>` con su elemento `<input>`. Esto se hace, como ya vimos, colocandole a la `<label></label>` un atributo 'for' con el mismo valor que el 'id' del `<input>` con el que lo queremos vincular.

#### **Step 31**
Asignamos texto a los elementos `<label></label>` de forma que el elemento `<input>` este antes. Y luego, asignamos a los `<input>` un atributo 'value' que coinsida con le texto.

#### **Step 32**
Vamos a evitar que se puedan seleccionar ambas entradas de radio colocandoles a ambas el mismo atributo 'name'.

#### **Step 33**
Para evitar repeticiones innecesarias, usaremos el pseudo-elemento **`...:before`** en el elemento **`p`** y le asignaremos una propiedad 'content' con el valor "_Question #"_.

```css
p:before {
	content: "Question #";
}
```

#### **Step 34**
La sección final del cuestionario tendrá un menú desplegable y un cuadro de texto.
Anidamos dentro de la última sección un `<div></div>` con un atributo 'class' con un valor _formrow_, y dentro de este anidamos cuatro `<div></div>` alternando los atributos 'class' con los valores _question-block_ y _answer_.

#### **Step 35**
Dentro de los elementos `<div class="question-block"></div>` anidamos una `<label></label>`.

#### **Step 36**
Dentro del primer elemento `<div class="answer></div>"`, anidamos un elemento `<select></select>` con tres `<option></option>`.

#### **Step 37**
Vinculamos la primera `<label></label>` con el `<select></select>` y le asignamos a este último un atributo 'name'.

#### **Step 38**
Anidamos un elemento `<textarea></textarea>` dentro del segundo elemento `<div class="answer"></div>`, y establecemos el número de filas y columnas que va a tener.

#### **Step 39**
Al igual que con los elementos `<input>` y `<label></label>`, vinculemos el `<textarea></textarea>` con su `<label></label>` correspondient y asignemosle un atributo 'name'.

#### **Step 40**
Le damos un botón de envio al cuestionario.

#### **Step 41**
Dos elementos finales de semánticas son el `<footer></footer>` y el `<address></address>`. El elemento de pie de página o `<footer></footer>` es un contenedor para un conjunto de contenido relacionado con la página, y el elemento `<address></address>` es un contenedor para la información de contacto del autor de la página.
Agregamos debajo del `<main></main>` el elemento `<footer></footer>` con un `<address></address>` anidado.

```html
    <footer>
      <address>

      </address>
    </footer>
```

#### **Step 42**
Le agregamos texto al `<address></address>`.

#### **Step 43**
Le agregamos a parte del texto dentro del `<address></address>` un _anchor_ o `<a></a>`.

#### **Step 44**
Seleccionamos los elemento de la lista del navegador con *`nav > ul > li`*, y le asignamos las propiedades: 'color', 'margin', 'padding' y 'display'.

#### **Step 45**
En la accesibilidad visual, el contraste entre elementos es un facto fundamental. Por ejemplo, el contraste entre el texto y el fondo de un encabezado debe ser de al menos **4,5:1**.
Vamos a cambiar el color de la fuente de todos los elementos _anchor_ dentro de los elementos de la lista a algo con un _contrast ratio_ de al menos 7:1, con la propiedad 'color' con el valor _inherit_.

```css
li > a {
  color: inherit;
}
```

***NOTA***: El selector **mayor qué** (símbolo: **>**) es utilizado en CSS para seleccionar todos los elementos que sean directamente descendientes de otro.

#### **Step 46**
Para que los botones de navegación se parezcan más a los típicos, vamos a eliminar el subrayado del _anchor_, con 'text-decoration' con el valor _none_.
Después, vamos a crear un selector dirigido a los elementos de la lista de navegación para que cuando el cursor se desplace sobre ellos, el color de fondo y el color del texto cambien, y el cursor se convierta en puntero (pointer).

```css
nav > ul > li:hover {
	background-color: #dfdfe2;
	color: #1b1b32;
	cursor: pointer;
}

li > a {
  color: inherit;
	text-decoration: none;
}
```

#### **Step 47**
Vamos a ordenar el **`header`** usando **flexbox** para dejar espacio entre los elementos secundarios ('justify-content' con el valor _space-between_) y centrandolos verticalmente ('align-items' con el valor _center_).
Después, fijamos el **`header`** en la parte superior de la ventana ('position' con el valor _fixed_).

```css
header {
  width: 100%;
	height: 50px;
	background-color: #1b1b32;
	display: flex;
	justify-content: space-between;
	align-items: center;
	position: fixed;
	top: 0;
}
```

#### **Step 48**
Cuando el ancho de la pantalla es pequeño, el **`h1`** no envuelve su contenido de texto como debería. Debemos alinear el elemento **`h1`** en el centro.
Después, le proporcionamos al **`main`** un 'padding' para que el encabezado de la sección **Student Info** se pueda ver.

```css
h1 {
  color: #f1be32;
	font-size: min(5vw, 1.2em);
  text-align: center;
}

main {
  padding-top: 50px;
}
```

#### **Step 49**
En pantallas pequeñas, la lista desordenada en la barra de navegación se desborda en el lado derecho de la pantalla.
Vamos a solucionar esto usando 'flex-wrap' con el valor _wrap_ sobre **`nav > ul`**. Después, vamos a configurar las siguientes propiedades CSS para alinear correctamente el texto:

```css
align-items: center;
padding-inline-start: 0;
margin-block: 0;
height: 100%;
```

```css
nav > ul {
  display: flex;
	justify-content: space-evenly;
  flex-wrap: wrap;
  align-items: center;
  padding-inline-start: 0;
  margin-block: 0;
  height: 100%;
}
```

#### **Step 50**
Establecemos el ancho de los elementos **`section`** al 80% de su contenedor principal. Después, usamos 'margin' para centrar los elementos de la **`section`** agregando 10px al margen inferior.
Además, nos aseguraremos de que los elementos de **`section`** no puedan tener más de 600px de ancho.

#### **Step 51**
Le asignamos a **`h2`** un 'margin-top' y un 'padding-top'.

#### **Step 52**
Le asignamos al selector **`.info`** un 'padding' superior e izquierdo.

#### **Step 53**
Le damos a **`.formrow`** un 'margin' y 'padding'. También le cambiamos el tamaño de la fuente a los **`input`**.

#### **Step 54**
Para que la primera sección se vea más en línea, primero vamos a apuntar solo a los elementos **`input`** dentro de los elementos **`.info`** con **`.info input`** y, luego, le vamos a dar un ancho de 50% y vamos a alinear su texto a la izquierda.

#### **Step 55**
Vamos a apuntar a todos los elementos **`label`** dentro del elemento **`.info`**, y le vamos a dar un ancho del 10% y que no ocupe menos de 55px (con 'min-width').

#### **Step 56**
Para alinear las cajas de los **`input`** entre sí hacia la derecha, vamos a establecerle la propiedad 'display' con un valor _inline-block_ para todos los **`input`** y **`label`** dentro de **`.info`**. 

```css
.info input, .info label {
 display: inline-block;
 text-align: right;
}
```

#### **Step 57**
Para mejorar los elementos **`.question-block`**, vamos a establecerle algunas propiedades:

```css
.question-block {
  text-align: left;
  display: block;
  width: 100%;
  margin-top: 20px;
  padding-top: 5px;
}
```

#### **Step 58**
Vamos a hacer que los párrafos aparezcan con mayor prioridad, con las siguientes propiedades: 
 
```css
p {
  margin-top: 5px;
  padding-left: 15px;
  font-size: 20px;
}
```

#### **Step 59**
Es útil ver el borde predeterminado alrededor del **`fieldset`**, durante el desarrollo, pero no queda muy bien después.
Retiramos el borde y el 'padding-bottom' de los elementos **`.question`**.

#### **Step 60**
Eliminamos el estilo predeterminado para los elementos de la lista de **`.answers-list`** con la propiedad 'list-style' con su valor en _none_, y removemos el 'padding' de la lista desordenada.

```css
.answers-list {
  list-style: none;
  padding: 0;
}
```

#### **Step 61**
Le damos al botón de envio un diseño con las siguientes propiedades:

```css
button {
  display: block;
  margin: 40px auto;
  width: 40%;
  padding: 15px;
  font-size: 23px;
  background: #d0d0d5;
  border: 3px solid #3b3b4f;
}
```

#### **Step 62**
Establceemos el 'background-color' del **`footer`** y usamos **flexbox** para centrar horizontalmente le texto.

#### **Step 63**
Seleccionamos el **`footer`** y el **`footer a`** y le asignamos un 'color' para que el texto se vea bien dentro del nuevo fondo.

#### **Step 64**
Centramos horizontalmente todo el texto dentro del elemento **`address`** y agregamos un poco de 'padding'.

#### **Step 65**
Al hacer clic en los enlace, la ventana de visualización debería saltar a la sección correspondiente. Éste salto podría desorientar a algunos usuarios.
Seleccionamos todos los elementos y establecemos la propiedad 'scroll-behavior' con el valor _smooth_, lo que producirá el efecto de bajar más lento.

```css
* {
  scroll-behavior: smooth;
}
```

#### **Step 66**
La regla **`@media`** tiene una función llamada _prefers-reduce-motion_ para establecer el movimiento, y puede tomar los valores:
* _reduce_.
* _no-preference_.

```css
@media (característica: valor) {
  selector {
    estilo
  }
}
```

Colocamos la regla 'scroll-behavior: smooth;' dentro de una regla **`@media`** con la función de _prefers-reduce-motion_ con _no-preference_ como valor.

```css
@media (prefers-reduced-motion: no-preference){
  * {
    scroll-behavior: smooth;
  }
}
```

#### **Step 67**
Finalmente, la accesibilidad de la navegación se puede mejorar proporcionando **atajos de teclado**.
El atributo 'accesskey' acepta una lista de claves de acceso separadas por espacios: 

```html
<button type="submit" accesskey="s">Submit</button>
```

Asignale a cada enlace de navegación una clave de acceso de una letra.

```html
        <ul>
          <li><a href="#student-info" accesskey="i">INFO</a></li>
          <li><a href="#html-questions" accesskey="h">HTML</a></li>
          <li><a href="#css-questions" accesskey="c">CSS</a></li>
        </ul>
```
