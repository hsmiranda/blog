---
layout: post
comments: true
title: "Instalando jekyll e publicando o seu primeiro post"
date:   2020-01-07 17:00:52 -0300
categories: jekyll ruby blogging
permalink: /posts/instalando-jekyll-e-publicando-seu-primeiro-post/
---
Hi :) 

Bom neste post vou explicar rapidamente como instalar e publicar posts no Jekyll. 

Primeiro instale os pre-requisitos dele, se você utiliza o Fedora é só rodar:

```shell
sudo dnf install ruby ruby-devel @development-tools
```

Pra instalar o jekyll e sua bibliotecas execute:
```shell
gem install jekyll bundler
```

Agora vamos gerar a build, use o comando:
```shell
jekyll new Meu Blog
```

Acesse o diretorio criado e execute o comando 
```ruby 
bundle exec jekyll serve
```

E acesse o link: [http://localhost:4000](http://localhost:4000) e a magica aconteceu :)

Agora vamos escrever o hello world (o primeiro post do blog)! 

Para realizar este processo basta criar um arquivo no diretorio _posts, por exemplo: primeiro-post.md com o seguinte conteudo:

```shell
---
layout: post
title: "Primeiro post"
date:   2020-01-07 17:00:52 -0300
categories: post
permalink: /url-primeiro-post
---
# Primeiro

Este e um exemplo de primeiro post
```
Salve o arquivo e no diretorio aonde foi criado site execute o comando: bundle exec jekyll serve e veja o resultado no seu browser.

