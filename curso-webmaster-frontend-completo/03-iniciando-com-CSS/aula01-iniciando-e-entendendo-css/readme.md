# Iniciando e entendendo o CSS

O CSS nada mais é que uma folha de estilos, que serve para estilizar nosso site, podemos fazer basicamente qualquer tipo de estilização das nossas TAGs no HTML.

## Como usar o CSS

Existem algumas formas de utilizar o CSS dentro do HTML, uma delas é a inline, que é colocando o css dentro da tag HTML, como se fosse um atributo.

```html
<h1 style="color: red;">Título h1</h1>
<h2 style="font-size: 50px;">Título h2</h2>
```

Outra maneira de utilizar o CSS, é dentro do próprio documento `index.html`

```html
<head>

    <style>
        /* 
            Comentário em CSS 
        */
        h2{
            color: orange;
        }

        h3{
            background: green;
        }

        a{
            text-decoration: none;
        }
    </style>

</head>
<body>
    <!-- Comentário em HTML -->

    <!-- CSS de forma inline -->
    <h1 style="color: red;">Título h1</h1>
    <h2 style="font-size: 50px;">Título h2</h2>
    <h3>Título h3</h3>
    <h4>Título h4</h4>
    <h5>Título h5</h5>
    <a style="text-decoration: none;" href="">Meu link!</a>

    <!-- CSS dentro do documento index.html -->
    <h1>Título h1</h1>
    <h2>Título h2</h2>
    <h3>Título h3</h3>
    <h4>Título h4</h4>
    <h5>Título h5</h5>
    <a href="">Meu link!</a>

</body>
```

**Obs.** *Perceba que para utilizar o CSS dentro do documento index.html, utilizamos a tag `<style>` dentro da tag ` <head>` do html, e dentro da tag ` <style>` fica a estilização*
