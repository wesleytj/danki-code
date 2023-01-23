# Estilos externos, Ids e Classes

A terceira maneira (e a maneira mais correta) de utilizar o CSS, é de forma externa.
Criando um arquivo com extensão `.css` no mesmo diretório do arquivo `index.html` podemos chamar o css da maneira abaixo:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Aula 02 - Estilos externos, IDs e Classes</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- conteudo -->
</body>
</html>
```

Note que no exemplo acima, o nome do arquivo é `style`, é a forma mais comum de chamarmos nosso arquivo de estilo, mas podemos dar o nome que quisermos.

Ainda assim, a maneira mais profissional de utilizar o CSS, é criando um diretório especialmente para ele (parecido com o que fizemos com as imagens nas aulas anteriores de HTML)

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Aula 02 - Estilos externos, IDs e Classes</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <!-- conteudo -->
</body>
</html>
```

Assim, criamos uma pasta chamada `css`, no mesmo diretório do arquivo `index.html` e dentro dessa pasta, colocamos nossa folha de estilo `style.css`.

E como podem perceber, a TAG utilizada para fazer a chamada do arquivo `.css` é a TAG `link`.



## Ids

Os `ids` servem para identificar as tags HTML no nosso documento, porém, ao contrário das classes, os Ids não podem ser repetidos.
Apesar do HTML e o CSS funcionarem normalmente, mesmo que existam vários Ids com a mesma identificação, é uma má prática de programação fazer isso. Os ids devem ser únicos.
E geralmente utilizamos Ids, apenas quando formos utilizar também o `JavaScript`, para realizar animações e etc..

```html
<div id="div1">
    <!-- conteúdo -->
</div>
```

```css
#div1{
    /* estilização */
}
```

**Obs.** Note que para identificar o id no CSS, utilizamos o `#` 



## Classes

Ao contrário dos Ids, como mencionado anteriormente, as classes podem se repetir ao longo do nosso desenvolvimento, podemos ter diversas tags que utilizam do mesmo nome de classe.

```html
<div class="div1">
    <!-- conteúdo -->
</div>
```

```css
.div1{
    /* estilização */
}
```

**Obs.** Note que os Ids são identificados por `#`, já as classes são identificadas por `.` no nosso CSS

E podemos ter tambéms, várias classes para o mesmo elemento, por exemplo:

```html
<div class="div1 outraclasse terceiraclasse assimpordiante">
    <!-- conteúdo -->
</div>
```



## Como chamar Id ou Classe no CSS?

**No HTML**

```html
<body>
    <div id="div1" class="div1 class">
        <h1>Título 1</h1>
        <div id="div3" class="div3 class">
            <h1>Título neto da div pai</h1>
        </div>
    </div>

    <div id="div2" class="div2 class">
        <h1>Título 2</h1>
    </div>
</body>
```

**No CSS**

```css
h1{
    color: red;
}
```

Dessa forma, todos os `h1` terão a mesma cor.

Por isso utilizamos os identificadores, vamos aprender a estilizar separadamente, vamos continuar usando o mesmo exemplo de estrutura HTML.



**No CSS**

```css
#div1 h1{
    color: red;
}

#div2 h1{
    color: orange;
}

#div3 h1{
    color: blue;
}
```

Dessa forma, cada título terá uma cor diferente. Note que estamos dizendo:
"Dentro da div com id = *** pegue o h1 e faça ..."



Agora por exemplo:

```css
#div1 h1{
    color: aqua;
}
```

Dessa maneira, note que até mesmo o título que está dentro da div com id `div3` ficou da mesma cor, isso porque estamos dizendo:

"Pegue todos os h1 que estiverem dentro do id `div1` direta e indiretamente"

Mas se usarmos o sinal `>` :

```css
#div1 > h1{
    color: aqua;
}
```

Agora apenas o h1 diretamente dentro da div com id `div1` mudou de cor, pois o outro h1 não é filho direto.



Note que nos exemplos chamamos a div sempre pelo `id`, mas o mais comum e correto é utilizar a `class` faremos isso no último exemplo e mostrar o que acontece quando vários elementos possuem a mesma TAG:

```css
.class h1{
    color: yellow;
    font-size: 45px;
}
```

Assim, todos os h1 que temos na página receberam a mesma estilização, mudaram de cor e aumentaram de tamanho.



**Exercício bônus**

- O que acontece se no CSS:

```css
.div1 .div3 h1{
    color: #fff;
}
```



## O que aprendemos?

- Aprendemos a importar um arquivo de estilo externo

- Aprendemos como identificar nossas tags

- Aprendemos a procurar tags dentro das nossas classes ou ids


