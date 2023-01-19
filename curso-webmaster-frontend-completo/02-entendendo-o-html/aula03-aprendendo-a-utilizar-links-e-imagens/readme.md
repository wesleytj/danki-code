# Aprendendo a utilizar links e imagens

## Imagens

```html
<img /> <!--TAG de Imagem-->
```

Podemos escolher qualquer imagem que quisermos no google e salvar no mesmo local do nosso arquivo `index.html`.

E para utilizarmos essa imagem no web site, precisamos utilizar a TAG `img`. 
Mas se só colocarmos a TAG, nada acontece, precisamos por um `atributo` dentro da TAG que informa qual imagem que deve ser renderizada naquela TAG:

```html
<img src="img1.png" />

<!--Observe que o nome deve ser exatamente o nome como a imagem está salva e não podemos esquecer de incluir a extensão da mesma-->

<!--Caso a imagem esteja exatamente dentro da mesma pasta que o arquivo index.html, não há necessidade de informar o diretório-->


```

<img title="null" src="file:///C:/Users/wesle/OneDrive/Área de Trabalho/workspace/github__projects/danki-code/curso-webmaster-frontend-completo/02-entendendo-o-html/aula03-aprendendo-a-utilizar-links-e-imagens/img1.png" alt="null" data-align="center">

### E se a imagem estiver em um diretório diferente?

O correto é colocar todas as imagens que serão utilizadas, dentro de uma pasta específica, para isso vamos criar uma pasta chamada `img` e por nossa foto lá.

Após isso, no atributo src, colocaremos o caminho, que agora sim, será: nome-do-diretorio/nome-da-imagem.extensao

```html
<img src="img/img2.png" />
```

<img title="null" src="file:///C:/Users/wesle/OneDrive/Área de Trabalho/workspace/github__projects/danki-code/curso-webmaster-frontend-completo/02-entendendo-o-html/aula03-aprendendo-a-utilizar-links-e-imagens/img/img2.jpg" alt="null" data-align="center">

### Imagem externa na internet fora do diretório local

Não é necessáriamente ter a imagem localmente para utiliza-la, desde que tenhamos o link de onde ela se encontra. Vamos exemplificar utilizando uma imagem diretamente do google.

Encontre a imagem que deseja utilizar e copie a `url` dela, depois disso, cole a `url` dentro do atributo `src`.

```html
<img src="https://blog.emania.com.br/wp-content/uploads/2016/02/direitos-autorais-e-de-imagem.jpg" />
```

<img title="null" src="https://blog.emania.com.br/wp-content/uploads/2016/02/direitos-autorais-e-de-imagem.jpg" alt="null">



### Alterando o tamanho da imagem

Podemos alterar o dimensionamento das imagens, diretamente pelos atributos dentro da TAG

- width => largura

- height => altura

```html
<img src="https://blog.emania.com.br/wp-content/uploads/2016/02/direitos-autorais-e-de-imagem.jpg" width="500" />
```

**Obs. Quando dimensionamos apenas a largura (width), a altura (height) se ajusta automaticamente, para que não tenha distorções**



---



## Links

Para utilizar os links, utilizamos a tag `a`:

```html
<a></a> <!-- a => ancora -->
```

O link funciona de forma parecida com a imagem, ele por sí só, não faz nada. Precisamos informar pra onde queremos ser redirecionados.



```html
<p>Você quer ir para o google? <a href="https://www.google.com.br" >Clique Aqui!</a></p>
```

Quando clicarmos em cima do link, iremos direto para o site informado.
Dessa forma, nós apenas somos redirecionados, acabamos saindo do site que estamos e vamos para o site que o link nos enviou.

Não seria melhor se o link abrisse em uma nova aba? Sim, né? Para isso, utilizamos um atributo chamado `target`

```html
<p>Você quer ir para o google? <a href="https://www.google.com.br" target="_blank">Clique Aqui!</a></p>
```

Prontinho, agora quando clicarmos, o link vai abrir em uma nova aba.
