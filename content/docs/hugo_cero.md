---
title: "hugo desde cero "
date: 2023-01-20T07:43:36-05:00
author: "Ney Perea"
draft: false
tag: hugo
---


[![](https://d33wubrfki0l68.cloudfront.net/c38c7334cc3f23585738e40334284fddcaf03d5e/2e17c/images/hugo-logo-wide.svg)](https://gohugo.io/)
<br>
 es un creador de sitios web estáticos que le permite crear un sitio web con poco o ningún código. Los generadores de sitios estáticos generalmente le permiten escribir su contenido en un lenguaje de marcado simple, como Markdown.
## ¿Qué es un sitio web estático?.
Un sitio web estático es un sitio cuyas páginas están diseñadas para que el contenido permanezca constante para todos los visitantes y no cambie, no hay una base de datos asociada con el sitio web a través del cual se cambia el contenido, y nadie puede cambiar o actualizar el contenido excepto por regresando al programador que actualiza las páginas y luego las vuelve a cargar al servidor nuevamente. Por lo general, un sitio web estático consta de una o varias páginas que son independientes entre sí, cada una de las cuales representa un archivo HTML y archivos asociados, como archivos CSS o Javascript.


## Chocolatey.
 es un administrador de paququete para windows. Lo podemos encontrar en **[pargina de chocolatey](https://chocolatey.org/)**.
![](https://chocolatey.org/assets/images/global-shared/logo-square.svg)

Es una de las formas mas faciles de instalar hugo;  **[¿Por qué usar chocolatey?](https://chocolatey.org/why-chocolatey)**

## Instalacion de Hugo con Chocolatey.
Desde **powerShell** instala chocolatey 
con el siguente comando:

`choco install hugo-extended` 

luego instala hugo usando el gestor de paquetes para windows chocolatey:

`choco install hugo-extended -confirm`

Para verificar que hugo quedó correctamente instalado usamos el comando:

`hugo verision`
debe mostrar algo como esto:

 `hugo v0.109.0-47b12b83e636224e5e601813ff3e6790c191e371+extended windows/amd64 BuildDate=2022-12-23T10:38:11Z VendorInfo=gohugoio`

## Hugo vs Hugo Extended
En la página de Hugo, cuando se explica la instalación para Windows, mencionan también la posibilidad de instalar el paquete "Hugo Extended". Básicamente es el mismo Hugo pero con soporte para la compilación de Sass/SCSS. Podría ser interesante si vamos a usar el  preprocesador de CSS.
<hr>

## Comandos utiles desde la terminal.

`hugo check`  – ejecuta varias comprobaciones de verificación

`hugo config` – muestra la configuración de un sitio Hugo.

`hugo convert` – convierte contenidos a diferentes formatos.
hugo deploy – despliega tu sitio en un proveedor de la nube.

`hugo env `– muestra la versión de Hugo y la información del entorno.

`hugo gen` – proporciona acceso a varios generadores.

``hugo help ``– muestra información sobre un comando.

``hugo import`` – permite importar un sitio desde otro lugar

``hugo list ``– muestra una lista de varios tipos de contenido

``hugo mod ``– proporciona acceso a varios ayudantes de módulos

``hugo new`` – te permite crear nuevos contenidos para tu sitio

``hugo server`` – inicia un servidor de desarrollo local

``hugo version`` – muestra la versión actual de Hugo


## sitios donde consultar de hugo:
### [Primeros pasos con Hugo](https://desarrolloweb.com/articulos/primeros-pasos-hugo)

### [Cómo construir un sitio estático rapidísimo con Hugo](https://kinsta.com/es/blog/hugo-sitio-estatico/#:~:text=En%20t%C3%A9rminos%20de%20rendimiento%20bruto,completar%20m%C3%A1s%20de%20media%20hora.)

### [¿Qué es el Generador de Sitios Web Persistentes de Hugo?](https://www.dz-techs.com/es/hugo-static-site-generator)



## crear un sitio hugo
`hugo new site primeros-pasos-hugo`

![](/themes/tale-hugo/static/images/captura_crear_sitio.png)
![](/themes/tale-hugo/static/images/captura_live_server.png)
### Añadir un tema 
Los temas de Hugo nos permiten crear un sitio web con un aspecto
atractivo y con mínimo esfuerzo. En el sitio web de Hugo una sección **[completamente dedicada a themes](https://themes.gohugo.io/)**, donde hay muchas alternativas interesantes y adaptables a todos los tipos de proyecto.
Hay temas realmente atractivos en el directorio de temas de Hugo, pero yo voy a usar uno un poco más sencillo,Trabajaremos con este theme, que aunque es sencillo también resulta bastante limpio: https://github.com/EmielH/tale-hugo

se va al subdirectorio theme y se ejecuta:

`git submodule add  https://github.com/EmielH/tale-hugo `


añade el tema al archivo config.toml

`echo "theme = 'tale-hugo'" >> config.toml`

o lo modificas directamente desde visual studio code:
añades al archivo "config.toml" la siguiente linea:theme = 'tale-hugo'.

para probar como vamos ejecutamos:
`hugo server` y nos arranca un liveserver en la siguente dirección:
http://localhost:1313/

ahora podemos llenar el tema con nuestra propia informacion. para ello el comando

`hugo new posts/post1.md` crea el siguente archivo:
`content/post1.md`
este se edita en **Markdown**, esta es la cabecera de cada post
![](/themes/tale-hugo/images/captura_live_server.png)

cuando el draft esta en true el contenido de este post no se publica, se puede revisar en modo develpment con el siguente comando:

`hugo server --buildDrafts `

`hugo server -D`

### Añadir contenido

[por aqui voy](https://gohugo.io/getting-started/quick-start/#add-content)

[tener en cuenta la documentacion del tema](https://github.com/EmielH/tale-hugo/)

<hr>
algo suelto por aca 
shortcodes.

{{< youtube w7Ft2ymGmfc >}}

<hr>