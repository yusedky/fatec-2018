# Aula 1 - Semestre 2

## Relembrando alguns conteúdos:

### format-detection
```
<meta nome="format-detection">
```
→ sim isso, o navegador não detecta formatos como no caso do telefone no IE

### abreviation
```
<abbs title="Final Fantasy XIV">FF14</abbs>
```
→ serve para colocar o significado da abreviação

### Como o navegador interpreta o número de telefone:
`<a href="tel:+551376767676">Telefone: (13)7676-7676</a>`
→ Detecta o telefone em navegadores que não o abrem sozinho normalmente ( *ao cliclar, pergunta por onde deseja abrir, como por exemplo o skype* ).

### Seletores personalizados: `class` e `id`

`id` → cada id no css pode ser usado **apenas uma vez** no html

`class` → pode ser usado mais de uma vez no html e é usado para **alterar elementos visuais**.

### Ordem de prioridade:
`!important` > id(`#`) > class(`.`) > tag 

### Pseudo-classe:
→ é uma class pré-definida para trabalhar caracteristicas especificas.

### Elementos de nível:
**De bloco** → separados por blocos (ex: *h1, h2, p, nav, ul, li, ...* ).

**De linha** → alinhado lado à lado por padrão (ex: *strong, em, a, img, ...* ).

**Propriedade `display` ** → permite alterar elementos de nível (ex: *inline, block, none, float* ).
