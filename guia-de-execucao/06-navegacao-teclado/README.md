# Navegação por Teclado e Foco Visual

A navegação por teclado permite que o utilizador percorra todos os elementos interativos de uma página (como links, botões e campos de formulário) utilizando apenas a tecla **Tab**.

---

## Por que é importante?

* **Deficiências Motoras:** Muitos utilizadores não conseguem utilizar um mouse e dependem de teclados adaptados.
* **Utilizadores Avançados:** Programadores experientes utilizam frequentemente o teclado para ganhar agilidade na navegação.
* **Orientação Espacial:** O foco visual (aquela "moldura" que aparece nos elementos) indica exatamente onde o utilizador está na página.

---

## Como Implementar: O Foco Visual

A regra mais importante é: **nunca remova o outline do foco sem fornecer uma alternativa visual clara**.

### Estilização do Foco em CSS

```css
/* Errado: Remove o indicador visual, impossibilitando a navegação por teclado */
:focus {
    outline: none;
}

/* Correto: Garante que o elemento em foco tenha um destaque visual nítido */
:focus {
    outline: 3px solid #1D438A; /* Cor de alto contraste */
    outline-offset: 2px;
}
