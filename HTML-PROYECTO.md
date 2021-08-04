
# html

HTML5 provee bàsicamente tres caracteristicas: estructura, estilo y funcionalidad. Es considerado el producto de la convinaciòn de HTML, CSS y JavaScript. Estas tecnologias son altamente dependientes y actuan como una sola unidad organizada bajo la especificaciòn de HTML5.
Mas allà de la integraciòn, laestructura sigue siendo parte esencial de un documento. La misma provee los elementos necesarios para ubicar contenido estàtico o dinàmico, y es tambièn una plataforma bàsica para aplicaciones. Debido a la variedad de dispositivos y la diversidad de interfaces que interactuan con la web, se vuelve vital un aspecto como la estructura en el documento, la misma debe proveer forma, organizacion y flexibilidad.
ESTRUCTURA GLOBAL 
Los documentos HTML se encuentran estrictamente organizados. Cada parte està diferenciada, declarada y determinada por etiquetas especìficas. 
<kbd>< !DOCTYPE ></kbd>
Primero indicamos el tipo de documento que vamos a crear

#### < !DOCTYPE html >

Esta lìnea debe ser la primera del archivo, sin espacios o lìneas que le precedan, para que el modo estandar del navegador sea activado y las incorporaciones de HTML5 sean interpretadas siempre que sea posible.

#### < html >

La estructura tipo àrbol de este lenjuage de marcado tiene su raìz en este elemento mencionado, el cual envolverà el resto del còdigo.

	<!DOCTYPE html>
	<html lang="es">
	</html>

El atributo <code>lang</code> en la etiqueta de apertura <kbd>< html ></kbd> es el ùnico que necesitamos especificar en HTML5, el mismo define el idioma del contenido del documento que estamos creando, el cual en este caso tiene como valor <code>es</code>

#### < head >

El codigo HTML insertado entra las etiquetas <kbd>< html ></kbd> tiene que ser dividido entre dos secciones principales <kbd>< head ></kbd> y <kbd>< body ></kbd>. El elemento <kbd>< head ></kbd> va primero

	<!DOCTYPE html>
	<html lang="es">
	<head>
	</head>
	</html>

Dentro de <kbd><  head ></kbd> definiremos el tìtulo de nuestra pàgina web, declararemos el set de caracteres correspondiente, proveeremos informaciòn general acerca del documento e incorporaremos los archivos externos con estilo, còdigos JavaScript o incluso imàgenes para generar la pàgina en la pantalla

#### < body >

Es el cuerpo que representa la parte visible de todo documento.

	<!DOCTYPE html>
	<html lang="es">
	<head>
	</head>
	<body>
	</body>
	</html>

Hasta el momento tenemos un còdigo simple pero con una estructura compleja, porque el còdigo HTML no està formado por un conjunto de instrucciones secuenciales. Es un lenjuage de marcado, de etiquetas, un listado de elementos que usualmente se utilizan en paresm y que pueden ser anidados.

#### < meta >

Es la etiqueta que define el juego de caracteres a utilizar para mostrar el documento, la que especifica còmo el texto serà presentado en pantalla. La misma se ubica dentro de <kbd>< head >< /head ></kbd>

	<!DOCTYPE html>
	<html lang="es">
	<head>
		<meta charset="iso-8859-1">
	</head>
	<body>
	</body>
	</html>

Podemos cambiar el tipo "iso-8859-1-" por el necesario para nuestro documento, tambien agragar otras etiquetas <kbd>< meta ></kbd> como <code>description</code> o <code>keywords</code>  para definir otros aspectos de la pàgina web.

	<!DOCTYPE html>
	<html lang="es">
	<head>
		<meta charset="iso-8859-1" />
		<meta name="description" content="ejemplo de HTML" />
		<meta name="keywords" content="HTML5, CSS3, JavaScript" />
	</head>
	<body>
	</body>
	</html>

#### < title >

Especifica el tìtulo del documento. Normalmente este texto es mostrado en la barra superior de la ventana del navegador.

	<!DOCTYPE html>
	<html lang="es">
	<head>
	 	<meta charset="iso-8859-1" />
	 	<meta name="description" content="Ejemplo de HTML5" />
	 	<meta name="keywords" content="HTML5, CSS3, JavaScript" />
	 	<title>Este texto es el título del documento</title>
	</head>
	<body>
	</body>
	</html>


#### < link >

Este elemento es usado para incorporar estilo, còdigos JavaScript, imàgenes o iconos desde archivos externos.

	<!DOCTYPE html>
	<html lang="es">
	<head>
		<meta charset="iso-8859-1"/>
		<meta name="description" content="Ejemplo de HTML" />
		<meta name="keywords" content="HTML, CSS3, JavaScript" />
		<title>Este texto es el tìtulo del documento</title>
		<link rel="stylesheet" href="misestilos.css" />
	</head>
	<body>
	</body>
	</html>

En HTML5 no se necesita especificar que tipo de estilos estamos insertando, por lo que el atributo "type" fue eliminado. Solo se necesitan el atributo "rel" y "href" para incorporar archivos de estilo. "rel" significa "relacion", la que existe entre el documento y el archivo que estamos incorporando por medio de "href". En el còdigo anterior "rel" tiene el valor "stylesheet" el cual le informa al navegador que el archivo "misestilos.css" es un archivo CSS con estilo requeridos para presentar la pàgina en pantalla.
Un archivo de CSS es un grupo de reglas de formato que ayudan a cambiar la apariencia de nuestra pàgina web. Sin estas reglas, el texto y cualquier otro elemento HTML seria mostrado en pantalla utilizando los estilos estàndar provistos por el navegador. Los estilos son reglas que normalmente solo son unas pocas lineas de còdigo y pueden ser declarados en el mismo documento. No es estrictamente necesario el vincular con archivos externo, pero es una pràctica recomendada. Cargar las reglas CSS desde un documento externo nos permite organizar el documento principal, incrementar la velocidad de carga y aprovechar nuevas caracteristicas de HTML5
ESTRUCTURA DEL CUERPO body

#### < header >

Provee información introductoria(títulos, subtítulos, logos) y es usado solo para el cuerpo o secciones específicas dentro del cuerpo.

	<!DOCTYPE html>
	<html lang="es">
	<head>
		<meta charset="iso-8859-1" />
		<meta name="description" content="Ejemplo de HTML5" />
		<meta name="keywords" content="HTML, CSS3, JavaScript" />
		<title>Este texto es el título del documento</title>
		<link rel="stylesheet" href="misestilos.css" />
	</head>
	<body>
		<header>
			<h1>Este es el título principal del documento</h1>
		</header>
	</body>
	</html>

El elemento <code>< h1 ></code> es un viejo elemento HTML usado para definir títulos. El número indica la importancia del título. Elelemento <kbd>< h1 ></kbd> es el más importante y <kbd>< h6 ></kbd> el de menor importancia, por lotanto <kbd>< h1 ></kbd> será utilizado para mostrar el título principal y los demás para subtítulos o subtítulos <samp>internos</samp>

##### nav[^1]

Es la etiqueta que representa  a la barra de navegación.

	<!DOCTYPE html>
	<html lang="es">
	<head>
		<meta charset="iso-8859-1" />
		<meta name="description content="Ejemplo de HTML5" />
		<meta name="keywords" content="HTML5, CSS3, JavaScript" />
		<title>Este texto es el título del documento</title>
		<link rel="stylesheet" href="misestilos.css" />
	</head>
	<body>
		<header>
			<h1>Este es el título principal del sitio web<h1>
		</header>
		<nav>
			<ul>
				<li>Principal</li>
				<li>Fotos</li>
				<li>Videos</li>
				<li>Contacto</li>
			</ul>
		</nav>
	</body>
	</html>



> Texto de marcado tipo cita

=H ~ 2 ~ O es líquido=

[^1]: Etiqueta nav

[![](rgmauri00@gmail.com)](http://www.gmail.com)


