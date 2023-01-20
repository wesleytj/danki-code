# Mais sobre Tabelas

Apesar de não ser obrigatório, existe uma forma ainda mais profissional para codar as tabelas, que é utilizando as TAGs:

- thead

- tbody

**Como funcionam as Tags?**

- thead
  
  ```html
  <thead></thead> <!-- Tag para cabeçalho da Tabela -->
  ```

Utilizamos a tag na primeira linha da tabela, para deixa-la em forma de título, assim o texto fica automaticamente centralizado e negrito.

```html
<table>
    <thead>
        <tr>
            <th>Nome</th>
            <th>Idade</th>
            <th>Cargo</th>
        </tr>
    </thead>
    <!-- Note que nesse caso, as colunas não mais td e sim th -->
        <tr>
            <td>Wesley Treib Jacques</td>
            <td>28</td>
            <td>Desenvolvedor Front-end</td>
        </tr>
</table>
```

**Obs. Note que quando utilizamos o `thead` as tags de colunas mudam de `td` para `th`**



- tbody
  
  ```html
  <tbody></tbody> <!-- Tag para o corpo da tabela -->
  ```

    Utilizamos a tag para o resto da nossa tabela, que será o corpo dela. Ela não altera nossa tabela, mas mantém a semântica.

```html
<table>
    <thead>
        <tr>
            <th>Nome</th>
            <th>Idade</th>
            <th>Cargo</th>
        </tr>
    </thead>
    <!-- Note que nesse caso, as colunas não mais td e sim th -->
    <tbody>
        <tr>
            <td>Wesley Treib Jacques</td>
            <td>28</td>
            <td>Desenvolvedor Front-end</td>
        </tr>
    </tbody>
</table>
```


