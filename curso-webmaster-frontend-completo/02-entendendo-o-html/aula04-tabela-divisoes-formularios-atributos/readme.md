# Tabelas, divisões, formulários e mais atributos

## Divisões

```html
<div></div> <!-- TAG de Divisão -->
```

A `<div></div>` serve para dividir o nosso website, seja através de imagem, texto, o que for... Serve para mantermos a organização na marcação e facilita depois para estilização do CSS

##### Exemplo de utilização:

```html
<div>
    <h2>Título do meu website</h2>
    <p>Conteúdo</p>
</div>

<div>
    <h2>Outra parte do site</h2>
    <p>Conteúdo</p>
</div>
```

## Tabela

```html
<table></table> <!-- Tag para Tabela -->
```

Como sabemos, uma tabela é composta por linhas e colunas e por isso, é importante aprendermos as TAGs de linha e coluna para tabela:

- tr => refere-se as linhas

- td => refere-se as colunas

```html
<table>
    <tr>
        <td></td>
        <td></td>
        <td></td>
    </tr>
</table>
<!-- Nesse exemplo, nos referimos a uma tabela de 1 linha e 3 colunas -->
```

Conforme o exemplo acima, temos uma tabela com 1 linha e 3 colunas, que vão servir como nosso "cabeçalho", então vamos criar mais uma linha e mais três colunas, para preencher a tabela:

```html
<table>
        <tr>
            <td>Nome</td>
            <td>Idade</td>
            <td>Cargo</td>
        </tr>

        <tr>
            <td>Wesley Treib Jacques</td>
            <td>28</td>
            <td>Desenvolvedor Front-end</td>
        </tr>
    </table>
```

E podemos ir preenchendo assim, sucessivamente, com quantas informações quisermos.

Já, introduzindo um pouco sobre atributos, existem alguns atributos que podemos utilizar nas tabelas também, como:

- width (Largura)
  
  - Aceita todos os tipos de medidas (px, %, em, etc...)

- align (Alinhamento)
  
  - Os valores aceitos são: Left, Center, Right

- border (Borda)
  
  - Manipula a espessura da borda da tabela

```html
<table width="900" align="center" border="2">
        <tr>
            <td>Nome</td>
            <td>Idade</td>
            <td>Cargo</td>
        </tr>

        <tr>
            <td>Wesley Treib Jacques</td>
            <td>28</td>
            <td>Desenvolvedor Front-end</td>
        </tr>
</table>
<!-- Não é indicado manipular o alinhamento e a borda através do atributos da tag, é boa prática de programação, deixar essa função diretamente para o CSS -->
```



## Formulário

```html
<form></form> <!-- Tag de Formulário -->
```

Parecido com a tabela, apenas a tag de formulário, não funciona por sí só, precisamos acrescentar algumas tags e declarar o que queremos que elas façam.
A mais utilizadas são:

- input
  
  - types:
    
    - text
    
    - number
    
    - password
    
    - email
    
    - etc...

- textarea

**Exemplo de código:**

```html
<form>
    <input type="text" />
    <textarea></textarea>
    <input type="submit" value="Enviar" />
</form>
```


