# Notas del uso de Hugo, generador de sitios Web estáticos.

[https://gohugo.io](https://gohugo.io) Esta es la URL oficial de la página.


### Install

[https://gohugo.io/getting-started/installing/](https://gohugo.io/getting-started/installing/) Aparecen las instrucciones para instalar.

**Ubuntu**
> sudo apt-get install hugo

**ArchLinux**
> sudo pacman -Syu hugo

> Nota: Para iniciar submódulos en Git se hace con *git submodule add URLRepo*

Instalamos con *apt-get install hugo* en el caso de Ubuntu.

Inicializar un sitio nuevo con *hugo new site nameProject*

En [https://themes.gohugo.io/](https://themes.gohugo.io/) Se consiguen los temas disponibles realziados por la comunidad de código abierto, algunas tienen licencia de uso libre con modificaciones para uso comercial.

Tema utilizado para hacer el ejemplo [https://themes.gohugo.io/story/](https://themes.gohugo.io/story/).

Alterar la versión mínima en el tema en theme.toml.

Procedimiento:

- Entrar en la carpeta *themes* y hacer un submódulo en git.
- En la carpeta del proyecto hay una carperta que dice examples, tomar los archivos de allí.
- Hacer pequeño hack a la versión mínima de requisito.
- Hacer post con *hugo new posts/namePost.md*
- Continuar editando en formato Markdown.
