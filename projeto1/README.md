# Praticando SASS
Aa realizar o curso de SASS criamos o projeto Galleria, nele foi possível abordar a metodologia do SASS. Uma tecnolgia magnifica, incrível.

[![Preview do projeto](./img/screenshot.avif "Clique para acesasr o preview do Projeto")](https://gleristoncastro.com.br/portfolio/github/preview/SASS/projeto3/)


_Para visualizar o preview do projeto clique na imagem acima._
______________________

Para instalar o SASS de forma global utilizar a seguinte linha de comando

``` console
> npm i -g sass
```

desta forma o "g" tornou global o uso do sass nos projetos.

Para conferir a instalação foi realizada com sucesso, podemos testar verificando a versão.

``` console
> sass --version
```

Para que seja gerado automaticamente o CSS, devemos deixar em modo assistido, com o comando abaixo, conforme esse projeto.

``` console
> sass --watch sass/styles.sass:css/styles.css
```

Podemos criar arquivos sass que contenham variáveis.

``` scss
$primary-color: #fff
$secondary-color: #20c997
$text-color: #777
$bg-color: #000
$container-width: 1170px
```

Para incluir sass com variáveis podemos usar o @use e 'nomeDoAquivo' sem o '_' e a extensão sass

O que mais chama atenção no SASS é a hierarquia do código

``` scss
&-social-media

        ul
            height: 100%
            @include mixins.flex-center

            li
                margin: 0 1rem

                a
                    &:hover
                        color: variables.$primary-color
```
que resulta em

``` css
.header-social-media ul {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.header-social-media ul li {
  margin: 0 1rem;
}
.header-social-media ul li a:hover {
  color: #fff;
}
```

com menos código e podendo reaproveitar trechos de códigos com facilidade.

> Sem sombra de dúvida o SASS é uma ferramenta incrível, apenas com pouco mais de 150 linhas (isso sem resumo de linhas) consegui fazer todo o css, que após transpilar passou a ter mais de 220 linhas. O SASS me lembrou bastante o TypeScript. Foi bom conhecer, quero adotar em futuros projetos.

______________________
### Agradecimentos/Créditos:

Gostaria de agradecer ao [Matheus Battisti](https://github.com/matheusbattisti) por disponibilizar seu tempo e disseminar seu conhecimento.

- [SASS: Crie o seu primeiro projeto](https://www.udemy.com/share/104mdS3@2joPWH7Eqwp0GEy6AV6myjzRKkTk3TDN2cUsWwl57Xbkbjcm39qhXGgKHIg1sz1v/)

______________________
### Dificuldades

Não sentir dificuldades visto que já tenho uma boa bagagem de CSS, a sintaxe do SASS muito prática.