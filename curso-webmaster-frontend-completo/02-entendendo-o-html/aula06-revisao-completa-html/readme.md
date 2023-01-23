# Revisão completa HTML

#### Div

```html
<div></div> <!-- serve para fazer divisões no site -->
```

A tag `div` serve para fazer divisões no site, e podemos colocar quantas `divs` quisermos. Principlamente, uma dentro da outra:

```html
<div>
    <div>
        <h1>Título</h1>
    </div>
</div>
```

**Obs.**  *As tags de títulos, vão de 1 à 6.*

#### Texto

```html
<p></p> <!-- serve para fazer paragrafos no site -->
<span></span> <!-- serve para representar elementos visuais destacados de um todo no site -->
```

**Obs.** *Podemos colocar outras tags dentro de p e sapn também, como as tags abaixo*

#### Tags de formatação

```html
<b></b> <!-- negrito -->
<i></i> <!-- italico -->
<u></u> <!-- sublinhado -->
```

#### Img

```html
<img src"caminho-da-imagem/nome-da-imagem.extensao-da-imagem" />
```

**Obs1.** *Nos atributos da tag img, podemos definir a largura e altura da imagem*

**Obs2.** *Se definir apenas a largura, a altura é definida automaticamente, para manter a proporção da imagem e evitar distorção*

**Obs3.** *Se a imagem estiver no mesmo diretório do arquivo index, não precisar informar o diretório no atributo src, ou podemos apenas colocar um ponto (.)*

**Obs4.** *A extensão da imagem no final do atributo é obrigatório*



#### Links

```html
<a href="endereco-url-do-site">Texto que receberá o link</a>
```

**Obs.** *Para abrir o link numa nova aba, precisamos usar o atributo target=_blank*



#### Tabelas

```html
<table>
    <thead>
        <tr>
            <th>Nome</th>
            <th>Cargo</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>Seu-Nome-Aqui</td>
            <td>Seu-Cargo-Aqui</td>
        </tr>
    </tbody>
</table>
```

**Obs.** *A coluna só é TH se utilizarmos o Thead, se não, é TD*



#### Formulário

```html
<form>
    <input tyoe="text" />
    <input tyoe="password" />
    <textarea></textarea>
    <input tyoe="submit" value="Enviar" />
    <input tyoe="button" value="Enviar" />
    <button>Enviar</button>
</form>
```


