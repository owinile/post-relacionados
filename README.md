> El mejor plugins de entradas relacionadas para Blogger

# Paso 1: Agregar CSS en blogger 
Todo lo que esta en el archivo entradas-relacionadas-estilos.css<br>

# Paso 2: añadir bibliotecas
Encima de la etiqueta </head> Pega:
```xml
<link href="//netdna.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.css" rel="stylesheet"/> 
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
```
# Paso 3: Añadir el código HTML/Javascript en blogger
 Incluir todo el contenido de **entradas-relacionadas-include.xml** dentro de un widget tipo "Blog", posteriormente, utilizar la siguiente etiqueta para incrustar los post relacionados donde se desee:

```xml
<b:include name='postRelated'/>
```

**Consejo:** Puede evitar la carga de post relacionados dentro de la vista previa ya que no se requiere, para ello agregue una condición:

```xml
<b:include cond='!data:view.isPreview' name='postRelated'/>
```


# Paso 4: Ajustes entradas a mostrar

Una vez incluido el código en el tema, el siguiente paso es desplazarnos hacia abajo lentamente hasta encontrar la línea 
```xml
Var maxresults=
```
Desde esa etiqueta tendrás la posibilidad de establecer la cantidad de entradas relacionadas que se mostrarán en la parte inferior de la publicación. En el código, en este caso nosotros hemos configurado solo 3 publicaciones. Pero puedes cambiarlo según tu preferencia.
