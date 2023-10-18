---
title: Markdown
description: 
published: true
date: 2023-10-15T10:33:19.903Z
tags: 
editor: markdown
dateCreated: 2023-10-15T10:33:13.523Z
---

# Incorporar imagens

## Incorporar imagens {.tabset}

### Visualização

![imagem com 64x64 pixels](/barraco-512.jpg =64x)

A imagem é incorporada diretamente ![imagem com 16x16 pixels](/barraco-512.jpg =16x) no texto.
A resolução é definida como `16x16 pixels` para que se encaixe bem no fluxo do texto.
Sem a especificação opcional da dimensão, a imagem seria produzida em resolução total.

### Código fonte

```markdown
![imagem com 64x64 pixels](/barraco-512.jpg =64x)

A imagem é incorporada diretamente ![imagem com 16x16 pixels](/barraco-512.jpg =16x) no texto.
A resolução é definida como `16x16 pixels` para que se encaixe bem no fluxo do texto.
Sem a especificação opcional da dimensão, a imagem seria produzida em resolução total.
```

# Incorporar imagens (com spoiler)

## Incorporar imagens (com spoiler) {.tabset}

### Visualização

<details>

![imagem no spoiler](/barraco-512.jpg =64x)

</details>

### Código fonte

```markdown
<details>

![imagem no spoiler](/barraco-512.jpg)


</details>
```

# bloco de citação

## citação em bloco {.tabset}

### Visualização

> Esta é uma citação de bloco regular, também conhecida como blockquote.

> Esta é um bloco de informação.
{.is-info}

> Esta é um bloco de sucesso.
{.is-success}

> Esta é um bloco de aviso.
{.is-warning}

> Esta é um bloco de erro/perigo.
{.is-danger}

### Código fonte

```markdown
> Esta é uma citação de bloco regular, também conhecida como blockquote.

> Esta é um bloco de informação.
{.is-info}

> Esta é um bloco de sucesso.
{.is-success}

> Esta é um bloco de aviso.
{.is-warning}

> Esta é um bloco de erro/perigo.
{.is-danger}
```

# Emoji

## Emoji {.tabset}

### Visualização

Você pode usar uma variedade de emojis como :palm_tree: ou :tea:.

### Código fonte

```markdown
Você pode usar uma variedade de emojis como :palm_tree: ou :tea:.
```

### Observações

> Uma visão geral detalhada dos emojis suportados pode ser encontrada nesta [Cheat Sheet](https://www.webfx.com/tools/emoji-cheat-sheet/).
{.is info}

# notas de rodapé

## notas de rodapé {.tabset}

### Visualização

Neste texto[^1] há duas notas de rodapé[^2].
As notas de rodapé podem ser encontradas no final de cada página.

[^1]: Esta é a primeira nota de rodapé.
[^2]: Esta é a segunda nota de rodapé.

### Código fonte

```markdown
Neste texto[^1] há duas notas de rodapé[^2].
As notas de rodapé podem ser encontradas no final de cada página.

[^1]: Esta é a primeira nota de rodapé.
[^2]: Esta é a segunda nota de rodapé.
```

# Linha divisória horizontal

## Separador horizontal {.tabset}

### Visualização

Este texto é separado por uma linha horizontal

---

linha divisória separada.

### Código fonte

```markdown
Este texto é separado por uma linha horizontal

---

linha divisória separada.
```

# hiperlinks

## Hiperlinks {.tabset}

### Visualização

Os hiperlinks podem ser incorporados como [texto](sintaxe/markdown) e como imagem [![imagem com 16x16 pixels](/barraco-512.jpg =16x)](sintaxe/markdown).

### Código fonte

```markdown
Os hiperlinks podem ser incorporados como [texto](sintaxe/markdown) e como imagem [![imagem com 16x16 pixels](/barraco-512.jpg =16x)](sintaxe/markdown).
```

# lista (tarefas)

## Lista (Tarefas) {.tabset}

### Visualização

- [X] Esta entrada na lista está completa.
- [ ] Esta entrada na lista ainda deve ser feita.

### Código fonte

```markdown
- [X] Esta entrada na lista está completa.
- [ ] Esta entrada na lista ainda deve ser feita.
```

# lista (numeração)

## lista (numeração) {.tabset}

### Visualização

1. Primeira entrada
2. Segunda entrada
3. Terceira entrada

### Código fonte

```markdown
1. Primeira entrada
1. Segunda entrada
1. Terceira entrada
```

### Observações

> É suficiente numerar todas as entradas com `1.`.
> Quando a página é construída, a numeração é automaticamente corrigida e contada na ordem registrada.
{.is info}

# lista (sem numeração)

## lista (não numerada) {.tabset}

### Visualização

Aqui está um exemplo de uma lista simples:
- Um item de lista simples.
- Ainda outro item de lista simples.
- E mais um item de lista simples.

Aqui está um exemplo de uma lista de grade:
- Um elemento de grade.
- Mais um elemento da grade.
- E outro elemento de grade.
{.grid-list}

Aqui está um exemplo de uma lista especialmente formatada para hiperlinks:
- [Um hiperlink *com descrição*](sintaxe/markdown)
- [Mais um hiperlink *com descrição adicional*](sintaxe/markdown)
- [E outro hiperlink *também com descrição*](sintaxe/markdown)
{.links-list}

### Código fonte

```markdown
Aqui está um exemplo de uma lista simples:
- Um item de lista simples.
- Ainda outro item de lista simples.
- E mais um item de lista simples.

Aqui está um exemplo de uma lista de grade:
- Um elemento de grade.
- Mais um elemento da grade.
- E outro elemento de grade.
{.grid-list}

Aqui está um exemplo de uma lista especialmente formatada para hiperlinks:
- [Um hiperlink *com descrição*](sintaxe/markdown)
- [Mais um hiperlink *com descrição adicional*](sintaxe/markdown)
- [E outro hiperlink *também com descrição*](sintaxe/markdown)
{.links-list}
```

# Código fonte

## código-fonte {.tabset}

### Visualização

Este texto contém formatação de código fonte `inline`.

```
Todo esse bloco de texto é formatado como código-fonte.
```

Exemplo com highlight:

```csharp
public static void Main(string[] args)
{
                 Ambiente.Exit(0);
}
```

### Código fonte

````markdown
Este texto contém formatação de código fonte `inline`.

```
Todo esse bloco de texto é formatado como código-fonte.
```

Exemplo com realce de sintaxe:

```csharp
public static void Main(string[] args)
{
                 Ambiente.Exit(0);
}
```
````

# spoilers

## spoilers {.tabset}

### Visualização

<details>
   <summary>Atenção: Spoilers</summary>
   Este é um texto de spoiler.
</details>

### Código fonte

```markdown
<details>
   <summary>Atenção: Spoilers</summary>
   Este é um texto de spoiler.
</details>
```

# Tabela

## Tabela {.tabset}

### Visualização

| Designação | tipo | valor |
|:-------------- |:-------:| ----:|
| Primeiro elemento | Primeiro | 1600 |
| Segundo elemento | Segundo | 12 |
| Terceiro elemento | Terceiro | 1 |

### Código fonte

```markdown
| Designação | tipo | valor |
|:-------------- |:-------:| ----:|
| Primeiro elemento | Primeiro | 1600 |
| Segundo elemento | Segundo | 12 |
| Terceiro elemento | Terceiro | 1 |
```

# abas

## Guias {.tabset}

### Visualização

As abas, que já podem ser vistas aqui na página toda, devem servir de exemplo.

### Código fonte

````markdown
## Guias {.tabset}

### Visualização

As abas, que já podem ser vistas aqui na página toda, devem servir de exemplo.

### Código fonte

```markdown
TEXTO...
```
````

### Observações

> As guias só podem ser usadas se os títulos correspondentes forem usados.
> Como pode ser visto no exemplo, o elemento `{.tabset}` deve ser anexado a um cabeçalho superior.
> Para cada guia, um cabeçalho correspondente deve ser especificado um nível abaixo, que serve como uma designação de guia.
{.is-info}

# ícones do teclado

## símbolos do teclado {.tabset}

### Visualização

Os ícones de botão também podem ser renderizados para melhorar a documentação e os guias:

<kbd>CTRL</kbd> + <kbd>X</kbd> para cortar um conteúdo.
<kbd>CTRL</kbd> + <kbd>C</kbd> para copiar o conteúdo.
<kbd>CTRL</kbd> + <kbd>V</kbd> para inserir conteúdo.

### Código fonte

```markdown
Os ícones de botão também podem ser renderizados para melhorar a documentação e os guias:

<kbd>CTRL</kbd> + <kbd>X</kbd> para cortar um conteúdo.
<kbd>CTRL</kbd> + <kbd>C</kbd> para copiar o conteúdo.
<kbd>CTRL</kbd> + <kbd>V</kbd> para inserir conteúdo.
```

# Formatação de texto

## Formatação de texto {.tabset}

### Visualização

Este texto está **negrito**.

Este texto está em *itálico*.

Este texto está <ins>sublinhado</ins>.

Este texto é ~~riscado~~.

Este texto é ^sobrescrito^.

Este texto é ~subscrito~.

### Código fonte

```markdown
Este texto está **negrito**.

Este texto está em *itálico*.
Este texto está em _itálico_.

Este texto está <ins>sublinhado</ins>.
Este texto está <u>sublinhado</u>.

Este texto é ~~riscado~~.

Este texto é ^sobrescrito^.

Este texto é ~subscrito~.
```

### Combinação de teclas

<kbd>CTRL</kbd> + <kbd>B</kbd> para **negrito**.
<kbd>CTRL</kbd> + <kbd>I</kbd> para *itálico*.


# Manchetes

## Títulos {.tabset}

### Visualização

Os títulos também são usados com muita frequência nesta página.

O nível do título pode ser especificado usando `#`. Quanto menos `#`, maior o nível e vice-versa.
A sintaxe pode ser verificada de acordo na guia de texto de origem.

Como alternativa, `=` ou `-` também podem ser inseridos sob o cabeçalho.

### Código fonte

```
# Cabeçalho de 1º nível
## Cabeçalho de 2º nível
### Cabeçalho da fase 3
#### Cabeçalho de nível 4
##### Cabeçalho de nível 5
###### Título da fase 6

####### Isso não é mais uma manchete.

Esta é uma ortografia alternativa para um cabeçalho de nível 1
==

Esta é uma ortografia alternativa para um cabeçalho de 2º nível
--
```

# Adicional

Existem outras funções que ainda precisam ser documentadas ou são fornecidas por plugins.

> Wiki.js oferece suporte à markdown completo.
> Portanto, as funções não descritas aqui também devem funcionar (por exemplo, incorporar vídeos do YouTube, etc.).
{.is info}
