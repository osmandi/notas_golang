# Notas de la herramienta para presentar código en Golang

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
