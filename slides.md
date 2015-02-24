# Markdown

![Markdown logo](img/208x128.png)

El lenguaje de marcas para los que no les gustan los lenguajes de marcas

--SLIDE--

## Bienvenidos

<table>
<tr><td>

![Yo](img/congato.jpg)

</td><td>

Pablo Hinojosa (*& Grizzly*)

http://www.psicobyte.com

@psicobyte_

</td></tr></table>

--SLIDE--

## ¿qué es Markdown

Texto simple, con ciertas convenciones "*lógicas*"

Un programa que convierte ese texto a **XHTML**

La extensión usual es **\*.md**

--SLIDE--

## El objetivo

Que cualquiera pueda editar un texto, sin restricciones de medio o conocimientos.

Fácil de leer, fácil de escribir.

--SLIDE--


## Antecedentes

* Textile
* ReStructuredText
* Wiki markup
* **email**

--SLIDE--

## ¿Quién?

John Gruber y Aaron Swartz

--SLIDE--

## ¿Por qué usar Markdown?

Simple, fácil, e intuitivo.

Código fuente **legible**.

Accesible y fácil de convertir.


--SLIDE--

## Párrafos

```md
Los párrafos se separan por una línea en blanco.
Esto no va separado y se mostrará a continuación.

Esto sí, y es otro párrafo.

Y esto es otro.
```

--SUBSLIDE--

Los párrafos se separan por una línea en blanco.
Esto no va separado y se mostrará a continuación.

Esto sí, y es otro párrafo.

Y esto es otro.

--SLIDE--

## Cabeceras

```md
# Cabecera H1
## Cabecera H2
### Cabecera H3
#### Cabecera H4
##### Cabecera H5
###### Cabecera H6
```

--SUBSLIDE--

# Cabecera H1
## Cabecera H2
### Cabecera H3
#### Cabecera H4
##### Cabecera H5
###### Cabecera H6

--SUBSLIDE--

## Cabeceras (Opcional)

```md
Cabecera H1
===========
Cabecera H2
-----------
```

--SUBSLIDE--

Cabecera H1
===========
Cabecera H2
-----------

--SLIDE--

## Citas

```md
Como dije yo mismo una vez:

> El texto tras el signo ">" aparece citado.
> Como en el correo electrónico.

> Muy conveniente.
```
Equivale al elemento `<blockquote>`

--SUBSLIDE--

Como dije yo mismo una vez:

> El texto tras el signo ">" aparece citado.
> Como en el correo electrónico.

> Muy conveniente.

--SLIDE--

## Énfasis (cursivas)

```md
Este texto contiene *Cursivas*

Este texto contiene _Cursivas_
```
Corresponde al elemento `<em>` de **HTML**

--SUBSLIDE--

Este texto contiene *Cursivas*

Este texto contiene _Cursivas_

--SUBSLIDE--

## Énfasis (negritas)

```md
Este texto contiene **Negritas**

Este texto contiene __Negritas__
```
Corresponde al elemento `<strong>` de **HTML**

--SUBSLIDE--

Este texto contiene **Negritas**

Este texto contiene __Negritas__

--SUBSLIDE--

## Tachado

```md
Y un poco de ~~texto Tachado~~
```

--SUBSLIDE--

Y un poco de ~~texto Tachado~~

--SLIDE--

## (escapando caracteres con "\\")

```md
Porque hay que saber distinguir *Hola* de \*Hola\*

El caracter de escape es \\

```

--SUBSLIDE--

Porque hay que saber distinguir *Hola* de \*Hola\*

El caracter de escape es \\

--SLIDE--

## Listas

```md
* Primer elemento
    * Subelemento
        * Sub-sub elemento
    * Otro subelemento
* Segundo elemento
+ Hay varias opciones, como + y -
- Y se pueden mezclar
* Y no pasa nada
```

--SUBSLIDE--

* Primer elemento
    * Subelemento
        * Sub-sub elemento
    * Otro subelemento
* Segundo elemento
+ Hay varias opciones, como + y -
- Y se pueden mezclar
* Y no pasa nada

--SUBSLIDE--

## Listas (numeradas)

```md
1. Primer elemento
    1. Subelemento
        1. Sub-sub elemento
    1. Otro subelemento
1. Segundo elemento
1. Tercero
1. Cuarto...
```

--SUBSLIDE--

1. Primer elemento
    1. Subelemento
        1. Sub-sub elemento
    1. Otro subelemento
1. Segundo elemento
1. Tercero
1. Cuarto...

--SLIDE--

## Barra Horizontal

¿pero alguien usa esto?

```md
-------------------------

- - - - - - - - - - - - -

_________________________

---
```

--SUBSLIDE--

-------------------------

- - - - - - - - - - - - -

_________________________

---

--SLIDE--

## Código

```md
Este código `self.parent = parent` está incrustado en una línea.
```

--SUBSLIDE--

Este código `self.parent = parent` está incrustado en una línea.

--SUBSLIDE--

<pre><code>
Esto es un bloque de código:

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

import sys

def Hola(var):
    if var == "hola":
        print "Hola Mundo"

Hola("hola")
```
</code></pre>

--SUBSLIDE--

Esto es un bloque de código:

```python
#!/usr/bin/env python
# -*- coding: utf-8 -*-

import sys

def Hola(var):
    if var == "hola":
        print "Hola Mundo"

Hola("hola")
```

--SLIDE--

## Enlaces

```md
Enlace a [Mi blog](http://www.psicobyte.com)
```

--SUBSLIDE--

Enlace a [Mi blog](http://www.psicobyte.com)

--SUBSLIDE--

```md
Y esto es un [Enlace por referencia][1]

La referencia [puede ser un texto][referencia de texto]

Y puede ser [el propio texto]

[1]: http://osl.ugr.es
[referencia de texto]: http://www.ugr.es
[el propio texto]: http://www.psicobyte.com
```

--SUBSLIDE--

Y esto es un [Enlace por referencia][1]

La referencia [puede ser un texto][referencia de texto]

Y puede ser [el propio texto]

[1]: http://osl.ugr.es
[referencia de texto]: http://www.ugr.es
[el propio texto]: http://www.psicobyte.com


--SLIDE--

## Imágenes

```md
![Foto de un gato en una caja](img/gato.jpg "Mi gato (Grizzly)")
```

--SUBSLIDE--

![Foto de un gato en una caja](img/gato.jpg "Mi gato (Grizzly)")

--SUBSLIDE--

## Imágenes (por referencia)

```md

![La misma foto del gato][gato]

[gato]: img/gato.jpg

```

--SUBSLIDE--

![La misma foto del gato][gato]

[gato]: img/gato.jpg

--SLIDE--

## Tablas

```md
|Cabecera 1 |Cabecera 2 |Cabecera 3 |
|-----------|----------:|:----------|
| celda 1 A | celda 2 A | celda 3 A |
| celda 1 B | celda 2 B | celda 3 B |

```

--SUBSLIDE--

|Cabecera 1 |Cabecera 2 |Cabecera 3 |
|-----------|----------:|:----------|
| celda 1 A | celda 2 A | celda 3 A |
| celda 1 B | celda 2 B | celda 3 B |



--SUBSLIDE--

```md
Cabecera 1 |Cabecera 2 |Cabecera 3
----|-----:|:------
celda 1A | celda 2A | celda 3 A
celda 1 B | celda 2 B | celda 3 B
```

--SUBSLIDE--

Cabecera 1 |Cabecera 2 |Cabecera 3
----|-----:|:------
celda 1A | celda 2A | celda 3 A
celda 1 B | celda 2 B | celda 3 B

--SLIDE--

## Hay algo que necesito y no está...

```md
...pero puedes usar <strong>HTML</strong>.
```

--SUBSLIDE--

...pero puedes usar <strong>HTML</strong>.

--SLIDE--

## ¿Donde?

http://stackoverflow.com 

http://github.com

pandoc





--SLIDE--

## Más allá de Markdown

R Markdown

http://rmarkdown.rstudio.com/

--SUBSLIDE--

![Uso de R Markdown](img/rmarkdown.png)

--SLIDE--

## Muchas gracias

¿Preguntas?

![Creative Commons By SA](img/Cc-by-sa.png)















--SLIDE--

## 

```md
```

--SUBSLIDE--




