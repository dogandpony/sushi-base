# Classes Utilitárias

>As Classes Utilitárias são a coleção de pequenas classes com objetivo 
específico. Algumas trocam o tamanho da fonte, outras modificam a visibilidade 
de um elemento em determinados breakpoints.

O Sushi Base implementa as seguintes Classes Utilitárias:

* [Alinhamento](/pt-br/utilities?id=alinhamento)
* [Clearfix](/pt-br/utilities?id=clearfix)
* [Display](/pt-br/utilities?id=display)
* [Elevação](/pt-br/utilities?id=elevação)
* [Float](/pt-br/utilities?id=float)
* [Overflow](/pt-br/utilities?id=overflow)
* [Posicionamento](/pt-br/utilities?id=posicionamento)
* [Espaçamento](/pt-br/utilities?id=espaçamento)
* [Tipografia](/pt-br/utilities?id=tipografia)
* [White Space](/pt-br/utilities?id=white-space)
* [Larguras](/pt-br/utilities?id=larguras)
* [Impressão](/pt-br/utilities?id=impressão)

?>O conjunto de Classes Utilitárias mais utilizado certamente será o [Utilitário
de Larguras]. Em conjunto com o [Objeto Layout] as Classes Utilitárias de 
Larguras possibilitam criar grids que se adaptam ao breakpoint atual sem a 
necessidade de criar classes especiais ou definir media queries customizados.

As Classes Utilitárias são as últimas a serem importadas no arquivo `app.scss`.



## Alinhamento

> Conjunto de Classes Utilitárias que modificam a propriedade `vertical-align` 
de um elemento. Além disso, inclui uma utilitária para centralizar elementos com
`margin: 0 auto`.

#### Alinhamento Vertical

| Classe  | vertical-align |
|---------|----------------|
| `_vabl` | baseline       |
| `_vab`  | bottom         |
| `_vam`  | middle         |
| `_vat`  | top            |
| `_vas`  | sub            |
| `_vap`  | super          |


#### Alinhamento horizontal 

| Classe    | margin-right | margin-left |
|-----------|--------------|-------------|
| `_center` | auto         | auto        |


#### Exemplos

```html
<td class="_vam">Item alinhado ao centro vertical</td>

<div class="_center">Item alinhado ao centro horizontal</div>
```

[//]: # (----------------------------------------------------------------------)

## Clearfix
 
> Classe Utilitária que ajuda a normalizar a técnica de clearfix pela página.

```html
<div class="_clearfix">
  <div class="_fl">Item com float: left</div>
  <div class="_fr">Item com float: right</div>
</div>
```

[//]: # (----------------------------------------------------------------------)

## Display
 
> Conjunto de Classes Utilitárias que modificam a propriedade `display` de um
elemento. Além disso, inclui uma utilitária para esconder um elemento apenas
visualmente.

#### Esconder visualmente um elemento

| Classe    |                           |
|-----------|---------------------------|
| `_hidden` | *ver ferramenta [hide()]* |


#### Display

| Classe  | display            |
|---------|--------------------|
| `_dn`   | none               |
| `_di`   | inline             |
| `_db`   | block              |
| `_dli`  | list-item          |
| `_dib`  | inline-block       |
| `_dit`  | inline-table       |
| `_dt`   | table              |
| `_dtc`  | table-cell         |
| `_dtcl` | table-column       |
| `_dtcg` | table-column-group |
| `_dtfg` | table-footer-group |
| `_dhg`  | table-header-group |
| `_dr`   | table-row          |
| `_drg`  | table-row-group    |
| `_df`   | flex               |
| `_dif`  | inline-flex        |
| `_dg`   | grid               |
| `_dig`  | inline-grid        |


#### Exemplos

```html
<p class="_hidden">
  Este bloco de texto está escondido da página, mas será lido por leitores 
  de tela.
</p> 

<p class="_dn">
  Este bloco de texto está escondido da página e não pode ser lido por leitores
  de tela.
</p> 
```

[//]: # (----------------------------------------------------------------------)

## Elevação

> Conjunto de Classes Utilitárias que adicionam sombras a um elemento para que
ele pareça elevado em relação à página.

```html
<div class="_elevation4">
  Este elemento parecerá suspenso em relação à página
</div>

<div class="_elevation16">
  Este elemento parecerá ainda mais suspenso em relação à página
</div>
```

[//]: # (----------------------------------------------------------------------)

## Float

> Conjunto de Classes Utilitárias que modificam a propriedade `float` de um
elemento.

| Classe | float |
|--------|-------|
| `_fn`  | none  |
| `_fl`  | left  |
| `_fr`  | right |

```html
<div class="_fl">Item com float: left</div>
<div class="_fr">Item com float: right</div>
```

[//]: # (----------------------------------------------------------------------)

## Overflow

> Conjunto de Classes Utilitárias que modificam a propriedade `overflow` de um
elemento.

```html
<div class="_ova">Este item terá scrolls quando necessário</div>
<div class="_ovya">Este item terá scrolls verticais quando necessário</div>
```

[//]: # (----------------------------------------------------------------------)

## Posicionamento

> Conjunto de Classes Utilitárias que modificam as propriedades `position`,
`top`, `right`, `bottom` e `left` de um elemento levando em consideração as 
[Configurações de Espaçamento].

#### Propriedade Position

| Classe | position |
|--------|----------|
| `_pos` | static   |
| `_por` | relative |
| `_poa` | absolute |
| `_pof` | fixed    |
| `_pot` | sticky   |


#### Exemplos

```html
<div class="_poa _t0 _r0">
  Este elemento se posicionará no canto superior direito
</div>

<div class="_por">
  Este elemento tem position: relative
</div>
```

[//]: # (----------------------------------------------------------------------)

## Impressão

> Conjunto de regras que normalizam a saída de CSS para impressão.

[//]: # (----------------------------------------------------------------------)

## Espaçamento

> Conjunto de Classes Utilitárias que modificam as propriedades `margin` e 
`padding` de um elemento levando em consideração as [Configurações de 
Espaçamento].

```html
<div class="_pxxs">
  Este elemento tem padding "xxs" (que por padrão é 8px)
</div>

<div class="_mrxs _ml">
  Este elemento tem margem direita "xs" (que por padrão é 16px) e margem
  esquerda padrão (que por padrão é 32px)
</div>
```

[//]: # (----------------------------------------------------------------------)

## Tipografia

> Conjunto de Classes Utilitárias que modificam diversas propriedades
relacionadas à tipografia de um elemento (como `font-size` e `line-height`)
levando em consideração as [Configurações de Tipografia].

```html
<h1 class="_fz2">Este heading nível 1 tem tamanho de fonte nível 2</h1>

<h4 class="_fzhero1 _fw4">
  Este heading nível 1 tem tamanho de fonte nível "hero1" e font-weight: 400
</h4>
```

[//]: # (----------------------------------------------------------------------)

## White Space

> Conjunto de Classes Utilitárias que modificam a propriedade `white-space` de
um elemento.

```html
<h1 class="_wsnw">Esta h1 não tem quebras de linha</h1>
```

[//]: # (----------------------------------------------------------------------)

## Larguras

> Conjunto de Classes Utilitárias que modificam a propriedade `display` de um
elemento. Além disso, inclui uma utilitária para esconder um elemento apenas
visualmente.

```html
<td class="_2/5">Esta célula tem 40% de largura</td>
<td class="_3/5">Esta célula tem 60% de largura</td>
```

[//]: # (----------------------------------------------------------------------)

## Z-index

> Conjunto de Classes Utilitárias que modificam a propriedade `z-index` de um
elemento.

```html
<td class="_z1">Este elemento tem z-index: 1</td>
<td class="_z2">Este elemento tem z-index: 2</td>
```


[Utilitário de Larguras]:/pt-br/utilities/widths
[Objeto Layout]:/pt-br/objects/layout
[hide()]:/pt-br/tools?id=hide
