# Formulários Acessíveis

Um formulário acessível é aquele em que todos os utilizadores, incluindo os que usam leitores de tela ou navegação por teclado, conseguem identificar, compreender e preencher os campos de entrada sem erros.

---

## Por que é importante?

* **Identificação de Campos:** Utilizadores cegos dependem do rótulo (`<label>`) para saber o que deve ser digitado em cada campo.
* **Área de Clique:** O uso correto do `<label>` aumenta a área clicável, facilitando o uso para pessoas com dificuldades motoras.
* **Prevenção de Erros:** Instruções claras ajudam a evitar que o formulário seja submetido com dados incorretos.

---

## Como Implementar: Rótulos e Campos

A regra de ouro é nunca usar apenas o `placeholder` como etiqueta, pois ele desaparece quando o utilizador começa a digitar.

### Conexão entre Label e Input

```html
<span>Nome:</span>
<input type="text">

<label for="nome-usuario">Nome:</label> <input type="text" id="nome-usuario"> ```

---

## Boas Práticas

1. Agrupamento com `<fieldset>`: Use para agrupar campos relacionados (ex: opções de endereço ou gênero).
2. Mensagens de Erro: Se um campo for obrigatório, use o atributo `required` e forneça uma mensagem de erro clara em texto.

---

## Exemplo de Formulário Completo

```html
<form>
  <fieldset>
    <legend>Informações de Contacto</legend>
    
    <label for="email">E-mail:</label>
    <input type="email" id="email" required>
    
    <label for="mensagem">Mensagem:</label>
    <textarea id="mensagem"></textarea>
  </fieldset>
  
  <button type="submit">Enviar Formulário</button>
</form>