# Aula 2 - Semestre 2

## Árvore de seletor descendente:

![arvore-seletor-descente](http://www3.ifrn.edu.br/~alexandregomes/design_web/css-parte_3/arvore.png)

* `li` e `li` são exemplos de irmão adjacentes (ficam lado a lado dentro do html).
* `p` e `blockquote` são exemplos de irmãos tradicionais (filhos de uma mesma tag pai).

-----------------------------------------------------

### Descendência:
```
body div { 
} 
```
→ funciona para todos os elementos de descendência (ex: *filho, neto, bisneto, ...* )

-----------------------------------------------------

### Seletores de filhos:
```
ul > li {
}
```
→ só funciona para níveis de pai e filho.

> Um filho é sempre um descendete, mas um descendente nem sempre é um filho.

### Exemplo de leitura:
```
<ul class="classp">
  <li> <a href="#" class="linkp"> Link 1 </a> </li>
  <li> <a href="#" class="linkr"> Link 2 </a> </li>
</ul>
```

```
u.classp > li > a.linkp {
  background-color: yellow;
}
```
→ comando dado a `ul` de classe `"classp"`, com filho `li`, com um neto `a` de classe `"linkp"`.

-----------------------------------------------------

### Seletor de irmão:
```
h1 ~ ul {
} 
```
→ irmão tradicional funciona para todos que forem irãos independente de proximidade dentro do html.

```
h1 + ul {
}
```
→ irmão adjacente só funciona para irmãos que estão ao lado dentro do html.

-----------------------------------------------------

### Seletor universal:
```
* {
} 
```
→ pega absolutamente tudo.

```
body > ul li * {
background-color: yellow;
}
```
→ **todo** `li` descendente de `ul` e exclusivamente filho de `body` terá seu fundo colorido de *amarelo*.
> Normalmente usado para css reset!

-----------------------------------------------------

### Pseudo-classes:
```
ul li:first-child{
}
```
→ pela o primeiro filho `li` dentro de `ul`

`first-child` → primeiro filho

`last-child` → ultimo

`nth-child` → nono

`first-child(even)` → alterna

`first-line` → toda a primeira linha

-----------------------------------------------------

### After / Before:

> em breve mais conteúdo.
