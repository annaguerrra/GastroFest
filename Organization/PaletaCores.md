# Brand Guide — Curitiba Gastronomic Festivals

Este documento define o padrão visual do projeto e deve ser seguido em todas as páginas para que o site mantenha a mesma identidade, mesmo sendo desenvolvido por pessoas diferentes.

O objetivo visual é transmitir uma sensação de **gastronomia local, aconchegante, moderna e elegante**, sem parecer formal demais.

---

# 1. Identidade visual

A identidade do site será baseada em:

* tons naturais e quentes;
* verde como principal cor da marca;
* terracota para ações e destaques;
* creme no fundo para evitar o aspecto muito branco/genérico;
* títulos com uma fonte mais sofisticada;
* textos e interfaces com uma fonte simples e moderna;
* cards claros, arredondados e com sombras discretas.

A interface deve parecer:

**acolhedora + gastronômica + moderna + organizada.**

Evitar:

* muitas cores diferentes;
* sombras muito fortes;
* bordas muito arredondadas;
* excesso de gradientes;
* textos completamente pretos;
* muitos elementos chamativos competindo entre si.

---

# 2. Paleta de cores

## Verde principal

**HEX:** `#3F5A45`

Principal cor da identidade.

Usar em:

* header;
* footer;
* títulos importantes;
* ícones principais;
* elementos de navegação;
* alguns botões secundários;
* detalhes da interface.

```css
--color-primary: #3F5A45;
```

---

## Verde escuro

**HEX:** `#304638`

Utilizado principalmente como variação do verde principal.

Usar em:

* hover de elementos verdes;
* footer mais escuro;
* estados ativos;
* textos sobre fundos claros quando queremos destaque.

```css
--color-primary-dark: #304638;
```

---

# 3. Terracota

**HEX:** `#C86B4A`

É a principal cor de destaque e ação do site.

Usar em:

* botões principais;
* links importantes;
* tags;
* destaques;
* elementos interativos;
* ícones que precisam chamar atenção.

Exemplo:

**Ver detalhes**

```css
--color-secondary: #C86B4A;
```

---

## Terracota escuro

**HEX:** `#A95338`

Usar principalmente em hover.

```css
--color-secondary-dark: #A95338;
```

Exemplo:

```css
.btn-primary:hover {
    background-color: var(--color-secondary-dark);
}
```

---

# 4. Dourado / Mostarda

**HEX:** `#E0A83B`

É uma cor de apoio.

Não deve aparecer em grandes áreas da página.

Usar principalmente em:

* estrelas de avaliação;
* badges especiais;
* festival em destaque;
* pequenos ícones;
* informações especiais.

```css
--color-accent: #E0A83B;
```

Exemplo:

★★★★★

As estrelas devem usar `#E0A83B`.

---

# 5. Background principal

**HEX:** `#F7F2E8`

Será o fundo principal das páginas.

```css
--color-background: #F7F2E8;
```

Evitar usar `#FFFFFF` como fundo principal do site.

O creme ajuda a deixar a interface mais aconchegante e relacionada à gastronomia.

---

# 6. Background de cards

**HEX:** `#FFFDF8`

Usar em:

* cards;
* painéis;
* caixas de informações;
* filtros;
* reviews;
* áreas destacadas.

```css
--color-surface: #FFFDF8;
```

---

# 7. Texto principal

**HEX:** `#262626`

Utilizado em:

* títulos;
* textos principais;
* informações importantes.

```css
--color-text: #262626;
```

Evitar utilizar preto puro `#000000`.

---

# 8. Texto secundário

**HEX:** `#6E6A63`

Utilizado em:

* descrições;
* datas;
* endereços;
* informações secundárias;
* textos auxiliares;
* placeholders.

```css
--color-text-secondary: #6E6A63;
```

---

# 9. Bordas

**HEX:** `#DED7CA`

Utilizar em:

* inputs;
* cards;
* divisórias;
* dropdowns;
* filtros.

```css
--color-border: #DED7CA;
```

---

# 10. Tipografia

Utilizaremos duas fontes.

## Fonte de destaque

### Playfair Display

Utilizada nos títulos principais para dar identidade ao projeto.

Usar em:

* `h1`;
* nome dos festivais;
* nome dos restaurantes;
* nome dos pratos;
* títulos principais de cada página;
* eventualmente títulos de seções importantes.

Exemplo:

```css
font-family: "Playfair Display", serif;
```

---

## Fonte principal da interface

### Inter

Utilizada em todo o restante do site.

Usar em:

* parágrafos;
* menus;
* botões;
* filtros;
* cards;
* avaliações;
* tags;
* informações;
* formulários.

```css
font-family: "Inter", sans-serif;
```

---

# 11. Importação das fontes

Adicionar no `<head>` de todas as páginas:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link
    href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Playfair+Display:wght@600;700&display=swap"
    rel="stylesheet"
>
```

---

# 12. Hierarquia de textos

## H1 — título principal da página

Fonte:

**Playfair Display**

Tamanho desktop:

`48px`

Peso:

`700`

Cor:

`#262626`

```css
h1 {
    font-family: "Playfair Display", serif;
    font-size: 48px;
    font-weight: 700;
    color: var(--color-text);
    line-height: 1.15;
}
```

Exemplo:

> Festival Gastronômico de Curitiba

---

## H2 — título de seção

Fonte:

**Playfair Display**

Tamanho:

`32px`

Peso:

`600`

Cor:

`#262626`

```css
h2 {
    font-family: "Playfair Display", serif;
    font-size: 32px;
    font-weight: 600;
    color: var(--color-text);
}
```

Exemplo:

> Restaurantes participantes

---

## H3 — título de card ou subseção

Fonte:

**Inter**

Tamanho:

`20px`

Peso:

`600`

Cor:

`#262626`

```css
h3 {
    font-family: "Inter", sans-serif;
    font-size: 20px;
    font-weight: 600;
}
```

---

# 13. Texto normal

Fonte:

**Inter**

Tamanho:

`16px`

Peso:

`400`

Cor:

`#262626`

Line-height:

`1.6`

```css
body {
    font-family: "Inter", sans-serif;
    font-size: 16px;
    line-height: 1.6;
    color: var(--color-text);
}
```

---

# 14. Texto secundário

Tamanho:

`14px`

Cor:

`#6E6A63`

Usar em:

* localização;
* datas;
* categorias;
* detalhes secundários;
* textos auxiliares.

```css
.text-secondary {
    font-size: 14px;
    color: var(--color-text-secondary);
}
```

---

# 15. Texto pequeno

Tamanho:

`12px`

Peso:

`500`

Pode ser usado para:

* badges;
* tags;
* legendas;
* informações pequenas.

---

# 16. Links

Links padrão:

```css
a {
    color: var(--color-primary);
    text-decoration: none;
}
```

Hover:

```css
a:hover {
    color: var(--color-secondary);
}
```

Evitar deixar todos os links permanentemente sublinhados.

---

# 17. Botão principal

Utilizado para a principal ação da tela.

Exemplos:

* Ver festival
* Ver restaurante
* Ver prato
* Explorar festivais

Background:

`#C86B4A`

Texto:

`#FFFFFF`

Fonte:

Inter

Peso:

`600`

Tamanho:

`15px`

Border radius:

`8px`

```css
.btn-primary {
    background-color: var(--color-secondary);
    color: #FFFFFF;

    padding: 12px 20px;

    border: none;
    border-radius: 8px;

    font-size: 15px;
    font-weight: 600;

    cursor: pointer;

    transition: 0.2s ease;
}
```

Hover:

```css
.btn-primary:hover {
    background-color: var(--color-secondary-dark);
}
```

---

# 18. Botão secundário

Background:

transparente.

Border:

`#3F5A45`

Texto:

`#3F5A45`

```css
.btn-secondary {
    background: transparent;
    color: var(--color-primary);

    border: 1px solid var(--color-primary);
    border-radius: 8px;

    padding: 11px 20px;
}
```

Hover:

```css
.btn-secondary:hover {
    background-color: var(--color-primary);
    color: white;
}
```

---

# 19. Cards

Todos os cards devem seguir aproximadamente o mesmo padrão.

Background:

`#FFFDF8`

Border:

`#DED7CA`

Border radius:

`12px`

Padding:

`20px`

Shadow:

leve.

```css
.card {
    background-color: var(--color-surface);

    border: 1px solid var(--color-border);
    border-radius: 12px;

    padding: 20px;

    box-shadow: 0 4px 16px rgba(38, 38, 38, 0.06);
}
```

Cards podem ter variações:

```html
<div class="card festival-card">
```

```html
<div class="card restaurant-card">
```

```html
<div class="card review-card">
```

O `.card` mantém o padrão geral.

As classes específicas controlam apenas diferenças necessárias.

---

# 20. Hover dos cards

Cards clicáveis podem possuir uma pequena animação.

```css
.card-clickable {
    transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.card-clickable:hover {
    transform: translateY(-3px);

    box-shadow: 0 8px 24px rgba(38, 38, 38, 0.10);
}
```

Evitar animações exageradas.

---

# 21. Imagens

As imagens são muito importantes no projeto porque gastronomia é bastante visual.

Todas devem utilizar:

```css
img {
    max-width: 100%;
    display: block;
}
```

Imagens dentro de cards:

```css
.card-image {
    width: 100%;
    height: 220px;

    object-fit: cover;

    border-radius: 10px;
}
```

Evitar:

* imagens esticadas;
* proporções diferentes dentro da mesma lista;
* imagens com border radius completamente diferente entre páginas.

---

# 22. Border radius

Para manter consistência:

### Pequeno

`6px`

Usar em:

* tags;
* pequenos elementos.

### Padrão

`8px`

Usar em:

* botões;
* inputs;
* selects.

### Cards

`12px`

### Imagens grandes

`14px`

Evitar valores aleatórios como:

```text
7px
13px
17px
21px
```

---

# 23. Espaçamento

Devemos trabalhar principalmente em múltiplos de `4px`.

Valores recomendados:

```text
4px
8px
12px
16px
20px
24px
32px
40px
48px
64px
```

---

## Espaçamento pequeno

`8px`

Entre:

* ícone e texto;
* elementos pequenos.

---

## Espaçamento interno padrão

`16px` ou `20px`

Usar dentro de:

* cards;
* inputs;
* componentes.

---

## Espaçamento entre elementos

`24px`

---

## Espaçamento entre seções

`64px`

Exemplo:

```css
section {
    margin-bottom: 64px;
}
```

---

# 24. Container padrão

Todas as páginas devem manter o conteúdo centralizado.

```css
.container {
    width: min(90%, 1200px);
    margin: 0 auto;
}
```

Isso evita que cada página tenha uma largura diferente.

---

# 25. Header

Background:

`#3F5A45`

Texto:

`#FFFFFF`

Altura aproximada:

`72px`

Links:

brancos.

Hover:

`#E0A83B`

Exemplo:

```css
.site-header {
    background-color: var(--color-primary);
    color: white;
}

.site-header a {
    color: white;
}

.site-header a:hover {
    color: var(--color-accent);
}
```

---

# 26. Footer

Background:

`#304638`

Texto principal:

`#FFFFFF`

Texto secundário:

preferencialmente um branco com transparência.

```css
.site-footer {
    background-color: var(--color-primary-dark);
    color: white;
}
```

---

# 27. Inputs, busca e filtros

Background:

`#FFFDF8`

Border:

`#DED7CA`

Texto:

`#262626`

Border radius:

`8px`

```css
input,
select {
    background-color: var(--color-surface);

    border: 1px solid var(--color-border);
    border-radius: 8px;

    padding: 12px 14px;

    font-family: "Inter", sans-serif;
    font-size: 15px;

    color: var(--color-text);
}
```

Quando estiver selecionado:

```css
input:focus,
select:focus {
    outline: none;
    border-color: var(--color-primary);
}
```

---

# 28. Tags

Podemos utilizar tags para categorias como:

```text
Italiano
Hambúrguer
Japonês
Festival participante
Vegano
```

Sugestão:

Background:

`#F1E7D7`

Texto:

`#3F5A45`

```css
.tag {
    display: inline-block;

    background-color: #F1E7D7;
    color: var(--color-primary);

    padding: 6px 10px;

    border-radius: 6px;

    font-size: 12px;
    font-weight: 600;
}
```

---

# 29. Avaliações

Estrela preenchida:

`#E0A83B`

Estrela vazia:

`#DED7CA`

Nota:

`#262626`

Exemplo:

```text
★★★★★ 4.8
```

Não utilizar verde ou terracota nas estrelas.

---

# 30. Ícones

Os ícones normalmente devem utilizar:

`#3F5A45`

ou

`#6E6A63`

Terracota pode ser utilizado para ações imp
