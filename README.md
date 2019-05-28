# Notas de Golang

Estas son las notas de Golang, con la finalidad de usarlas en proyectos y presentaciones en este tema.

Web Page [golang.org](https://golang.org)
Slack [gophers.slack.com](https://gophers.slack.com)
Twitter [@golang](https://twitter.com/golang)

## Instalacion

> Se recomienda usar Ubuntu o cualquier otro Linux ya que el rendimiento es mejor en este entorno.

Entrar en [https://golang.org/dl/](https://golang.org/dl/) y descargar la imagen.

```
tar -C /usr/local -xzf go1.12.5.linux-amd64.tar.gz
```

**Variables de entorno**

En el archivo `~/.bashrc` agregar las siguientes variables.
```
export GOROOT=/usr/lib/go
export GOPATH=/$HOME/go
export GOBIN=$GOPATH/bin
export PATH=$GOROOT/bin:$GOBIN:$PATH
```

## GoDoc
- `go doc fmt`
- `go doc fmt Printf`
- `godoc -http :8080`

## GoPresent

### Install

```
go get golang.org/x/net
go get golang.org/x/tools
go install golang.org/x/tools/cmd/present
```

sample.slide

```

Title of document
Subtitle of document
15:04 2 Jan 2006
Tags: foo, bar, baz

Author Name
Job title, Company
joe@example.com
http://url/
@twitter_name
Some Text

* Title of slide or section (must have asterisk)

Some Text
```

Run with *present*.

Doc [Package present](https://godoc.org/golang.org/x/tools/present).

> Es muy importante entrar desde la URL desde la terminal para que el código de Golang compile correctamente.

[Go Present - Youtube](https://www.youtube.com/watch?v=83JBmS8WpHM)

## GoTour

[GoTour](https://github.com/golang/tour) En este enlace se encuentra la página del proyecto en cuestion.


Comando para instalar la librería. Es importante tener seteado *GOBIN* correctamente.
> go get -v -u golang.org/x/tour

Correr con `tour`. (El cual es el que está almacenado en la carpeta *bin* del path de go.

## Hugo

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
- Hacer post con *hugo new posts/namePost.md