# CVV con HTML y CSS
En esta practica fue realizada a través de un editor de texto llamado Sublime Text 3, para poder llevarla acabo no es necesario tener amplios conocimientos en estas diciplinas, basta con saber lo básico y lo más importante, a continuacion dejaré muestras del contenido de la practica.

Empezamos con html, abrimos nuestro editor de texto y guardamos con la extencion *.html* hecho esto ocupamos el siguiete codigo.



![](https://mir-s3-cdn-cf.behance.net/project_modules/disp/4850de49604597.5608607aaab6c.png)






```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="author" content="Demetrio Emmanuel Martinez Gaspar">
    <meta name="desciption" content="Soy estudiante del Instituto Tecnologico de Pochutla">
    <meta name="keywords" content="">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Portafolio</title>
```
Esta sintaxis es para añadir una fuente externa a nuestra página web.
```
    <link href="https://fonts.googleapis.com/css2?family=Tinos:wght@700&display=swap" rel="stylesheet">
```

Aquí cargamos los estilos que hemos desarrollado en css usamos un *href* y la ubicación de los archivos.
```
  
    <link rel="stylesheet" href="css/animacion.css">
    <link rel="stylesheet" href="css/estilos.css">

</head>
<body style="background-color:rgb(255,255,255);">



    <header>

        <h1 class="title">Demetrio Emmanuel Martinez Gaspar</h1>

    </header>
   
    <main>

     
        
        <section class="miinfo">
            

            <div class="informacion">
                <img src="recursos/datos/calendario.png" alt="nacimiento">
                <p class="title">Fecha de nacimiento</p>
                <p class="desc">28 de abril de 1999</p>
            </div>

            <div class="informacion">
                <img src="recursos/datos/mapa.png" alt="lugar">
                <p class="title">Domicilio</p>
                <p class="desc">Puerto Escondido Oaxaca, México</a></p>
            </div>
            
            <div class="informacion">
                <img src="recursos/datos/estudio2.png" alt="eduación">
                <p class="title">Grado de estudios</p>
                <p class="desc">Universidad en Instituo Tecnológico de Pochutla</p>
            </div>
            
            <div class="informacion">
                <img src="recursos/datos/estudiante2.png" alt="ocupacion">
                <p class="title">Ocupación actual</p>
                <p class="desc">Estudiante</p>
            </div>

```
En este primer apartado debemos escribir el esquema básico que tendrá nuestra página, declaramos los diferentes titulos,  clases e imagenes que ocuparemos.


Después creamos un nuevo archivo en nuestro editor al cual llamaremos como queramos pero con la extención *.css* ya que aquí escribiremos los efectos y animaciones asi también como el formato que tendrá la página de nuestro CVV.






![](https://seeklogo.com/images/C/css3-logo-FD8D698B77-seeklogo.com.png)



Con este primer apartado definimos las caracteristicas generales de nuestra ventana.
```CSS
*{
    margin: 5;
    padding: 10;
    box-sizing: border-box;

    font-size: 20;
    font-family: 'Tinos';
    font-weight: 400;
}
```

Aqui definimos lo que viene siendo las especificaciones de la imgen que tendremos como fondo.
```
img{
    vertical-align: top;
}
a{
    text-decoration: none;
}
s

body{
    overflow-x: hidden;
}


header{
    width: 100%;
    height: 100vh;
    overflow: hidden;
    padding: 25vh 0;

    background: url('../recursos/img/fondo5.jpg');
    background-position: center;
    background-size: cover;
    background-repeat: repeat;
    background-attachment: fixed;

    animation: in ;
    animation-iteration-count: initial;
    animation-duration: 2s;
}
```
Apartir de aqui ya daremos formato general usando herencia a cada componente de nuestra página.
```

header .title{

    width: 100%;
    text-align: center;
    font-size: 5em;
    font-weight: 0;

    padding: 70px 0;
    color: #fff;
    background: rgba(90,90,255,.5);
}

header figure{
    text-align: center;
    margin: 30px 0;
}

header figure img{
    width: 150px;
    border-radius: 50%;
    border: 6px solid rgba(255, 255, 255, .1)
}

header .valor{
    text-align: center;
    color: ##313131;
    font-weight: 700;
    font-size: 1.2em;
}



```




Con estos códigos damos formatos a todas las clases que hemos creado en el archivo html, dentro del formato que hacemos aqui, se encuentra darle color a cada apartado asi como las diferentes animaciones que tendrá y el icono del cursor al pasar sobre cada objeto.
