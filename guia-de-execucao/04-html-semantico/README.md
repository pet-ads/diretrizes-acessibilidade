# HTML Semântico

O HTML semântico é a base da acessibilidade na web. Ele utiliza tags que descrevem o significado do conteúdo, e não apenas sua aparência, permitindo que tecnologias assistivas (como leitores de tela) compreendam a estrutura da página.

---

## Por que usar?

* **Marcos de Navegação:** Permite que usuários de leitores de tela "saltem" entre as seções principais da página usando atalhos de teclado.
* **SEO (Search Engine Optimization):** Mecanismos de busca priorizam sites com tags semânticas, pois facilitam a indexação do conteúdo.
* **Interoperabilidade:** Garante que o site funcione corretamente em diferentes dispositivos e navegadores.

---

## Principais Tags Estruturais (Landmarks)



### 1. Elementos de Estrutura
* **`<header>`**: Representa o cabeçalho da página ou de uma seção específica.
* **`<nav>`**: Define um conjunto de links de navegação principal.
* **`<main>`**: Indica o conteúdo principal e único da página. **Regra:** Deve haver apenas um por página.
* **`<section>`**: Agrupa conteúdos relacionados de forma genérica.
* **`<article>`**: Conteúdo autônomo que faz sentido por si só (ex: um post de blog).
* **`<footer>`**: Define o rodapé da página ou seção.

---

## Hierarquia de Títulos (h1-h6)

A correta ordem dos títulos é vital para a navegação lógica:

1. **Título Principal (`<h1>`)**: Use apenas um por página para representar o assunto principal.
2. **Níveis Hierárquicos**: Use `<h2>` para seções principais, `<h3>` para subseções e assim por diante.
3. **Não pule níveis**: Nunca passe de um `<h1>` direto para um `<h3>` apenas por estética visual. O CSS deve cuidar do tamanho, enquanto o HTML cuida da estrutura.

---

## Exemplo Prático

> **Dica:** Evite o uso excessivo de `<div>` para estruturar layouts. Prefira sempre a alternativa semântica.

```html
/*Errado!*/

<div class="topo">Menu</div>
<div class="conteudo">
    <div class="titulo">Meu Artigo</div>
</div>

/*Prefira o HTML semântico.*/

<header>
    <nav>Menu</nav> </header>
<main> <article>
        <h1>Meu Artigo</h1> </article>
</main>